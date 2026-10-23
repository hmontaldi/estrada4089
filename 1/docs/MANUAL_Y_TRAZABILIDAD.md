# Manual de usuario y trazabilidad — Front End

## Curso: Teorema de Pitágoras

### Alcance
Este proyecto implementa únicamente el Front End. No incluye backend, autenticación real, base de datos, almacenamiento de resultados ni emisión real de certificados.

### Ejecución
Abrir `index.html` en un navegador moderno.

### Paleta visual
- Azul oscuro: `#0B3558`
- Azul secundario: `#0D456F`
- Azul de acción: `#0D6EFD`
- Verde de aprobación: `#16A06D`
- Fondo: `#F4F8FC`
- Error: `#EA4F4F`

### Matriz de trazabilidad
| ID | Pantalla | Archivo | Salida principal |
|---|---|---|---|
| SCR-01 | Inicio | index.html | SCR-02 |
| SCR-02 | Índice | 02_indice.html | SCR-03 |
| SCR-03 | Teoría | 03_teoria.html | SCR-04 |
| SCR-04 | Video | 04_video.html | SCR-10 |
| SCR-10 | Aplicaciones | 10_aplicaciones.html | SCR-11 |
| SCR-11 | Práctica | 11_practica.html | SCR-05 |
| SCR-05 | Evaluación | 05_evaluacion.html | SCR-06 / SCR-12 |
| SCR-06 | Feedback correcto | 06_feedback.html | SCR-07 |
| SCR-12 | Feedback incorrecto | 12_error.html | SCR-05 / SCR-03 |
| SCR-07 | Resultado | 07_resultado.html | SCR-08 / SCR-14 |
| SCR-08 | Certificado | 08_certificado.html | Impresión del navegador |
| SCR-09 | Mis cursos | 09_mis_cursos.html | SCR-02 |
| SCR-13 | Certificados | 13_certificados.html | SCR-08 |
| SCR-14 | Finalización | 14_felicitaciones.html | SCR-01 |
| SCR-15 | Recursos | 15_recursos.html | SCR-03/04/11 |
| SCR-16 | Ayuda | 16_ayuda.html | SCR-01 |

### Eventos principales
| ID | Evento | Acción |
|---|---|---|
| EVT-01 | Comenzar curso | Abre índice |
| EVT-02 | Anterior/Siguiente | Navega entre pantallas |
| EVT-03 | Seleccionar respuesta | Resalta opción |
| EVT-04 | Respuesta correcta | Abre feedback correcto |
| EVT-05 | Respuesta incorrecta | Abre feedback incorrecto |
| EVT-06 | Ver certificado | Abre certificado |
| EVT-07 | Imprimir certificado | Ejecuta `window.print()` |
| EVT-08 | Ayuda | Expande/contrae respuestas |

### Separación Front End / Back End
Implementado: diseño, navegación, selección visual, progreso de muestra, resultado de muestra, certificado visual e impresión.

No implementado: login, usuarios reales, corrección persistente, almacenamiento, API, base de datos, firma digital, seguridad o generación de PDF en servidor.

### Convención de seguimiento
Usar IDs `SCR-XX` para pantallas, `EVT-XX` para eventos y `REQ-XX` para futuros requerimientos. Ejemplo: `REQ-EVA-01 -> SCR-05 -> EVT-03 -> SCR-06/SCR-12`.
