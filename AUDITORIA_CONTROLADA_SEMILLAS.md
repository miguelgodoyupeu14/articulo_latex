# Auditoría bibliográfica controlada de Introducción, Discusión y Conclusiones

Fecha de cierre: 7 de octubre de 2026.

## Alcance y fuentes comprobadas

La edición se limitó a Introducción, Discusión y Conclusiones. El texto y los datos de Metodología y Resultados se compararon automáticamente con la copia anterior a esta tarea y permanecen idénticos. La corrección ortográfica de una vocal dañada en el diagrama PRISMA (`evaluaci?n` → `evaluación`) estaba pendiente de la revisión anterior y no altera cifras ni decisiones metodológicas.

La comparación de solapamiento utilizó los 99 registros de la hoja `ARTÍCULOS PRESELECCIONADOS` del archivo `Articulos (1).xlsx`, identificados por DOI. Se consultó `Manual Parsifal Cypher.docx` para comprobar el alcance del protocolo; el manual no contiene una lista independiente de artículos semilla. Se revisó el texto completo de los 15 antecedentes usados en Introducción y se verificaron sus metadatos bibliográficos por DOI.

## A. Antecedentes científicos de Introducción

La columna Scopus se verificó mediante consulta individual del DOI en la API oficial de Scopus. Cada respuesta devolvió un EID `2-s2.0-*`. No se atribuyó indexación en Web of Science sin una consulta verificable a esa base. `olmos2018` también se verificó en ScienceDirect mediante su DOI y PII; los demás trabajos están alojados en otras plataformas editoriales.

| Clave BibTeX | Título | Año | DOI | Scopus | Web of Science | ScienceDirect | Fuente verificada | Idea que respalda en la Introducción | ¿Pertenece a los 99? |
|---|---|---:|---|---|---|---|---|---|---|
| `sultani2018` | Real-World Anomaly Detection in Surveillance Videos | 2018 | 10.1109/CVPR.2018.00678 | Sí | No comprobado | No | Scopus EID 2-s2.0-85056851488 | Diversidad de anomalías y aprendizaje con etiquetas a nivel de video | No |
| `cheng2021` | RWF-2000: An Open Large Scale Video Database for Violence Detection | 2021 | 10.1109/ICPR48806.2021.9412502 | Sí | No comprobado | No | Scopus EID 2-s2.0-85110515836 | Costo del monitoreo manual, violencia en CCTV y RWF-2000 | No |
| `tran2015` | Learning Spatiotemporal Features with 3D Convolutional Networks | 2015 | 10.1109/ICCV.2015.510 | Sí | No comprobado | No | Scopus EID 2-s2.0-84973865953 | Representación espacio-temporal mediante C3D | No |
| `wang2016` | Temporal Segment Networks: Towards Good Practices for Deep Action Recognition | 2016 | 10.1007/978-3-319-46484-8_2 | Sí | No comprobado | No | Scopus EID 2-s2.0-84990047892 | Estructura temporal de largo alcance en reconocimiento de acciones | No |
| `olmos2018` | Automatic handgun detection alarm in videos using deep learning | 2018 | 10.1016/j.neucom.2017.05.012 | Sí | No comprobado | Sí | Scopus EID 2-s2.0-85019947234; ScienceDirect PII S0925231217308196 | Detección de pistolas, falsas alarmas y condiciones visuales | No |
| `carreira2017` | Quo Vadis, Action Recognition? A New Model and the Kinetics Dataset | 2017 | 10.1109/CVPR.2017.502 | Sí | No comprobado | No | Scopus EID 2-s2.0-85044290845 | I3D, Kinetics y transferencia para reconocimiento de acciones | No |
| `liuswin2022` | Video Swin Transformer | 2022 | 10.1109/CVPR52688.2022.00320 | Sí | No comprobado | No | Scopus EID 2-s2.0-85132940057 | Atención en ventanas espacio-temporales para video | No |
| `liu2018` | Future Frame Prediction for Anomaly Detection – A New Baseline | 2018 | 10.1109/CVPR.2018.00684 | Sí | No comprobado | No | Scopus EID 2-s2.0-85062695405 | Predicción de fotogramas y restricciones de apariencia y movimiento | No |
| `gong2019` | Memorizing Normality to Detect Anomaly: Memory-Augmented Deep Autoencoder for Unsupervised Anomaly Detection | 2019 | 10.1109/ICCV.2019.00179 | Sí | No comprobado | No | Scopus EID 2-s2.0-85081894025 | Memoria de patrones normales para detectar anomalías | No |
| `ullah2021` | An Efficient Anomaly Recognition Framework Using an Attention Residual LSTM in Surveillance Videos | 2021 | 10.3390/s21082811 | Sí | No comprobado | No | Scopus EID 2-s2.0-85104309011 | CNN ligera y LSTM residual con atención para anomalías | No |
| `wojke2017` | Simple Online and Realtime Tracking with a Deep Association Metric | 2017 | 10.1109/ICIP.2017.8296962 | Sí | No comprobado | No | Scopus EID 2-s2.0-85045318361 | Seguimiento mediante asociación de movimiento y apariencia | No |
| `zhang2022` | ByteTrack: Multi-Object Tracking by Associating Every Detection Box | 2022 | 10.1007/978-3-031-20047-2_1 | Sí | No comprobado | No | Scopus EID 2-s2.0-85142725518 | Uso de detecciones de baja confianza para evitar trayectorias fragmentadas | No |
| `zheng2015` | Scalable Person Re-identification: A Benchmark | 2015 | 10.1109/ICCV.2015.133 | Sí | No comprobado | No | Scopus EID 2-s2.0-84973855896 | Definición y evaluación de re-identificación en múltiples cámaras | No |
| `zhou2019` | Omni-Scale Feature Learning for Person Re-Identification | 2019 | 10.1109/ICCV.2019.00380 | Sí | No comprobado | No | Scopus EID 2-s2.0-85081935131 | Representaciones a distintas escalas para re-identificación | No |
| `barthelemy2024` | Safety After Dark: A Privacy Compliant and Real-Time Edge Computing Intelligent Video Analytics for Safer Public Transportation | 2024 | 10.3390/s24248102 | Sí | No comprobado | No | Scopus EID 2-s2.0-85213079003 | Integración local, comunicación de alertas y prueba de campo | No |

`ullah2021` y `barthelemy2024` ya estaban en `snbibliography.bib`. Las otras trece entradas se incorporaron después de revisar su texto completo. En el artículo se describen únicamente como antecedentes científicos utilizados para contextualizar la Introducción. No se afirma que hayan sido semillas originales del protocolo: el manual de Parsifal no registra una lista histórica de artículos semilla.

## B. Referencias eliminadas de Introducción

Las siguientes claves estaban citadas en la Introducción inmediatamente antes de esta tarea y se retiraron porque sus DOI sí aparecen entre los 99 estudios: `ahmed2022`, `amado2024`, `berardini2024`, `berardini2025`, `bhatti2021`, `ciampi2022`, `fierrosilva2026`, `garciacobo2023`, `hnoohom2022`, `magdy2023`, `mehmood2021`, `rendon2021`, `rendon2023`, `sernani2021` y `vijeikis2022`. No se eliminaron del archivo bibliográfico ni de otras secciones donde cumplen otra función.

## C. Referencias metodológicas reubicadas

Kitchenham (`kitchenham2007`) y PRISMA (`page2021`) no se usan como antecedentes temáticos. Ya habían sido retiradas de Introducción en la revisión previa y se mantuvieron únicamente en Metodología, junto con las demás referencias que justifican el diseño de la revisión. Esta tarea no modificó la Metodología.

## D. Citas múltiples

Al iniciar esta corrección controlada, la Introducción ya no contenía agrupaciones del tipo `\cite{a,b}`. La nueva versión mantiene una fuente principal por afirmación: 15 llamadas de cita y 15 claves diferentes. La comprobación automática confirma cero citas múltiples en esa sección.

## E. Discusión

Se incorporaron cuatro estudios pertenecientes a los 99 que no forman parte de los 35 analizados en detalle:

| Clave | Registro del Excel | Interpretación respaldada | ¿Está entre los 35? |
|---|---|---|---|
| `vijeikis2022` | AR-017 | Relación entre diseño ligero, MobileNet V2, LSTM y tarea temporal | No |
| `hnoohom2022` | AR-041 | Limitaciones de iluminación, entorno y tipos de arma en ACF | No |
| `rendon2021` | AR-057 | Diferencia entre validación interna y pruebas entre datasets | No |
| `ahmed2022` | AR-013 | Dependencia del rendimiento respecto del equipo y la optimización para edge | No |

La Discusión conserva además estudios de los 35 cuando son necesarios para interpretar arquitectura, eventos, adaptación de dominio e implementación. El conteo de Resultados no se recalculó: el texto completo de `rendon2021` describe una prueba entre datasets que debe contrastarse con la clasificación agregada de tres estudios si en el futuro se audita la matriz de extracción.

## F. Conclusiones

La Conclusión no contiene citas externas. Resume los resultados ya expuestos: técnicas y eventos predominantes, menor presencia de seguimiento e identificación, uso de benchmarks, generalización, heterogeneidad de métricas, tiempo real, despliegue y trabajo futuro. Se reemplazaron expresiones internas por `estudios seleccionados` o formulaciones equivalentes sin modificar cifras.

## G. Solapamiento y controles automáticos

- Antecedentes de Introducción presentes también entre los 99: **0**.
- Antecedentes confirmados en Scopus: **15 de 15**.
- Antecedentes confirmados adicionalmente en ScienceDirect: **1 de 15** (`olmos2018`).
- Indexación en Web of Science: no se atribuyó cuando no pudo consultarse directamente; no es necesaria para cumplir la condición porque todos fueron confirmados en Scopus.
- Claves BibTeX usadas sin entrada: **0**.
- DOI duplicados entre los tres archivos bibliográficos: **0**.
- Antecedentes científicos diferentes en Introducción: **15**.
- Citas múltiples en Introducción: **0**.
- Referencias únicas: Introducción 15; Metodología 13; Resultados 35; Discusión 11; Conclusiones 0; total del artículo 67.
- Metodología: idéntica a la versión anterior a esta tarea.
- Resultados: idéntica a la versión anterior a esta tarea.

La auditoría reproducible quedó registrada en `build/auditoria-controlada.json`; los PDF y textos extraídos empleados para comprobar el contenido se conservaron en `build/seed-evidence/` como material local de revisión y no forman parte de la bibliografía publicada.

## Validación de compilación y presentación

El proyecto compiló con `latexmk`, BibTeX y las pasadas necesarias de pdfLaTeX. El PDF final contiene 37 páginas. Se comprobó el texto extraído y la disposición visual de la Introducción, la Discusión, la Conclusión y las páginas de referencias. No hay referencias indefinidas, marcadores `[?]`, claves inexistentes, DOI duplicados ni cajas `Overfull`.

El registro mantiene 51 avisos `Underfull`, tres avisos de ajuste de flotantes, cuatro sustituciones de tamaño de fuentes matemáticas, tres mensajes no fatales de `Infinite glue shrinkage` asociados a tablas largas y un ajuste de nivel de marcador. Estos avisos no produjeron texto fuera de margen ni tablas cortadas en la revisión visual. MiKTeX también muestra su recordatorio local de actualizaciones pendientes; no afecta el contenido del artículo.
