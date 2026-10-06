# Revisión integral del manuscrito

Fecha: 6 de octubre de 2026. Estado: primera versión revisada; no constituye todavía una versión lista para envío.

## Cambios de contenido

- Se corrigieron la puntuación del título y el título abreviado, sin cambiar el tema ni la autoría.
- El resumen de ejemplo se sustituyó por un resumen de 191 palabras y palabras clave pertinentes, en español.
- Se revisó la Introducción para presentar el problema, las familias de soluciones, las limitaciones de comparación y el aporte. Se retiraron afirmaciones generales no justificadas sobre superioridad tecnológica, atención humana, prevención y carencias de todas las revisiones previas. No se eliminaron las entradas bibliográficas correspondientes.
- Se corrigió la Metodología con las cifras finales proporcionadas y el reporte de Parsifal. Se separaron PICOC, preguntas, selección, calidad, extracción, Reporting Core, bibliometría y amenazas a la validez.
- Se conservó la estructura de Resultados, incluida la tabla de 35 estudios. Se formalizó la síntesis final como 3.4 y se completaron los desgloses auditados de RQ1 y RQ2.
- Se redactó una Discusión con cuatro apartados: arquitecturas y tareas; generalización y comparabilidad; rendimiento experimental frente a operación; relación con bibliometría y límites de la revisión.
- Se redactaron cinco párrafos de Conclusiones que responden la pregunta general y delimitan las líneas futuras sin declarar un modelo ganador.
- Se eliminaron las instrucciones visibles de Springer, el apéndice de ejemplo y las declaraciones genéricas. Se incluyó únicamente una descripción verificable de los datos utilizados; no se inventaron ausencia de financiamiento, ausencia de conflictos ni contribuciones individuales.

## Inconsistencias corregidas

| Aspecto | Versión anterior | Versión revisada |
|---|---|---|
| Registros identificados | 477 | 510 |
| Bases | WoS 299, Scopus 148, ScienceDirect 30 | WoS 105, Scopus 145, ScienceDirect 260 |
| Duplicados | 79 | 113 |
| Selección | 91 rechazados y 307 aceptados; la introducción mencionaba 373 cribados | 397 únicos, 249 rechazados y 148 aceptados |
| Calidad | 307 evaluados, criterio inclusivo ≥7,0, 256 elegibles y auditorías posteriores de 253/204 | 148 evaluados, 99 PASS ≥7,5 y 49 FAIL ≤7,0 |
| Casos con QA=7,0 | 45 y considerados elegibles | 7; incluidos en los 49 FAIL |
| Instrumento QA | Introducción: cinco preguntas; método: diez con contenido distinto | Diez preguntas QA1–QA10, cotejadas con el reporte final |
| Extracción | 20 campos y 211 estudios | 30 campos × 99 estudios = 2.970 celdas |
| Corpus | 45 trabajos y 35 como corpus final en la Introducción | 99 elegibles; Reporting Core intencional de 35; otros 64 incluidos en conteos |
| Marco | PICOCT con tiempo como dimensión | PICOC; 2021–2026 como filtro |
| Exclusiones | CE1 era duplicación; distribución no consolidada | IC1–IC4 y EC1–EC6 del reporte; 33+45+46+102+23+0=249 |
| UCF-Crime en Introducción | 13/35 | Se retiró el adelanto obsoleto; Resultados conserva 15/99 |
| Tres campos | Autores, fuentes y conceptos | TI_TM, ID y KW_Merged: vocabularios bibliográficos |
| Mapa de acoplamiento | Mapa temático genérico | Centralidad e impacto; sin inferir densidad, temas motores o tamaño de burbujas |

Se retiraron las cifras de auditorías intermedias porque no describen el corpus definitivo. Las versiones anteriores permanecen en Git y en el respaldo local.

## Control de metodología y resultados

Se verificó la aritmética: 510−113=397; 397−249=148; 148−49=99; 35+64=99. El umbral configurado de 7,0 se distingue del efectivo de 7,5. Los siete casos con 7,0 no se suman otra vez al total de FAIL.

Las frecuencias de RQ1–RQ5 se conservaron conforme a los valores auditados aportados. Se añadieron 14/20 apariciones de YOLO en detección de armas, arma no especificada (11/99) y el desglose multietiqueta de seguimiento, identificación y reconocimiento facial. Se mantuvieron las cuatro comparaciones de desempeño moderadas, sin promedios globales ni rankings. Los 35 estudios del Core y sus claves bibliográficas se conservaron.

Se distingue entre falta de reporte y ausencia real de una capacidad. La no identificación de evaluaciones de re-ID corresponde al corpus recuperado, no a toda la literatura.

## Revisión bibliométrica

Se verificaron los 145 registros de `../bibliometrix/Scopus.csv`: producción anual, principales fuentes, palabras clave y promedios de citas. El promedio de 2022 es 53,625; se conserva 53,63 mediante redondeo decimal convencional. El total de 555 corresponde a nombres completos distintos; 521 de esas etiquetas aparecen en un documento. Se aclaró la unidad de conteo, pues las iniciales o identificadores producen totales distintos.

| Figura | Interpretación revisada y límites |
|---|---|
| Three-Field Plot | Términos de título TI_TM, palabras de indexación ID y palabras combinadas KW_Merged. ID no contiene documentos ni autores en esta imagen. |
| Country Collaboration Map | Distribución y vínculos internacionales; sin inferir liderazgo institucional del color. |
| Collaboration Network | Grupos de coautoría con conexiones internas; sin afirmar una comunidad única. |
| Co-citation Network | Referencias citadas conjuntamente; no se asignan especialidades a cada color con etiquetas superpuestas. |
| Historiograph | Relaciones bibliográficas a través del tiempo; sin causalidad. Se mencionan únicamente etiquetas legibles. |
| Clustering by Coupling | Documentos con referencias compartidas; se distinguen nodos y periferia sin atribuir temas no verificables. |
| Co-occurrence Network | Posición visual central de deep learning y asociaciones de términos; sin convertirla en una medida matemática. |
| Coupling Map | Ejes Centrality e Impact. No se interpreta el tamaño de burbuja sin configuración. El archivo original tiene texto truncado a la derecha. |
| Factorial Map | MCA, ejes 24,41 % y 18,12 %; proximidad conceptual, sin inferir dominio por área del polígono. |
| Word Cloud | Frecuencia relativa; no demuestra relaciones entre palabras. |

También se inspeccionó el dendrograma disponible como recurso, que no está incluido en el manuscrito. No se añadió como un resultado nuevo.

La interpretación de ID se contrastó con la [documentación oficial de campos de Bibliometrix](https://www.bibliometrix.org/documents/Field_Tags_bibliometrix.pdf). El archivo normalizado conserva columnas separadas DE, ID y KW_Merged. No se equiparan las frecuencias de palabras clave de autor con las del vocabulario combinado de las figuras.

## Referencias

La auditoría estructural encontró 57 entradas en los dos archivos `.bib`, 55 claves utilizadas y ningún identificador BibTeX duplicado, DOI duplicado o cita sin entrada. Las dos entradas que dejaron de citarse permanecen en la biblioteca; no se forzó su aparición en la bibliografía.

Solo se corrigieron dos rangos de páginas incompletos, comprobados en el archivo Scopus:

- `shah2023`: 528 → 528–544.
- `muriithi2024`: 2666 → 2666–2673.

No se cambiaron claves ni se crearon referencias nuevas. Se mantienen `sandhya2022` con año bibliográfico 2023 y `lin2025` con año 2026; el nombre de una clave interna no determina el año de publicación. Esta revisión no equivale a una nueva extracción de texto completo de los 99 estudios.

## Aspectos que requieren confirmación

1. **Cadenas ejecutadas y fecha de búsqueda.** El `.tex` histórico contiene consultas sin bloque de tracking; el reporte de Parsifal presenta otras consultas con tracking. Las instrucciones recibidas también indican ausencia del bloque histórico. No se atribuyeron a los 510 registros ecuaciones cuya ejecución no está confirmada. El manuscrito hace explícita esta discrepancia. Hace falta el historial/exportación que vincule consulta, fecha y resultados; no basta elegir la cadena metodológicamente más conveniente.
2. **Declaraciones de autores.** Financiamiento, conflictos, contribuciones individuales y permiso de publicación de la matriz no están confirmados. Se consultaron al usuario y no se sustituyeron por afirmaciones de ausencia.
3. **Exportaciones bibliométricas.** Coupling Map contiene etiquetas cortadas; varias redes tienen texto solapado o de bajo contraste en la imagen fuente. Un cambio de ancho en LaTeX no recupera etiquetas que no están en el PNG. Conviene reexportar las mismas salidas desde Bibliometrix con sus parámetros originales, preferentemente en formato vectorial. No se reconstruyeron valores ni clusters.
4. **Revista de destino.** No se identificó una revista concreta. Idioma, extensión, formato de declaraciones y otros requisitos deberán cotejarse con sus instrucciones antes del envío. No se afirma preparación definitiva para publicación Q1 ni se garantiza similitud textual.

## Archivos de entrega

- `sn-article.tex`: contenido, organización, tablas, figuras y cierre del artículo.
- `core35_refs.bib`: dos rangos de páginas corregidos.
- `REVISION_INTEGRAL.md`: este informe de cambios, comprobaciones y pendientes.
- `build/sn-article.pdf`: PDF compilado, excluido de Git según la configuración existente.

Se conservaron la clase `sn-jnl.cls`, el estilo bibliográfico, `snbibliography.bib`, los originales de las figuras y la configuración de VS Code. Los scripts y renders de comprobación permanecen en `build/`, y los respaldos en `backups/`; ambas carpetas están excluidas de Git.

## Compilación y revisión visual

Comando de compilación, desde la carpeta del proyecto y con MiKTeX y Perl en PATH:

```sh
latexmk -g -pdf -bibtexfudge- -synctex=1 -interaction=nonstopmode -file-line-error -halt-on-error -outdir=build sn-article.tex
```

Se utilizó `-g` para repetir la compilación después de instalar `placeins`. No se cambiaron los márgenes, el ancho de texto ni el interlineado de Springer. Se ajustaron columnas, tipos de floats, tamaños de figuras y barreras entre subsecciones. El recorte de colocación de la nube de palabras afecta únicamente su espacio blanco, sin modificar el PNG original.

La compilación definitiva produjo un PDF de 34 páginas, revisadas visualmente en su totalidad. El registro final no contiene referencias indefinidas, destinos duplicados ni desbordamientos horizontales o verticales (`Overfull`). Las 55 referencias citadas se resuelven correctamente. Se corrigieron también las colisiones de anclas de las tablas y se mantuvieron completas las tablas breves cuando su tamaño lo permitía.

Persisten 3 avisos `Underfull hbox`, 34 `Underfull vbox` y 4 avisos de fuentes de LaTeX; no impiden la compilación. No se alteraron los márgenes para eliminarlos. Las limitaciones de legibilidad y las etiquetas truncadas que ya existen en las figuras originales siguen pendientes de una nueva exportación, según el inventario anterior. La revisión editorial está completada como primer borrador integral; la confirmación de las búsquedas y las declaraciones de los autores sigue siendo necesaria antes del envío.
