![Estado del Proyecto](https://img.shields.io/badge/Estado-Completado-green)
![Chrome DevTools](https://img.shields.io/badge/Chrome-DevTools-blue?logo=google-chrome&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Udemy Course](https://img.shields.io/badge/Curso-Backend%20Developer%20(Udemy)-ec1c24?logo=udemy&logoColor=white)

---

## 📖 Descripción del Proyecto
Este repositorio reúne el conjunto de prácticas y ejercicios desarrollados a lo largo de mi aprendizaje sobre las **Herramientas de Desarrollo del Navegador (DevTools)**, enfocadas en el ecosistema del desarrollo backend. Abarca el uso de paneles clave para la inspección, depuración, optimización de rendimiento y monitoreo de seguridad en aplicaciones web. Todo el contenido forma parte de mi especialización académica orientada al desarrollo backend:

1. **Curso de Backend Developer (Udemy):** Una aproximación práctica a las utilidades que ofrece el navegador para analizar la comunicación de red, el comportamiento de scripts en el cliente, la gestión de memoria y el almacenamiento de datos.
2. **Prácticas en Entorno Web (`be_devtools`):** Un proyecto base (`index.html`) consistente en una calculadora interactiva diseñada específicamente para practicar la manipulación de variables, la captura de errores en consola y el flujo de depuración con puntos de interrupción.

---

## 🎯 Objetivo
Consolidar el dominio técnico en el uso de las herramientas de diagnóstico del navegador bajo estándares profesionales de desarrollo backend, logrando:

- Analizar la estructura del DOM y estilos aplicados a elementos interactivos desde el panel **Elementos**.
- Monitorear registros, advertencias y errores en tiempo de ejecución utilizando la **Consola**, además de interactuar dinámicamente con variables de JavaScript.
- Depurar el código fuente de scripts en el cliente estableciendo puntos de interrupción (**Breakpoints**) y analizando la pila de ejecución en el panel **Fuentes**.
- Auditar el rendimiento de carga y ejecución de aplicaciones web con los paneles **Rendimiento** e **Lighthouse**.
- Inspeccionar el consumo de recursos de memoria (Heap) y diagnosticar fugas en el panel **Memoria**.
- Administrar y validar información persistida como cookies, LocalStorage y SessionStorage desde el panel **Aplicación**.
- Comprobar la seguridad de las conexiones y el cifrado de datos mediante el panel **Seguridad**.
- Registrar y reproducir flujos automatizados de navegación con la herramienta **Grabadora**.

---

## 🛠️ Requerimientos Técnicos / Temas Cubiertos
Este proyecto cumple con los estándares exigidos para el aprendizaje integral de las herramientas del desarrollador (DevTools) y su uso en la depuración de aplicaciones:

### 1. Panel de Elementos (Elements)
- ✅ **Inspección de Estructura DOM:** Inspección visual de la jerarquía de etiquetas, campos de entrada (`<input type="number">`) y botones de acción en [index.html](./ARCHIVOS/index.html).
- ✅ **Edición en Tiempo Real:** Modificación dinámica del DOM y atributos desde el navegador para probar cambios de interfaz de forma inmediata.

### 2. Panel de Consola (Console)
- ✅ **Registro de Mensajes (Log):** Envío de trazas y estados internos del programa mediante `console.log` para seguir las variables de entrada y el resultado en [index.html](./ARCHIVOS/index.html).
- ✅ **Manejo de Errores (Error):** Captura e impresión de errores de validación con `console.error` al introducir valores no numéricos en [index.html](./ARCHIVOS/index.html).
- ✅ **Inspección de Estructuras de Datos:** Visualización y lectura de arreglos de datos complejos (e.g., `let numeros = [...]`) directamente en la terminal interactiva de la consola.

### 3. Panel de Fuentes (Sources)
- ✅ **Depuración de Scripts (Debugging):** Establecimiento de breakpoints en la función `sumar()` para detener la ejecución y analizar los valores asignados en tiempo real.
- ✅ **Pila de Ejecución (Call Stack):** Seguimiento del flujo de llamadas y el alcance de las variables locales/globales durante la depuración.

### 4. Panel de Rendimiento (Performance)
- ✅ **Grabación de Perfil de Rendimiento:** Registro de la actividad del navegador al realizar operaciones para detectar cuellos de botella e hilos bloqueados.

### 5. Panel de Memoria (Memory)
- ✅ **Instantáneas de Heap (Heap Snapshots):** Captura del estado de la memoria para rastrear variables persistentes y asegurar la correcta recolección de basura (Garbage Collection).

### 6. Panel de Aplicación (Application)
- ✅ **Inspección del Almacenamiento:** Visualización de la persistencia de datos localmente usando cookies de sesión, LocalStorage o SessionStorage.

### 7. Panel de Seguridad (Security)
- ✅ **Auditoría de Orígenes y SSL:** Verificación de la seguridad de la conexión, estado de certificados HTTPS y detección de contenido mixto (Mixed Content).

### 8. Panel de Lighthouse
- ✅ **Auditoría de Calidad Web:** Generación de informes automáticos puntuando el rendimiento, la accesibilidad, las mejores prácticas y el SEO de la página web.

### 9. Panel de Grabadora (Recorder)
- ✅ **Grabación de Flujos de Usuario:** Registro de una sesión interactiva (introducción de datos en la calculadora y clic de suma) para exportarla o volver a ejecutarla de manera automática.

---

## 📂 Estructura del Proyecto
```
be_devtools/
│
├── ARCHIVOS/
│   └── index.html      # Página web de calculadora utilizada para prácticas de depuración
│
└── README.md           # Documentación del repositorio
```

---

## 🚀 Instrucciones de Ejecución y Validación
Para interactuar con la aplicación de prueba y abrir las herramientas de desarrollo en tu navegador:

### 1. Clonar el repositorio
```bash
git clone https://github.com/jltamayocabello-droid/be_devtools.git
cd be_devtools
```

### 2. Levantar un Servidor Local
Para evitar problemas de restricciones de seguridad (CORS) del navegador y simular un entorno real de producción, sirve el proyecto localmente. Puedes usar:
- **Python (Recomendado):**
  ```bash
  python -m http.server 8000
  ```
- **Live Server (Extensión de VS Code):** Clic derecho sobre `ARCHIVOS/index.html` y seleccionar *Open with Live Server*.

### 3. Abrir Chrome DevTools
Una vez que accedas a la aplicación en `http://localhost:8000/ARCHIVOS/index.html` (o el puerto que te indique tu servidor local):
1. Presiona `F12` o `Ctrl + Shift + I` (en Windows/Linux) / `Cmd + Option + I` (en macOS).
2. Dirígete a la pestaña **Consola** para ver las entradas y salidas de la calculadora al realizar operaciones.
3. Abre la pestaña **Fuentes (Sources)** y coloca un punto de interrupción (Breakpoint) en la línea `21` del script de `index.html` para depurar el proceso de la función `sumar()` paso a paso.

---

## 📱 Áreas Técnicas Destacadas
| Área Técnica | Conceptos Clave | Descripción |
| :--- | :--- | :--- |
| 🎨 **Elementos** | Inspector DOM, Edición de CSS en vivo, Box Model | Permite visualizar y modificar temporalmente la estructura HTML y las reglas de diseño CSS del documento web. |
| 💬 **Consola** | console.log/error/warn, Entorno interactivo | Terminal interactiva para depuración, visualización de datos de scripts y evaluación de expresiones JavaScript en vivo. |
| 🔍 **Fuentes (Sources)** | Breakpoints, Call Stack, Scope, Callbacks | Panel para navegar por el código fuente, pausar la ejecución en líneas clave y auditar el estado de memoria interna. |
| ⚡ **Rendimiento** | CPU throttling, FPS, Perfilado de carga | Herramienta de perfilado que ayuda a detectar ralentizaciones, renderizados costosos y bloqueos de la interfaz. |
| 💾 **Memoria** | Heap snapshot, Allocation instrumentation | Permite analizar la distribución de memoria de JavaScript, identificar objetos retenidos y solucionar fugas de memoria. |
| 📂 **Aplicación** | Local/Session Storage, Cookies, Cache Storage | Gestión del almacenamiento del lado del cliente, cookies de sesión y recursos locales cacheados por Service Workers. |
| 🛡️ **Seguridad** | Certificados SSL, TLS, Orígenes mixtos | Ofrece un diagnóstico rápido de la seguridad del sitio web, asegurando el uso correcto de certificados seguros HTTPS. |
| 📊 **Lighthouse** | Métricas de Core Web Vitals, Auditoría SEO | Genera auditorías automáticas que miden la velocidad, accesibilidad, calidad de código y optimización para buscadores. |
| 🔴 **Grabadora** | Registro de flujo, Replay de acciones, Automatización | Permite grabar interacciones de usuario recurrentes para medir el rendimiento de la interacción o automatizar pruebas de regresión. |

---

## ✒️ Autor
**Jorge Tamayo Cabello**  
*Desarrollador Front-End*

---

## 📄 Licencia
Este repositorio es de carácter estrictamente académico y educativo. Todo el contenido es libre de ser consultado con fines de aprendizaje y referencia técnica.

---

## 🙏 Agradecimientos
- A **Udemy** por la excelente formación en desarrollo de backend mediante el curso de Backend Developer.
- A la **comunidad de desarrollo de software libre** por la creación y mantenimiento de herramientas de desarrollo web de primer nivel.
