# Manual de usuario y trazabilidad — Sistemas Digitales y Redes
**Institución:** Escuela N.º 4-089 “José Manuel Estrada” · **Versión:** 1.0 · **Octubre de 2026**

## 1. Propósito
Maqueta navegable para evaluar una posible distribución de pantallas de una aplicación educativa. Mantiene la referencia visual: barra lateral azul marino, encabezado con ruta y usuario, tarjetas blancas, botones azules, indicadores verdes y fondo gris claro.

## 2. Alcance
Incluye HTML, CSS y JavaScript del lado del navegador. No incluye Back End, API, autenticación real, base de datos ni sincronización. El nombre y los resultados se guardan localmente cuando el navegador lo permite. El certificado es de demostración, imprimible, y no oficial. El video es un marcador visual, no un recurso incrustado.

## 3. Cómo abrir
1. Descomprimir el ZIP conservando la estructura.
2. Abrir `index.html` en Chrome, Edge o Firefox.
3. Usar “Comenzar curso”, avanzar por los módulos, resolver la práctica y completar la evaluación.
4. Para imprimir, abrir Certificado y elegir “Imprimir / Guardar PDF”.
5. No mover archivos HTML: dependen de `css/styles.css` y `js/app.js`.

## 4. Mapa de navegación
P01 Inicio → P02 Índice → P03 Sistemas digitales → P04 Video → P05 Circuitos lógicos → P06 Devolución → P07 Memorias → P08 Redes → P09 Práctica → P10 Resultado de práctica → P11 Evaluación final → P12 Resultado → P13 Certificado. La barra lateral enlaza además con P14 Mis cursos y P15 Ayuda. P16 Error/reintento es una pantalla de recuperación de demostración.

## 5. Inventario y trazabilidad
| ID | Archivo | Propósito | Interacción/contenido |
|---|---|---|---|
| P01 | `index.html` | Presentación | Nombre local, botón comenzar, tarjetas |
| P02 | `02_indice.html` | Organizar módulos | Índice y progreso |
| P03 | `03_sistemas_digitales.html` | Fundamentos | Señales binarias, sistema binario, álgebra de Boole |
| P04 | `04_video_sistemas.html` | Recurso audiovisual | Marcador de video y guía |
| P05 | `05_circuitos_logicos.html` | Práctica lógica | Pregunta AND y devolución |
| P06 | `06_feedback.html` | Feedback | Explicación de AND |
| P07 | `07_memorias.html` | Memorias | RAM, ROM y caché |
| P08 | `08_redes.html` | Introducir redes | LAN/MAN/WAN y referencia a direccionamiento y protocolos |
| P09 | `09_practica_redes.html` | Práctica de redes | Pregunta sobre switch |
| P10 | `10_resultado_practica.html` | Devolución práctica | Explicación del switch |
| P11 | `11_evaluacion_final.html` | Evaluación | Seis preguntas de opción única |
| P12 | `12_resultado_evaluacion.html` | Resultado | Puntaje y acceso condicionado al certificado |
| P13 | `13_certificado.html` | Certificado | Nombre, fecha e impresión |
| P14 | `14_mis_cursos.html` | Catálogo | Cursos de ejemplo |
| P15 | `15_ayuda.html` | Ayuda | Preguntas frecuentes desplegables |
| P16 | `16_error.html` | Recuperación | Reintento y enlace a explicación |

## 6. Estructura de código
- **HTML:** un archivo por pantalla. `data-screen` identifica el tipo de pantalla.
- **CSS:** `css/styles.css` centraliza paleta, diseño adaptable, componentes y estilos de impresión. Variables: `--navy: #07345b`, `--blue: #1479f8`, `--green: #14a783`, `--bg: #f3f7fc`, `--surface: #fff`.
- **JavaScript:** `js/app.js` controla nombre/progreso local, validación de la práctica, navegación de preguntas, cálculo del puntaje y certificado de demostración.

## 7. Trazabilidad del contenido fuente
El PDF incluye dos bloques de contenido visibles: **Direccionamiento y Protocolos** (IP pública/privada, IPv4, IPv6, clases tradicionales de IPv4, MAC e IP, HTTP/HTTPS, TCP, IP, DNS, DHCP, modelos OSI y TCP/IP y un caso de conexión Wi‑Fi) y **Medios de transmisión, dispositivos y topologías** (UTP Cat 5e/Cat 6, coaxial, fibra óptica, Wi‑Fi, Bluetooth, infrarrojo, conexión satelital, switch, router, access point, patch panel, rack y topologías en estrella, bus y anillo). La maqueta incorpora parte de esos conceptos en P08 y preguntas relacionadas en P11; por razones de prototipado no están desarrollados como lecciones separadas. Para la aplicación final se recomienda crear pantallas específicas para esos ejes y validar la organización con el docente. El PDF también contiene preguntas de cierre y recursos multimedia; el video de esta maqueta es solo un marcador.

## 8. Pruebas manuales
- [ ] Abrir P01 y comprobar carga de estilos.
- [ ] Seguir enlaces del índice y navegación lateral.
- [ ] Cambiar el nombre y comprobar la barra superior/certificado.
- [ ] Probar respuestas correctas e incorrectas en P05 y P09.
- [ ] Completar las seis preguntas de P11 y comprobar P12.
- [ ] Imprimir el certificado.
- [ ] Probar en escritorio y ventana estrecha.

## 9. Antes de producción
Validar la secuencia y profundidad curricular; incorporar videos autorizados; ampliar pantallas para direccionamiento, protocolos, medios, dispositivos y topologías; acordar criterios de evaluación; diseñar Back End/API/base de datos en etapa separada; probar accesibilidad, seguridad y compatibilidad.
