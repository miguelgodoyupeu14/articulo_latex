# ARGUS-RSL — artículo LaTeX

Manuscrito Springer Nature. Archivo principal: **sn-article.tex**, conservado en un único archivo.

## Preparar otro equipo

Instalar Git, VS Code, MiKTeX y la extensión **LaTeX Workshop** (James Yu).

```sh
git clone https://github.com/miguelgodoyupeu14/articulo_latex.git
cd articulo_latex
code .
```

Abrir con **File > Open Folder**. Copiar `.vscode/settings.example.json` a `.vscode/settings.json` si no existe una configuración local. Esta última está excluida de Git para poder adaptar las rutas en cada equipo.

Comprobar que `pdflatex --version` y `bibtex --version` funcionan en una terminal nueva. Si no, añadir los ejecutables de MiKTeX al PATH y reiniciar VS Code. Permitir la instalación de paquetes faltantes mediante MiKTeX.

La configuración de ejemplo usa pdfLaTeX → BibTeX → pdfLaTeX → pdfLaTeX, sin necesitar Perl. También incluye latexmk, que requiere Perl en el PATH. La configuración local original mantiene su receta ya verificada.

## Compilar y visualizar

Abrir **sn-article.tex**, pulsar **Ctrl + Alt + B** y después **Ctrl + Alt + V** para ver el PDF, o ejecutar **LaTeX Workshop: View LaTeX PDF**.

Salida: **build/sn-article.pdf**. Elegir recetas con **LaTeX Workshop: Build with recipe**.

Con latexmk y Perl:

```sh
latexmk -pdf -bibtexfudge- -outdir=build sn-article.tex
```

La opción `-bibtexfudge-` mantiene BibTeX en la raíz para localizar bibliografías y estilos.

Alternativa desde PowerShell:

```powershell
New-Item -ItemType Directory -Path build -Force | Out-Null
pdflatex -synctex=1 -interaction=nonstopmode -halt-on-error -output-directory=build sn-article.tex
bibtex build/sn-article
pdflatex -synctex=1 -interaction=nonstopmode -halt-on-error -output-directory=build sn-article.tex
pdflatex -synctex=1 -interaction=nonstopmode -halt-on-error -output-directory=build sn-article.tex
```

## Colaborar

El propietario debe invitar al compañero desde **GitHub > Settings > Collaborators**. El compañero debe aceptar para poder subir cambios al mismo repositorio.

Antes de un cambio, con el trabajo previo confirmado:

```sh
git switch main
git pull --ff-only
git switch -c revision-resultados
```

Usar un nombre de rama diferente para cada cambio. Después de editar y compilar:

```sh
git add sn-article.tex
git commit -m "Revisa resultados"
git push -u origin revision-resultados
```

Añadir explícitamente bibliografías o figuras si también cambiaron. Abrir un **Pull Request** en GitHub hacia `main` para revisión e integración. Después, volver a `main` y hacer `git pull --ff-only` antes de iniciar otra rama.

Coordinar qué sección edita cada persona reduce conflictos. Git permite compartir cambios y revisarlos; no es edición simultánea. Resolver los conflictos comparando ambos textos y recompilar antes de confirmar.

## Bibliografía, figuras y limpieza

- Conservar separados `snbibliography.bib` y `core35_refs.bib`. Las 35 claves del Reporting Core tienen entradas entre ambos archivos.
- Ante citas `[?]`, comprobar las claves, revisar `build/sn-article.blg` y ejecutar la receta completa. No inventar referencias ni borrar citas para ocultarlas.
- Las figuras están en `figures/` y se localizan mediante `\graphicspath{{figures/}}`.
- La clave `lin2025` se conserva; el año del volumen es 2026 y su publicación online fue en 2025.
- Usar **LaTeX Workshop: Clean up auxiliary files** y volver a compilar. La limpieza configurada conserva fuentes, bibliografías, imágenes, estilos, PDF y `.bbl`.
- Para recompilar sin borrar: `latexmk -g -pdf -bibtexfudge- -outdir=build sn-article.tex`.

## Archivos compartidos

```text
sn-article.tex
sn-jnl.cls
sn-mathphys-num.bst
snbibliography.bib
core35_refs.bib
figures/
bst/
user-manual.pdf
empty.eps
fig.eps
.vscode/settings.example.json
.vscode/extensions.json
```

Los respaldos, diagnósticos, configuración personal y resultados de compilación quedan excluidos mediante `.gitignore` y se conservan localmente.
