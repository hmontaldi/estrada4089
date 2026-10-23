# Manual del usuario y trazabilidad — Arquitectura de Hardware

## 1. Propósito y alcance
Maqueta navegable de Front End construida con HTML, CSS y JavaScript para servir como punto de partida de una futura Aplicación Web. No incluye Back End ni base de datos. Está diseñada principalmente para PC, netbook y notebook, conservando la paleta y distribución visual de la maqueta de referencia: barra lateral azul marino, fondo gris claro, tarjetas blancas, acciones azules y progreso verde.

## 2. Organización de los contenidos
El curso presenta seis módulos temáticos, siguiendo los grupos del material fuente: Grupo 1, Procesador y memoria; Grupo 2, Almacenamiento; Grupo 3, Placa madre y expansión; Grupo 4, Periféricos; Grupo 5, Conectividad y alimentación. El Grupo 3 incorpora motherboard, socket, chipset, BIOS, UEFI, ranuras de expansión, PCI Express, SATA, M.2 y tarjetas de expansión. Los recursos audiovisuales enlazados son los incluidos en el documento aportado.

## 3. Inventario y trazabilidad de pantallas
| ID | Archivo | Pantalla | Origen/función |
|---|---|---|---|
| P01 | `index.html` | Inicio | Presentación general |
| P02 | `02_indice.html` | Índice del curso | Organización de los seis módulos |
| P03 | `03_procesador_memoria.html` | Procesador y memoria | Grupo 1 |
| P04 | `04_almacenamiento.html` | Almacenamiento | Grupo 2 |
| P05 | `05_placa_madre.html` | Placa madre y expansión | Grupo 3 |
| P06 | `06_perifericos.html` | Periféricos | Grupo 4 |
| P07 | `07_conectividad.html` | Conectividad | Grupo 5 |
| P08 | `08_alimentacion.html` | Alimentación | Grupo 5 |
| P09 | `09_recursos.html` | Recursos | Enlaces audiovisuales incluidos en Grupo 3 |
| P10 | `10_practica.html` | Práctica | Actividad formativa sobre placa madre y expansión |
| P11 | `11_evaluacion.html` | Evaluación | Preguntas integradoras de los grupos temáticos |
| P12 | `12_resultado.html` | Resultado | Cálculo local de puntaje |
| P13 | `13_certificado.html` | Certificado | Impresión desde navegador |
| P14 | `14_mis_cursos.html` | Mis cursos | Pantalla demostrativa |
| P15 | `15_ayuda.html` | Ayuda | Manual de uso |
| P16 | `16_error.html` | Error | Estado de contingencia demostrativo |

## 4. Mapa de navegación
Inicio → Índice → Módulos 1 a 6 → Recursos → Práctica → Evaluación → Resultado → Certificado (si se alcanza 60 %). Todos los destinos principales también están disponibles en la barra lateral. Mis cursos, Ayuda y Error son pantallas complementarias.

## 5. Archivos y responsabilidades
- `index.html` y los archivos HTML numerados: estructura y contenido de cada pantalla.
- `css/styles.css`: paleta, barra lateral, distribución, tarjetas, controles, evaluación, certificado y reglas de presentación.
- `js/app.js`: navegación activa, progreso local, devolución de práctica, cálculo de evaluación, resultado, nombre del estudiante y fecha del certificado.
- `docs/MATRIZ_TRAZABILIDAD.csv`: relación tabular entre ID, archivo, pantalla y contenido/función.

## 6. Datos y lógica del Front End
Se utiliza `localStorage` del navegador para `ah_progress`, `ah_score`, `ah_exam_total` y `ah_student_name`. Las respuestas de evaluación se califican localmente. El umbral de aprobación de la maqueta es 60 %. El certificado se imprime o guarda como PDF mediante la función de impresión del navegador; no se genera ni valida en un servidor.

## 7. Cómo ejecutar
1. Descomprimí el ZIP en una carpeta.
2. Abrí `index.html` con Chrome, Edge o Firefox.
3. Navegá con la barra lateral o los enlaces de cada pantalla.
4. Para el certificado, completá la evaluación y elegí “Imprimir / Guardar PDF”.

## 8. Límites explícitos
No hay autenticación, perfiles reales, persistencia centralizada, base de datos, Back End, panel docente, validación de identidad ni emisión de certificados verificables. Los enlaces externos dependen de la disponibilidad de los recursos. El progreso local puede perderse al borrar los datos del navegador o cambiar de dispositivo.

## 9. Recomendaciones para continuidad del proyecto
Mantener los identificadores P01–P16. Si se implementa Back End posteriormente, documentar para cada pantalla los datos requeridos, validaciones, servicios/endpoints, respuestas esperadas y manejo de errores. No tratar los datos guardados en localStorage como información segura ni oficial.
