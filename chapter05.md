# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

**Project Management**

Para la administración del proyecto, se utilizaron varias herramientas para la comunicación, la planificación y el control de versiones.

| Plataforma                   | Descripción                                                                                                                                                                                             | Enlace               |
| :--------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :------------------- |
| Trello                       | Esta plataforma de gestión de proyectos ofrece el seguimiento detallado del progreso de cada tarea, además de permitir la designación de responsables para cada actividad dentro del equipo de trabajo. | https://trello.com   |
| Herramientas de Comunicación | La comunicación interna del equipo se gestionó a través de Discord y WhatsApp para reuniones y mensajes rápidos, respectivamente.                                                                       | https://discord.com/ |
| GitHub                       | Se creó una organización para centralizar el código fuente y su versionado, lo que permitió un control de versiones eficiente y una gestión ordenada.                                                   | https://github.com   |

**Requirement Management**

En la fase inicial, se emplearon herramientas para la recolección y organización de los requisitos del proyecto, lo que aseguró una base sólida para el desarrollo.

| Plataforma | Descripción                                                                                                                                                                                                     | Enlace                 |
| :--------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------- |
| UXPressia  | Fue la herramienta principal para el diseño. Permitió al equipo crear y validar propuestas de diseño con wireframes, mockups y prototipos interactivos, lo que aseguró un producto final efectivo y atractivo.  | https://uxpressia.com/ |
| Miro       | Esta herramienta se usó para visualizar y desarrollar los escenarios "As-Is" (estado actual) y "To-Be" (estado futuro), lo que ayudó a planificar la evolución del proyecto.                                    | https://miro.com/es/   |

**Product UX/UI Desing**

Para el diseño de la experiencia y la interfaz de usuario, se usó una plataforma colaborativa que simplificó el flujo de trabajo.

| Plataforma | Descripción        																																															  |						  |
| :--------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------- |
| Figma      | Fue la herramienta principal para el diseño. Permitió al equipo crear y validar propuestas de diseño con wireframes, mockups y prototipos interactivos, lo que aseguró un producto final efectivo y atractivo. | https://www.figma.com |

**Software Development**

El desarrollo se realizó utilizando un conjunto de lenguajes y entornos de programación que garantizan la estructura, el estilo y la interactividad del producto.

| Plataforma          | Descripción                                                                                                                                    | Link                                       |
|---------------------| :--------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------- |
| HTML                | Sirve para definir la estructura y el contenido de una página web.                                                                             | https://www.w3schools.com/html/default.asp |
| CSS                 | Se encarga de la presentación visual y el estilo de la página web.                                                                             | https://www.w3schools.com/css/default.asp  |
| JS                  | Añade interactividad y dinamismo a la página web.                                                                                              | https://www.w3schools.com/js/default.asp   |
| Visual Studio Code  | Entorno de desarrollo que facilita la escritura, edición, depuración y gestión de código para una amplia gama de lenguajes y proyectos.        | https://code.visualstudio.com              |
| JetBrains ToolBox   | Aplicación de gestión que contiene IDEs como IntelliJ IDEA, WebStorm y Rider (cada miembro del equipo trabajó en alguna de estas herramientas) | https://www.jetbrains.com/toolbox-app/     |

**Software Documentation**

La documentación y la publicación del proyecto se manejaron con herramientas que optimizan la colaboración y el despliegue final.

| Plataforma | Descripción                                             | Link                                                              |
|------------|---------------------------------------------------------|-------------------------------------------------------------------|
| GitHub     | Gestión de la documentación en función a repositorios y organizaciones | `https://github.com`          |
| Markdown   | Formato base para la presentación y documentación del proyecto | `https://markdown.es/  `                   |

Se utilizó la estrategia GitHub Flow para la colaboración y el control de versiones, usando ramas específicas para cada funcionalidad. Esto mantuvo el proyecto organizado. También sirvió como repositorio central para toda la documentación.
Para el despliegue de la Landing Page se utilizó GitHub Pages, una herramienta perfecta para publicar sitios web estáticos.

<br>

### 5.1.2. Source Code Management

Definir convenciones de nomenclatura para ramas en Git es crucial para mantener un flujo de trabajo organizado y mejorar la colaboración. Al seguir modelos como Git Flow, se puede crear una estructura clara que hace más predecible la gestión del proyecto.

---

### **Beneficios de la Nomenclatura Predictiva**

Un esquema de nombres consistente ofrece múltiples ventajas:

- **Automatización de procesos (CI/CD)**: Facilita la configuración de flujos de trabajo de integración y despliegue continuos.
- **Identificación de propósito**: Permite a los desarrolladores identificar rápidamente el objetivo y el alcance de cada rama.

---

### **Estrategia de Ramificación (Git Flow)**

En nuestro proyecto, aplicamos un modelo simplificado de Git Flow con las siguientes ramas principales:

* **Rama `main`**: Contiene el **código de producción**, incluyendo archivos CSS, imágenes, JavaScript y el `index.html`. Esta rama se mantiene siempre en un estado **estable y listo para ser desplegado**.
* **Rama `gh-pages`**: Esta rama se usa para **desplegar el proyecto en GitHub Pages**, lo que permite una visualización en tiempo real del sitio web.

Además de estas, gestionamos el progreso del desarrollo en un repositorio separado, donde organizamos las tareas en epics y usamos archivos `.feature` para definir los **criterios de aceptación** de cada funcionalidad.

---

### **Flujo de Trabajo y Herramientas**

Elegimos **GitHub** como nuestra plataforma de colaboración principal. Esto nos ayuda a **dar seguimiento al progreso** del equipo, **gestionar los cambios** y **visualizar las actualizaciones** del proyecto. Una de las ventajas es que las actualizaciones en el código se reflejan automáticamente en la rama `gh-pages`, lo que permite a los interesados ver los avances en tiempo real.

---

### **Convenciones de Nomenclatura**

A continuación, se detallan las convenciones de nomenclatura para diferentes tipos de ramas que usamos en nuestro proyecto:

1. **Master branch (Rama principal):** Es la rama principal del proyecto, donde se almacena el código estable y listo para producción. Solo se integrarán cambios que hayan sido probados y validados previamente en las ramas de desarrollo y funcionalidad.

2. **Develop Branch (Rama de Desarrollo):** Esta rama actúa como un espacio de integración para el trabajo en equipo, permitiendo pruebas y ajustes de las nuevas funcionalidades antes de fusionarlas con la rama principal. Garantiza que el código sea funcional y estable.

3. **Feature branch (Ramas de funcionalidad):** Cada nueva funcionalidad o tarea específica se desarrollará en su propia rama. Una vez completada y probada, se integrará en la rama de desarrollo. Las ramas de funcionalidad seguirán un esquema de nombres descriptivos.

✔ **Ramas de característica (`feature`)**
- Prefijo: `feature/`
- Formato: `feature/nombre-corto-descriptivo`
- Ejemplos: `feature/login-ui`, `feature/pdf-export`, `feature/api-integration-usuarios`

✔ **Ramas de lanzamiento (`release`)**
- Prefijo: `release/`
- Formato: `release/x.y.z (donde x, y, z representan el número mayor, menor y de parche)`
- Ejemplos: `release/1.0.0`, `release/2.1.0`

✔ **Ramas de corrección urgente (`hotfix`)**
- Prefijo: `hotfix/`
- Formato: `hotfix/x.y.z-nombre-corto`
- Ejemplos: `hotfix/1.0.1-fix-login-error`, `hotfix/2.3.2-bug-carrito`

---

**Repositorio de Github:**
- Enlace para acceder a la organizacion en Github: `https://github.com/1ASI0730-2520-7452-G1-FrostShield`
- Enlace para acceder al repositorio de la Landing Page: `https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page`
- Enlace para acceder al repositorio del Informe: `https://github.com/1ASI0730-2520-7452-G1-FrostShield/Report`

---

### 5.1.3. Source Code Style Guide & Conventions

Para asegurar la calidad, mantenibilidad y coherencia de nuestra solución, hemos definido un conjunto de convenciones y buenas prácticas. Dado que el proyecto inicial es una landing page, nos centramos en los estándares para HTML, CSS y JavaScript, los pilares de nuestro desarrollo.

**Convenciones de Nomenclatura**

Para mantener la consistencia y la claridad, seguimos las siguientes convenciones:

**Variables y Funciones en JavaScript:** Se utiliza la convención camelCase (ej. myVariable, initializeVideos()). Los nombres deben ser descriptivos.

**Constantes en JavaScript:** Se utilizan letras mayúsculas y guiones bajos para separar las palabras (SNAKE_CASE) para valores que no cambian (ej. VIDEO_CONFIG).

**Archivos:** Los nombres de archivos se escriben en minúsculas y se separan con guiones (ej. index.html, style.css, languages.js).

**HTML**
La estructura de nuestro documento HTML se basa en la semántica web, utilizando etiquetas con un significado claro para el navegador y los desarrolladores. Esto no solo mejora la accesibilidad y el SEO, sino que también facilita la comprensión del código. A continuación, se detallan las etiquetas utilizadas:

* `<!DOCTYPE html>` - Define el tipo de documento como HTML5.
* `<html>` - Raíz del documento HTML.
* `<head>` - Encabezado del documento, donde se incluyen metadatos.
* `<meta>` - Define metadatos sobre el documento (charset y viewport).
* `<title>` - Título del documento.
* `<link>` - Para enlaces de icono, hoja de estilos CSS y fuente externa.
* `<body>` - Cuerpo del documento, donde se encuentra el contenido visible.
* `<header>` - Encabezado de la página.
* `<div>` - Contenedor para el logo y otros elementos.
* `<img>` - Imagen del logo.
* `<nav>` - Contenedor para la navegación.
* `<ul>` - Lista no ordenada de enlaces de navegación.
* `<li>` - Elemento de lista para cada enlace de navegación.
* `<a>` - Enlaces de navegación.
* `<button>` - Botón para el modo de deuteranopia.
* `<section>` - Define secciones de contenido principal:
    * Sección principal: `<h1>`, `<p>`
    * Por Qué Interactiva: `<h2>`, `<span>`, `<div>`, `<h3>`, `<p>`
    * Valor Propuesto: `<h3>`, `<p>`, `<img>`
    * Presentamos a...: `<h2>`, `<h4>`, `<p>`, `<img>`
    * Servicios: `<h2>`, `<div>`, `<h4>`, `<p>`
    * Testimonios: `<h2>`, `<p>`, `<img>`
    * Cómo empezar: `<h2>`, `<h5>`, `<strong>`, `<p>`
    * Descargar: `<h2>`, `<h3>`, `<span>`, `<a>`, `<img>`
* `<footer>` - Pie de página.
* `<small>` - Texto de derechos reservados.
* `<script>` - Script JavaScript para funcionalidades.

**CSS**

Nuestra guía de estilo para CSS se centra en la claridad y la consistencia. Se han definido propiedades clave para el diseño visual, asegurando que todos los elementos se vean y se comporten de manera uniforme.

* `width:` Representa el ancho de un elemento.
* `height:` Representa el alto de un elemento.
* `padding:` Representa el espacio con relleno entre el borde y el contenido.
* `font-family:` Representa el tipo de letra.
* `font-size:` Representa el tamaño de letra.
* `font-weight:` Representa el grueso o el peso de la letra.
* `font-style:` Representa el estilo de letra.
* `Text-align:` Representa la alineación del texto.
* `color:` Otorga color al elemento.
* `Background-color:` Otorga color del fondo del elemento.

### 5.1.4. Software Deployment Configuration

Para poder publicar nuestra landing page, seguimos una serie de pasos específicos utilizando GitHub Pages, que permite alojar sitios web estáticos directamente desde un repositorio.

El despliegue en GitHub Pages requiere que los archivos estén organizados de una manera particular para que la plataforma los reconozca y los sirva correctamente.

**1. Organización del Repositorio:**

- Los archivos principales deben estar en la carpeta raíz del repositorio.

- Los nombres de los archivos deben seguir la convención establecida: index.html para la página principal, styles.css para los estilos, y script.js para los scripts.

- Las imágenes se guardan en una carpeta llamada assets/images.

- El archivo languages.js se utiliza para gestionar las traducciones.

**2. Subida de Archivos:**

- Una vez que los archivos están correctamente organizados, se suben al repositorio a través de un commit.

**3. Configuración en GitHub Pages:**

- Se navega a Settings > Pages dentro del repositorio.

- Se selecciona la rama main como la fuente de despliegue.

- Se configura la carpeta raíz (/root) para el origen de la página.

**4. Despliegue Automático:**

- GitHub Pages inicia un proceso de verificación y despliegue automático.

- Al finalizar, se genera una URL pública para acceder a la landing page.

Además, nuestra solución incluye un archivo llamado languages.js, que contiene las traducciones en español e inglés. Este archivo es cargado por el script principal main.js para permitir que los usuarios cambien el idioma de la página de forma dinámica.

**Github Pages:**

URL de la Landing Page desplegada en Github Pages: 

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

<table border="1">
<tr>
    <th colspan="5">Sprint 1</th>
    <th colspan="9">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-10-6</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">1:00 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Presencial (Universidad Peruana de Ciencias Aplicadas sede San Miguel)</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Kenyi Ramirez</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alejandro Galindo, Julio Guillen, Ivan La Madrid, Pedro Nanfuñay</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Review Summary</td>
    <td colspan="8"></td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Retrospective Summary</td>
    <td colspan="8">Durante este sprint, todos los integrantes compartieron sus ideas respecto a la plataforma web, tales como el rubro, los segmentos objetivos, beneficios, funcionalidades. Tuvimos tareas bien organizadas y realizadas, que se puede verificar en los avances del informe y del Landing Page</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Goal</td>
       <td colspan="8">Nuestro enfoque está en implementar la landing page de nuestra plataforma, asegurando su adaptabilidad a diferentes dispositivos, coherencia visual y funcionalidad multilingüe. Creemos que esto ofrece una experiencia de navegación más clara, atractiva y accesible a los usuarios potenciales de nuestra solución. Esto se confirmará cuando los usuarios puedan cambiar el idioma fácilmente desde la interfaz, navegar la página sin errores visuales desde cualquier dispositivo, y se valide que imágenes y textos estén correctamente integrados y espaciados. </td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Velocity</td>
    <td colspan="8">15</td>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">10</td>
</tr>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators

##### 5.2.1.2. Aspect Leaders and Collaborators

Durante este primer Sprint, el equipo se enfocó principalmente en el desarrollo, la mejora estructural y visual de la Landing Page, asegurando su visualización en distintos dispositivos (diseño responsive), la integración armoniosa de imágenes y textos, y la implementación de un cambio de idioma dinámico mediante un botón.
Con el fin de organizar de manera más eficiente el trabajo colaborativo, se ha elaborado la matriz de Liderazgo y Colaboración (LACX). Esta matriz asigna responsabilidades específicas a cada miembro del equipo en relación con los aspectos clave del Sprint.

<table border="1">
  <tr>
    <td colspan="2"><strong>Team Member (Last Name, First Name)</strong></td>
    <td><strong>GitHub Username</strong></td>
    <td><strong>Diseño visual y maquetación web (Landing Page)<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Responsividad y pruebas en distintos dispositivos<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Implementación técnica del cambio de idioma (Multilenguaje funcional)<br>Leader (L) / Collaborator (C)</strong></td>
  </tr>
  <tr>
    <td colspan="2">Ramírez Cabrera, Kenyi Efrain</td>
    <td>Kenyi15upc</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2"> Galindo Montero, Alejandro Manuel </td>
    <td>AlejandroG12970</td>
    <td>C</td>
    <td>L</td>
    <td>L</td>
  </tr>
  <tr>
    <td colspan="2"> Guillen Galindo, Julio Adolfo </td>
    <td>julio645</td>
    <td>C</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2">La Madrid Lozano, Ivan Jeanpierre</td>
    <td>ivanlamadrid</td>
    <td>C</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2">Nanfuñay Liza, Pedro Jesus</td>
    <td>PedroJ18</td>
    <td>C</td>
    <td>C</td>
    <td>C</td>
  </tr>
</table>

#### 5.2.1.3. Sprint Backlog 1

El objetivo principal de este Sprint es elaborar la Landing Page de nuestra plataforma. Para ello, dividimos el desarrollo de esta según las User Stories pertenecientes a la Epic enfocada en Landing Page. La plataforma elegida para ser la herramienta de control de tareas fue Trello, el cuál se presenta una captura de pantalla de nuestro tablero y su enlace público.

Enlace: https://trello.com/b/sUPp1a6b/sprints

![Sprint1-Trello.png](assets/chapter05/Sprint1-Trello.png)
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Sprint Backlog 1.
  </figcaption>

---
<table border="1">
<tr>
    <th colspan="3">Sprint #</th>
    <th colspan="10">Sprint 1</th>
</tr>
<tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
</tr>
<tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1">Estimation (Hours)</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status (To do/ In-Process/ To-Review/ Done)</td>
</tr>
<tr>
    <td colspan="1">US-23</td>
    <td colspan="2">Visualizar propuesta de valor principal</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear la sección 'Hero'</td>
    <td colspan="3">Añadir la sección donde se muestra nuestra propuesta de valor principal</td>
    <td colspan="1">1</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-24</td>
    <td colspan="2">Explorar soluciones específicas para mi rubro</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear la sección 'Beneficios'</td>
    <td colspan="3">Añadir la sección donde se visualizan las soluciones específicas al segmento Dueño de negocio </td>
    <td colspan="1">1</td>
    <td colspan="2">Ivan La Madrid</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-24</td>
    <td colspan="2">Explorar soluciones específicas para mi rubro</td>
    <td colspan="1">UT-02</td>
    <td colspan="2">Crear la sección 'Beneficios'</td>
    <td colspan="3">Añadir la sección donde se visualizan las soluciones específicas al segmento Proveedor de Servicios </td>
    <td colspan="1">1</td>
    <td colspan="2">Ivan La Madrid</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-28</td>
    <td colspan="2">Acceder a la plataforma web (Call to Action)</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear el elemento Call to Action</td>
    <td colspan="3">Añadir el elemento que redirecciona a la página de la aplicación web</td>
    <td colspan="1">0.5</td>
    <td colspan="2">Kenyi Ramírez</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-27</td>
    <td colspan="2">Contactar con el equipo de ventas</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear la sección "Contacto"</td>
    <td colspan="3">Agregar un formulario para contactar con los responsables de la plataforma</td>
    <td colspan="1">1</td>
    <td colspan="2">Julio Guillen</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-26</td>
    <td colspan="2">Conocer misión y visión</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear la sección 'Nosotros'</td>
    <td colspan="3">Añadir la sección donde se visualiza la misión y visión de nuestra startup</td>
    <td colspan="1">1</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-00</td>
    <td colspan="2">-</td>
    <td colspan="1">UT-01/td>
    <td colspan="2">Implementar cambio de idioma</td>
    <td colspan="3">Implementar la funcionalidad de cambio de idioma en la landing page</td>
    <td colspan="1">1</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-00</td>
    <td colspan="2">-</td>
    <td colspan="1">UT-02/td>
    <td colspan="2">Añadir la sección de testimonios</td>
    <td colspan="3">Crear la sección "Testimonios" y asignar los comentarios más favorables respecto a nuestra plataforma</td>
    <td colspan="1">1</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>

</table>

##### 5.2.1.4. Development Evidence for Sprint Review

En este primer Sprint hemos realizado la implementación de nuestra Landing Page, donde todo el equipo ha aportado en varias tareas. En la siguiente tabla se muestran los commits realizados.

<table>
    <tr>
        <th colspan="2">Repository</th>
        <th colspan="2">Branch</th>
        <th colspan="2">Commit Id</th>
        <th colspan="2">Commit Message</th>
        <th colspan="2">Commit Message Body</th>
        <th colspan="2">Committed on (Date)</th>
    </tr>
        <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Merge pull request #2 from 1ASI0730-2520-7452-G1-FrostShield/develop</td>
        <td colspan="2">Merge pull request #2 from 1ASI0730-2520-7452-G1-FrostShield/develop</td>
        <td colspan="2">21/09/2025</td>
    </tr>
        <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: add images</td>
        <td colspan="2">add images</td>
        <td colspan="2">21/09/2025</td>
    </tr>
        <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: add testimonials section</td>
        <td colspan="2">add testimonials section</td>
        <td colspan="2">21/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Update script.js</td>
        <td colspan="2">Update script.js</td>
        <td colspan="2">21/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Update style.css</td>
        <td colspan="2">Update style.css</td>
        <td colspan="2">21/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Update index.html</td>
        <td colspan="2">Update index.html</td>
        <td colspan="2">21/09/2025</td>
    </tr>
   <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: update script to about us section</td>
        <td colspan="2">update script to about us section</td>
        <td colspan="2">21/09/2025</td>
    </tr>
   <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Merge pull request #1 from 1ASI0730-2520-7452-G1-FrostShield/feature/benefits</td>
        <td colspan="2">Merge pull request #1 from 1ASI0730-2520-7452-G1-FrostShield/feature/benefits</td>
        <td colspan="2">21/09/2025</td>
    </tr>
   <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Merge branch 'develop' into feature/benefits</td>
        <td colspan="2">Merge branch 'develop' into feature/benefits</td>
        <td colspan="2">21/09/2025</td>
    </tr>
   <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">update index.html</td>
        <td colspan="2">update index.html</td>
        <td colspan="2">20/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(landing-page): add styles for benefits section</td>
        <td colspan="2">add styles for benefits section</td>
        <td colspan="2">20/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(landing-page): add benefits section</td>
        <td colspan="2">add benefits section</td>
        <td colspan="2">20/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Add about us section in style.css</td>
        <td colspan="2">Add about us section in style.css</td>
        <td colspan="2">20/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Add about us section in HTML</td>
        <td colspan="2">Add about us section in HTML</td>
        <td colspan="2">20/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">style: add color palette and responsive layout for landing page</td>
        <td colspan="2">add color palette and responsive layout for landing page</td>
        <td colspan="2">19/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: add language switching functionality and translations for ES/EN</td>
        <td colspan="2">add language switching functionality and translations for ES/EN</td>
        <td colspan="2">19/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: add JavaScript for mobile menu toggle, smooth scroll, and CTA button functionality</td>
        <td colspan="2">add JavaScript for mobile menu toggle, smooth scroll, and CTA button functionality</td>
        <td colspan="2">19/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: added Header, Hero and Footer Section Structure</td>
        <td colspan="2">added Header, Hero and Footer Section Structure</td>
        <td colspan="2">19/09/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat: initialize basic landing page structure with HTML</td>
        <td colspan="2">initialize basic landing page structure with HTML</td>
        <td colspan="2">19/09/2025</td>
    </tr>
</table>

#### 5.2.1.5. Execution Evidence for Sprint Review

**Inicio**
Muestra el logo de la marca, una navegación clara y un botón de "Registrarse" en un color llamativo para guiar al usuario.
Presenta la propuesta de valor principal con una imagen atractiva y un texto impactante, capturando la atención del visitante de inmediato
![LPEvidenceInicio.png](assets/chapter05/LPEvidenceInicio.png)
---

**Beneficios**
Detalla las principales ventajas que los usuarios obtienen al usar el producto, mostrando cómo resuelve sus problemas de manera efectiva.
![LPEvidenceBeneficios.png](assets/chapter05/LPEvidenceBeneficios.png)
---

**Sobre Nosotros**
Explica la misión y visión de la empresa, compartiendo los valores y la historia para generar confianza.
![LPEvidenceSobreNosotros.png](assets/chapter05/LPEvidenceSobreNosotros.png)
---

**Testimonios**
Muestra opiniones de clientes satisfechos, actuando como prueba social para validar la calidad del producto o servicio.
![LPEvidenceTestimonios.png](assets/chapter05/LPEvidenceTestimonios.png)
---

**Contacto**
Ofrece un medio para que los usuarios se comuniquen, ya sea para pedir más información o para agendar una demostración.
![LPEvidenceContacto.png](assets/chapter05/LPEvidenceContacto.png)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

A continuación, se presenta las  secciones principales de la Landing Page desplegada en GitHub Pages:

**Inicio**
![LPEvidenceInicio.png](assets/chapter05/LPEvidenceInicio.png)
---
**Beneficios**
![LPEvidenceBeneficios.png](assets/chapter05/LPEvidenceBeneficios.png)
---
**Sobre Nosotros**
![LPEvidenceSobreNosotros.png](assets/chapter05/LPEvidenceSobreNosotros.png)
---
**Testimonios**
![LPEvidenceTestimonios.png](assets/chapter05/LPEvidenceTestimonios.png)
---
**Contacto**
![LPEvidenceContacto.png](assets/chapter05/LPEvidenceContacto.png)
---

URL del Landing Page desplegado: https://1asi0730-2520-7452-g1-frostshield.github.io/IceTrack---Landing-Page/

#### 5.2.1.8. Team Collaboration Insights during Sprint

![Insights-LP.png](assets/chapter05/Insights-LP.png)
---

![Contributors.png](assets/chapter05/Contributors.png)

### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2

<table>
<tr>
    <th colspan="5">Sprint 2</th>
    <th colspan="9">Sprint 2</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-09-27</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">15:00 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Kenyi Ramirez</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alejandro Galindo, Julio Guillen, Ivan Lozano, Pedro Nanfuñay, Pedro Jesús</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Review Summary</td>
    <td colspan="8">En este sprint, nos enfocamos en desarrollar el front-end y en realizar la implementación inicial de la plataforma IceTrack. Completamos las funciones principales de la página, ofreciendo a los usuarios una primera experiencia de navegación y exploración del servicio de refrigeración. El equipo cumplió con los objetivos de entrega dentro del plazo previsto, estableciendo además los cimientos de la interfaz gráfica para futuras iteraciones.
</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Retrospective Summary</td>
    <td colspan="8">Durante el sprint, a pesar de estar enfocado en el desarrollo técnico, permitió identificar oportunidades para mejorar nuestra dinámica de trabajo en equipo. En la retrospectiva, se destacó la necesidad de ajustar la duración de las reuniones diarias, redistribuir las tareas de acuerdo con las especialidades del equipo e incorporar una planificación individual con hitos verificables. Estas medidas tienen como objetivo incrementar la eficiencia en las próximas iteraciones.
 </td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Goal</td>
       <td colspan="8">Nuestro enfoque de desarrollo se centra en la creación e implementación de la interfaz front-end de IceTrack, con el objetivo de proporcionar una experiencia de navegación fluida e intuitiva, mostrar las principales funcionalidades de la plataforma y disponer de una página de inicio funcional que comunique de manera efectiva el valor diferencial del servicio.</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Velocity</td>
    <td colspan="8">35</td>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">30</td>
</tr>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators

Durante este segundo sprint, el equipo se enfocó principalmente en el desarrollo, mejora estructural y visual de las aplicaciones del Frontend, asegurando su correcto funcionamiento en distintos dispositivos (diseño responsive), la integración coherente de componentes visuales e interactivos, así como la implementación de funcionalidades dinámicas que mejoran la experiencia del usuario.

Con el objetivo de optimizar la organización y la colaboración del equipo, se elaboró la matriz de Liderazgo y Colaboración (LACX), la cual asigna responsabilidades y roles específicos a cada miembro del equipo en relación con los aspectos clave abordados durante el Sprint.

<table border="1">
  <tr>
    <td colspan="2"><strong>Team Member (Last Name, First Name)</strong></td>
    <td><strong>GitHub Username</strong></td>
    <td><strong>Implementacion de la gestión de equipos de refrigeracion (Frontend Applications)<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Responsividad y pruebas en distintos dispositivos<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Despliegue de la aplicación web<br>Leader (L) / Collaborator (C)</strong></td>
  </tr>
  <tr>
    <td colspan="2">Ramírez Cabrera, Kenyi Efrain</td>
    <td>Kenyi15upc</td>
    <td>L</td>
    <td>C</td>
    <td>L</td>
  </tr>
  <tr>
    <td colspan="2"> Galindo Montero, Alejandro Manuel </td>
    <td>AlejandroG12970</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2"> Guillen Galindo, Julio Adolfo </td>
    <td>julio645</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2">La Madrid Lozano, Ivan Jeanpierre</td>
    <td>ivanlamadrid</td>
    <td>C</td>
    <td>C</td>
    <td>L</td>
  </tr>
  <tr>
    <td colspan="2">Nanfuñay Liza, Pedro Jesus</td>
    <td>PedroJ18</td>
    <td>C</td>
    <td>L</td>
    <td>L</td>
  </tr>
</table>

#### 5.2.2.3. Sprint Backlog 2
El objetivo principal de este Sprint es elaborar el Frontend de nuestra plataforma. Para ello, dividimos el desarrollo de esta según las User Stories pertenecientes a la Epic enfocada en la aplicacion web. La plataforma elegida para ser la herramienta de control de tareas fue Trello, el cuál se presenta una captura de pantalla de nuestro tablero y su enlace público.

Enlace: https://trello.com/b/mLKlTDIY/frontend

![Sprint1-Trello.png](assets/chapter05/Sprint2-Trello.png)
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Sprint Backlog 2.
  </figcaption>

<table border="1">
<tr>
    <th colspan="3">Sprint #</th>
    <th colspan="10">Sprint 2</th>
</tr>
<tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
</tr>
<tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1">Estimation (Hours)</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status (To do/ In-Process/ To-Review/ Done)</td>
</tr>

<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Registro de usuario</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear formulario de registro</td>
    <td colspan="3">Implementar formulario con campos: nombre, correo, contraseña y confirmación.</td>
    <td colspan="1">4</td>
    <td colspan="2">Kenyi Ramírez</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Registro de usuario</td>
    <td colspan="1">UT-02</td>
    <td colspan="2">Validar formato de correo y contraseñas</td>
    <td colspan="3">Añadir validaciones visuales en tiempo real (email válido, contraseña ≥ 8 caracteres).</td>
    <td colspan="1">3</td>
    <td colspan="2">Kenyi Ramírez</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Registro de usuario</td>
    <td colspan="1">UT-03</td>
    <td colspan="2">Integrar API de registro</td>
    <td colspan="3">Enlazar el formulario con el endpoint de backend `/api/v1/users`.</td>
    <td colspan="1">3</td>
    <td colspan="2">Julio Guillén</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-02</td>
    <td colspan="2">Inicio de sesión</td>
    <td colspan="1">UT-04</td>
    <td colspan="2">Diseñar pantalla de login</td>
    <td colspan="3">Crear vista con campos de email y contraseña, y enlace a “Olvidé mi contraseña”.</td>
    <td colspan="1">3</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-02</td>
    <td colspan="2">Inicio de sesión</td>
    <td colspan="1">UT-05</td>
    <td colspan="2">Integrar API de login</td>
    <td colspan="3">Implementar autenticación usando endpoint `/api/v1/auth` y manejo de token JWT.</td>
    <td colspan="1">4</td>
    <td colspan="2">Julio Guillén</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-14</td>
    <td colspan="2">Registrar y gestionar técnicos</td>
    <td colspan="1">UT-06</td>
    <td colspan="2">Crear vista de registro de técnicos</td>
    <td colspan="3">Implementar formulario con campos requeridos (nombre, correo, especialidad).</td>
    <td colspan="1">3</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-14</td>
    <td colspan="2">Registrar y gestionar técnicos</td>
    <td colspan="1">UT-07</td>
    <td colspan="2">Tabla dinámica de técnicos</td>
    <td colspan="3">Mostrar lista de técnicos con opciones de editar y eliminar registros.</td>
    <td colspan="1">4</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestionar equipos de refrigeración</td>
    <td colspan="1">UT-08</td>
    <td colspan="2">Crear vista de listado de equipos</td>
    <td colspan="3">Mostrar tabla con equipos registrados (nombre, modelo, estado, fecha de instalación).</td>
    <td colspan="1">4</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestionar equipos de refrigeración</td>
    <td colspan="1">UT-09</td>
    <td colspan="2">Crear formulario para nuevo equipo</td>
    <td colspan="3">Diseñar formulario para registrar un nuevo equipo de refrigeración.</td>
    <td colspan="1">3</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestionar equipos de refrigeración</td>
    <td colspan="1">UT-10</td>
    <td colspan="2">Integrar API de equipos</td>
    <td colspan="3">Conectar la vista con el endpoint `/api/v1/equipos` para registrar y listar equipos.</td>
    <td colspan="1">3</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>

<tr>
    <td colspan="1">US-28</td>
    <td colspan="2">Acceder a la plataforma web (Call to Action)</td>
    <td colspan="1">UT-11</td>
    <td colspan="2">Vincular botón “Iniciar sesión” con la app web</td>
    <td colspan="3">Asegurar que el botón de la landing page redirija correctamente al login del portal.</td>
    <td colspan="1">1</td>
    <td colspan="2">Kenyi Ramírez</td>
    <td colspan="1">Done</td>
</tr>
</table>

#### 5.2.2.4. Development Evidence for Sprint Review

En este segundo Sprint hemos realizado la implementación de nuestra Frontend, donde todo el equipo ha aportado en varias tareas. En la siguiente tabla se muestran los commits realizados.

<table>
    <tr>
        <th colspan="2">Repository</th>
        <th colspan="2">Branch</th>
        <th colspan="2">Commit Id</th>
        <th colspan="2">Commit Message</th>
        <th colspan="2">Commit Message Body</th>
        <th colspan="2">Committed on (Date)</th>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(auth): add user registration form</td>
        <td colspan="2">Implemented registration form with fields: name and confirmation.</td>
        <td colspan="2">02/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(validation): add email and password validation</td>
        <td colspan="2">Added real-time validation for password strength.</td>
        <td colspan="2">02/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(api): integrate user registration API</td>
        <td colspan="2">Linked registration form to frontend endpoint.</td>
        <td colspan="2">01/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(ui): design login screen</td>
        <td colspan="2">Created login view with inputs for name and password link.</td>
        <td colspan="2">01/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(auth): integrate login API with JWT</td>
        <td colspan="2">Implemented user authentication, managing tokens and session storage.</td>
        <td colspan="2">01/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(technicians): add technician registration view</td>
        <td colspan="2">Developed form for registering new technicians.</td>
        <td colspan="2">05/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(technicians): add technicians table with edit/delete options</td>
        <td colspan="2">Implemented dynamic table for managing technicians.</td>
        <td colspan="2">07/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(equipment): list registered refrigeration units</td>
        <td colspan="2">Created view displaying equipment data: name, model, state and installation date.</td>
        <td colspan="2">03/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(equipment): add form for new equipment registration</td>
        <td colspan="2">Implemented new equipment registration form for refrigeration systems.</td>
        <td colspan="2">07/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">feat(api): integrate equipment API</td>
        <td colspan="2">Connected frontend views with `/api/v1/` for operations.</td>
        <td colspan="2">08/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">fix(ui): fix login redirection from landing page</td>
        <td colspan="2">Linked “Iniciar sesión” button correctly to the web portal login page.</td>
        <td colspan="2">09/10/2025</td>
    </tr>
    <tr>
        <td colspan="2">1ASI0730-2520-7452-G1-FrostShield/IceTrack---Frontend</td>
        <td colspan="2">develop</td>
        <td colspan="2">N/A</td>
        <td colspan="2">Merge branch 'develop' into feature/frontend-sprint2</td>
        <td colspan="2">Final merge after completing Sprint 2 frontend tasks.</td>
        <td colspan="2">09/10/2025</td>
    </tr>
</table>

#### 5.2.2.5. Execution Evidence for Sprint Review

En el Sprint 2 se desplegó la primera versión de la Web Application de IceTrack, implementando funcionalidades esenciales como el dashboard del usuario, lugares, equipos que posee el usuario, las solicitudes de servicio de mantenimiento, las alertas y los reportes generados. Estas funcionalidades permiten a los usuarios hacer uso de herramientas que permitan mejorar la gestión de equipos de refrigeración para su posterior mantenimiento y seguimiento. A continuación, se presentan las evidencias:

**Dashboard:**

![DashboardFrontv1](./assets/chapter05/DashboardFrontv1.png)

<br>

**Sites:**
![SitesFrontv1](./assets/chapter05/SitesFrontv1.png)

![SiteDetailFrontv1](./assets/chapter05/SiteDetailFrontv1.png)

<br>

**Equipments:**

![EquipmentFrontv1](./assets/chapter05/EquipmentFrontv1.png)

![EquipmentDetailFrontv1](./assets/chapter05/EquipmentDetailFrontv1.png)

<br>

**Service Requests:**

![ServiceRequestFrontv1](./assets/chapter05/ServiceRequestFrontv1.png)

![NewServiceRequestFrontv1](./assets/chapter05/NewServiceRequestFrontv1.png)

<br>

**Alerts:**

![AlertsFrontv1](./assets/chapter05/AlertsFrontv1.png)

<br>

**Reports:**

![ReportsFrontv1](./assets/chapter05/ReportsFrontv1.png)

![EditReportFrontv1](./assets/chapter05/EditReportFrontv1.png)

**Url del frontend:** [`https://ice-track-frontend.vercel.app/`](https://ice-track-frontend.vercel.app/)

#### 5.2.2.6. Services Documentation Evidence for Sprint Review

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Para el presente sprint, se realizó el proceso de despliegue para la primera versión del Web Application, así como la Fake API. A continuación, se presentan las evidencias del despliegue:

**Fake API:** Para el despliegue del Fake API, se creó un nuevo repositorio que contiene el db.json para su posterior despliegue en Render.

![EvidenceDeployFakeAPI](./assets/chapter05/EvidenceDeployFakeAPI.png)

**Web Application:** Para el despliegue del Web Application se hizo el despliegue en Vercel a partir del repositorio creado en la organización.

![EvidenceDeployFrontend](./assets/chapter05/EvidenceDeployFrontend.jpg)

#### 5.2.2.8. Team Collaboration Insights during Sprint

![insights-frontend.png](assets/chapter05/insights-frontend.png)

![insights2-landingpage.png](assets/chapter05/insights2-landingpage.png)

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3

<table>
<tr>
    <th colspan="5">Sprint 3</th>
    <th colspan="9">Sprint 3</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-11-02</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">2:30 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Pedro Nanfuñay</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alejandr Galindo, Julio Guillen, Ivan La Madrid, Kenyi Ramírez</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Review Summary</td>
    <td colspan="8">Se realizó el primer despliegue de la web application, implementando funcionalidades orientadas al primer segmento objetivo.</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Retrospective Summary</td>
    <td colspan="8">El equipo se comprometió a cumplir sus partes asignadas, así también como colaborar con otras secciones del trabajo para cumplir nuestro objetivo.</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 3 Goal</td>
       <td colspan="8">El enfoque para este sprint es establecer el núcleo integrado de la plataforma IceTrack. Esto implica conectar la página de inicio pública con la aplicación de usuario funcional (frontend) y un sistema de gestión de datos fundamental (backend). Se espera que esta unificación asegure un punto de entrada sencillo para los usuarios a nuestra aplicación y posibilite la gestión de información esencial, elevando la calidad de la experiencia inicial del usuario y proveyendo al equipo de un cimiento estable para el desarrollo futuro. El resultado exitoso se verificará cuando los usuarios puedan entrar y navegar por la aplicación web central sin obstáculos desde la página de aterrizaje; el sistema de gestión de datos respalde las operaciones para entidades críticas como equipos, solicitudes de servicio, técnicos, reportes y alertas; y la interfaz de usuario logre comunicarse con el sistema de gestión de datos para presentar y manejar dichas entidades principales, probando una conexión operativa entre todos los niveles del sistema.</td>
</tr>
<tr>
    <td colspan="5">Sprint 3 Velocity</td>
    <td colspan="8">100</td>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">97</td>
</tr>
</table>

#### 5.2.3.2. Aspect Leaders and Collaborators

Durante este tercer Sprint, el equipo se enfocó principalmente en el desarrollo, la mejora estructural y visual del frontend y en más de l% de los endpoints asociados al alcance de nuestro proyecto en el backend asegurando la integración entre ellas.
Con el fin de organizar de manera más eficiente el trabajo colaborativo, se ha elaborado la matriz de Liderazgo y Colaboración (LACX). Esta matriz asigna responsabilidades específicas a cada miembro del equipo en relación con los aspectos clave del Sprint.

<table border="1">
  <tr>
    <td colspan="2"><strong>Team Member (Last Name, First Name)</strong></td>
    <td><strong>GitHub Username</strong></td>
    <td><strong>Implementacion de la gestión de equipos de refrigeracion (Frontend Applications)<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Responsividad y pruebas en distintos dispositivos<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Despliegue de la aplicación web<br>Leader (L) / Collaborator (C)</strong></td>
  </tr>
  <tr>
    <td colspan="2">Ramírez Cabrera, Kenyi Efrain</td>
    <td>Kenyi15upc</td>
    <td>L</td>
    <td>C</td>
    <td>L</td>
  </tr>
  <tr>
    <td colspan="2"> Galindo Montero, Alejandro Manuel </td>
    <td>AlejandroG12970</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2"> Guillen Galindo, Julio Adolfo </td>
    <td>julio645</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
  </tr>
  <tr>
    <td colspan="2">La Madrid Lozano, Ivan Jeanpierre</td>
    <td>ivanlamadrid</td>
    <td>C</td>
    <td>C</td>
    <td>L</td>
  </tr>
  <tr>
    <td colspan="2">Nanfuñay Liza, Pedro Jesus</td>
    <td>PedroJ18</td>
    <td>C</td>
    <td>L</td>
    <td>L</td>
  </tr>
</table>

#### 5.2.3.3. Sprint Backlog 3

Nuestro enfoque principal para este Sprint ha sido el desarrollo del frontend y backend de la plataforma IceTrack. Hemos estructurado nuestras tareas siguiendo las User Stories y Technical Stories que hemos detallado, asegurando un progreso claro y alineado con los objetivos de negocio y la arquitectura técnica.

Enlace: https://trello.com/invite/b/691a11e1c474e0f0295ac8bf/ATTId41abf32c3a717b7d5e39eba218930f0541704BF/frontshield

![Sprint1-Trello.png](assets/chapter05/Sprint3-Trello.png)
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Sprint Backlog 3.
  </figcaption>

<table border="1">
<tr>
    <th colspan="3">Sprint 3</th>
    <th colspan="10">Sprint Backend</th>
</tr>
<tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
</tr>
<tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1">Estimation (Hours)</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status</td>
</tr>

<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Registro de usuario</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Crear endpoint /api/v1/users</td>
    <td colspan="3">Implementar registro con validación de email único y hash de contraseña.</td>
    <td colspan="1">6</td>
    <td colspan="2">Julio Guillén</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Registro de usuario</td>
    <td colspan="1">UT-02</td>
    <td colspan="2">Validación de contraseñas</td>
    <td colspan="3">Verificar longitud, complejidad y confirmación de contraseña.</td>
    <td colspan="1">3</td>
    <td colspan="2">Julio Guillén/td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-02</td>
    <td colspan="2">Inicio de sesión</td>
    <td colspan="1">UT-03</td>
    <td colspan="2">Crear endpoint /api/v1/auth/login</td>
    <td colspan="3">Implementar autenticación con JWT y validación de usuario/contraseña.</td>
    <td colspan="1">6</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestionar equipos</td>
    <td colspan="1">UT-04</td>
    <td colspan="2">Crear CRUD de equipos</td>
    <td colspan="3">Endpoints para crear, editar, listar y eliminar equipos.</td>
    <td colspan="1">8</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestionar equipos</td>
    <td colspan="1">UT-05</td>
    <td colspan="2">Validaciones de datos</td>
    <td colspan="3">Validar modelo, número de serie y estado del equipo.</td>
    <td colspan="1">4</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-08</td>
    <td colspan="2">Solicitar servicios</td>
    <td colspan="1">UT-06</td>
    <td colspan="2">Endpoint POST /api/v1/service-requests</td>
    <td colspan="3">Crear solicitud con datos del equipo, tipo y descripción del problema.</td>
    <td colspan="1">7</td>
    <td colspan="2">Julio Guillén</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-09</td>
    <td colspan="2">Seguimiento del servicio</td>
    <td colspan="1">UT-07</td>
    <td colspan="2">Endpoint GET /api/v1/service-status/{id}</td>
    <td colspan="3">Devolver estado actual: pendiente, asignado, en progreso, completado.</td>
    <td colspan="1">4</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-10</td>
    <td colspan="2">Reporte de servicio</td>
    <td colspan="1">UT-08</td>
    <td colspan="2">Generar reporte PDF</td>
    <td colspan="3">Crear documento con resultados, repuestos y observaciones.</td>
    <td colspan="1">6</td>
    <td colspan="2">Julio Guillén/td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-14</td>
    <td colspan="2">Registrar técnicos</td>
    <td colspan="1">UT-09</td>
    <td colspan="2">CRUD de técnicos</td>
    <td colspan="3">Registro, edición y asignación de roles (técnico).</td>
    <td colspan="1">7</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-16</td>
    <td colspan="2">Asignar técnicos a servicios</td>
    <td colspan="1">UT-10</td>
    <td colspan="2">Endpoint asignación técnica</td>
    <td colspan="3">Asignar un técnico a una solicitud y enviar notificación.</td>
    <td colspan="1">5</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-21</td>
    <td colspan="2">Notificaciones de eventos</td>
    <td colspan="1">UT-11</td>
    <td colspan="2">Integrar sistema de notificaciones</td>
    <td colspan="3">Enviar alertas ante cambios de estado o problemas del servicio.</td>
    <td colspan="1">6</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">To Do</td>
</tr>

<tr>
    <td colspan="1">US-22</td>
    <td colspan="2">Evaluar servicio</td>
    <td colspan="1">UT-12</td>
    <td colspan="2">Endpoint POST /api/v1/reviews</td>
    <td colspan="3">Registrar calificación y permitir edición dentro del plazo.</td>
    <td colspan="1">4</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">To Do</td>
</tr>
</table>

#### 5.2.3.4. Development Evidence for Sprint Review

En esta sección se presentan los commits realizados en el repositorio de backend y frontend durante el sprint 3.

**Commits realizados en el repositorio de frontend durante el sprint 3:**

A continuación se presenta un registro de los cambios realizados en la interfaz de usuario de nuestra aplicación. Cada commit detalla las modificaciones efectuadas en el diseño, la estructura y la interacción de los elementos visuales durante este Sprint.

<table>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): create login UI for monitoring platform</td>
	    <td colspan="2">Implemented login screen with form validation and error messages.</td>
	    <td colspan="2">02/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): integrate login API with JWT</td>
	    <td colspan="2">Connected login form with authentication endpoint, added token handling.</td>
	    <td colspan="2">01/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(users): add UI for registering admin/owners</td>
	    <td colspan="2">Created registration form with fields for admin user creation.</td>
	    <td colspan="2">01/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(technicians): create technician registration interface</td>
	    <td colspan="2">Designed form to add new technicians with validation rules.</td>
	    <td colspan="2">05/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(technicians): implement technicians table with actions</td>
	    <td colspan="2">Added list view with edit / delete options and dynamic state updates.</td>
	    <td colspan="2">07/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(equipment): create refrigeration equipment list UI</td>
	    <td colspan="2">Added table view showing equipment name, model, status and installation date.</td>
	    <td colspan="2">03/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(equipment): add new equipment registration form</td>
	    <td colspan="2">Implemented form for adding refrigeration units with basic validation.</td>
	    <td colspan="2">07/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(api): connect equipment views to backend</td>
	    <td colspan="2">Integrated equipment screens with API `/api/v1/equipment` for CRUD operations.</td>
	    <td colspan="2">08/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">fix(ui): correct login redirection</td>
	    <td colspan="2">Fixed landing-page navigation to correctly route users to login.</td>
	    <td colspan="2">09/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">chore: merge develop into feature/frontend-sprint2</td>
	    <td colspan="2">Merged all completed frontend features from Sprint 2.</td>
	    <td colspan="2">09/11/2025</td>
	</tr>
</table>

**Commits realizados en el repositorio de backend durante el sprint 3:**

<table>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): create user registration endpoint</td>
	    <td colspan="2">Added POST /api/v1/auth/register with DTO, validation, hashing and persistence.</td>
	    <td colspan="2">12/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(validation): add email & password validation rules</td>
	    <td colspan="2">Implemented strong password validator and unique email constraint.</td>
	    <td colspan="2">12/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): implement user registration service & mapper</td>
	    <td colspan="2">Connected controller → service → repository for user registration flow.</td>
	    <td colspan="2">11/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): add login endpoint with JWT</td>
	    <td colspan="2">Created POST /api/v1/auth/login issuing JWT tokens and refresh tokens.</td>
	    <td colspan="2">11/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(security): configure JWT filters & authentication manager</td>
	    <td colspan="2">Added token validation, secured routes and role-based access (admin/tech/client).</td>
	    <td colspan="2">11/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(technicians): add technician creation endpoint</td>
	    <td colspan="2">Implemented POST /api/v1/technicians with entity, repository and service.</td>
	    <td colspan="2">15/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(technicians): add CRUD for technicians</td>
	    <td colspan="2">Added GET/PUT/DELETE routes for technician management.</td>
	    <td colspan="2">17/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(equipment): list refrigeration equipment</td>
	    <td colspan="2">Added GET /api/v1/equipment returning filtered & paginated units.</td>
	    <td colspan="2">13/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(equipment): create equipment registration endpoint</td>
	    <td colspan="2">Implemented POST /api/v1/equipment with validation and repository operations.</td>
	    <td colspan="2">07/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(api): integrate equipment service with domain layer</td>
	    <td colspan="2">Connected controllers → services → unit repository for CRUD operations.</td>
	    <td colspan="2">08/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">fix(auth): correct login redirect & unauthorized handler</td>
	    <td colspan="2">Fixed unauthorized responses returning 401 and improved error messages.</td>
	    <td colspan="2">09/11/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">Merge branch 'develop' into feature/backend-sprint2</td>
	    <td colspan="2">Merged backend tasks for Sprint 2 including auth, technicians & equipment modules.</td>
	    <td colspan="2">09/11/2025</td>
	</tr>
</table>

A continuación se presenta un registro detallado de los commits realizados en el repositorio, enfocados a la parte de backend. Cada entrada incluye el identificador único del commit (ID), descripciones realizados durante la elaboracion de esta.

#### 5.2.3.5. Execution Evidence for Sprint Review

En el Sprint 3 se desplegó la segunda versión de la Web Application de IceTrack, implementando funcionalidades complementarias y esenciales en cada una de las secciones de la aplicación. Así mismo, se implementaron mejoras respectivas a la retroalimentación brindada en el sprint anterior. A continuación, se presentan las evidencias:

**Register:**

![RegisterFrontV2](./assets/chapter05/RegisterFrontV2.png)

<br>

**Login:**

![LoginFrontV2](./assets/chapter05/LoginFrontV2.png)

<br>

**Dashboard:**

![DashboardFrontV2](./assets/chapter05/DashboardFrontV2.png)

<br>

**Sites:**

![SitesFrontV2](./assets/chapter05/SitesFrontV2.png)
![SitesDetailFrontV2](./assets/chapter05/SitesDetailFrontV2.png)

<br>

**Equipments:**

![EquipmentsFrontV2](./assets/chapter05/EquipmentsFrontV2.png)
![EquipmentsDetailFrontV2](./assets/chapter05/EquipmentsDetailFrontV2.png)

<br>

**Services:**

![ServicesFrontV2](./assets/chapter05/ServicesFrontV2.png)
![CreateServiceFrontV2](./assets/chapter05/CreateServiceFrontV2.png)

<br>

**Alerts:**

![AlertsFrontV2](./assets/chapter05/AlertsFrontV2.png)

<br>

**Reports:**

![ReportsFrontV2](./assets/chapter05/ReportsFrontV2.png)
![CreateReportFrontV2](./assets/chapter05/CreateReportFrontV2.png)
![EditReportFrontV2](./assets/chapter05/EditReportFrontV2.png)

<br>

**Profile:**

![ProfileFrontV2](./assets/chapter05/ProfileFrontV2.png)
![SettingsFrontV2](./assets/chapter05/SettingsFrontV2.png)

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

**Dashboard**

| Verbo HTTP | Endpoint 		 					    | Descripción 				   |
| :--------: | :--------------------------------------- | :--------------------------- |
| GET		 | /api/v1/dashboard-config/{id}     		| Obtener ID				   |
| PUT		 | /api/v1/dashboard-config/{id}  	  	    | Actualizar ID 			   |
| DELETE 	 | /api/v1/dashboard-config/{id}			| Eliminar ID 				   |
| GET 		 | /api/v1/dashboard-config/user/{userId}   | Obtener configuracion por ID |
| POST 		 | /api/v1/dashboard-config					| Crea configuracion		   |
| POST 		 | /api/v1/dashboard-config/{id}/cards 		| Añade cartas				   |
| GET 		 | /api/v1/dashboard-config/available-cards | Obtener cartas disponible	   |

**ReportController**

| Verbo HTTP | Endpoint 		   | Descripción 										 |
| :--------: | :------------------ | :-------------------------------------------------- |
| POST		 | /api/v1/report      | Crear un nuevo reporte 							 |
| GET		 | /api/v1/report 	   | Obtener un reporte por el ID de un equipo o empresa |
| GET 		 | /api/v1/report/{id} | Obtener un reporte por su ID 						 |

**Equipment**

| Verbo HTTP | Endpoint 		  	  | Descripción	 			|
| :--------: | :--------------------- | :---------------------- |
| POST		 | /api/v1/equipment	  | Crear equipo 			|
| GET		 | /api/v1/equipment 	  | Tener todos los equipos |
| GET		 | /api/v1/equipment/{id} | Tener equipo por ID     |

**Site**

| Verbo HTTP | Endpoint 	     | Descripción	 		  |
| :--------: | :---------------- | :--------------------- |
| POST		 | /api/v1/site	  	 | Crear site 			  |
| GET		 | /api/v1/site 	 | Tener todos los sitios |
| GET		 | /api/v1/site/{id} | Tener sitio por ID     |

**Report**

| Verbo HTTP | Endpoint      	   | Descripción	   	  |
| :--------: | :------------------ | :------------------- |
| POST		 | /api/v1/report 	   | Crear reporte   	  |
| GET		 | /api/v1/report 	   | Tener reportes    	  |
| GET		 | /api/v1/report/{id} | Tener reporte por ID |

**User**

| Verbo HTTP | Endpoint      	   | Descripción	   |
| :--------: | :------------------ | :---------------- |
| GET		 | /api/v1/report/{id} | Tener user por ID |
| GET		 | /api/v1/users 	   | Tener usuarios    |

**Authentication**

| Verbo HTTP | Endpoint 		  			  | Descripción	   |
| :--------: | :----------------------------- | :------------- |
| POST		 | /api/v1/authentication/sign-in | Iniciar sesión |
| POST		 | /api/v1/authentication/sign-up | Registrarse    |

**Alerts**

| Verbo HTTP | Endpoint 		  			  | Descripción	                                 |
| :--------: | :----------------------------- | :--------------------------------------------|                          
| POST		 | /api/v1/authentication/sign-in | Crear alerta                                 |
| GET		 | /api/v1/alert                  | Tener alerta por equipmentid y tenantid      |
| GET		 | /api/v1/alert/{id}             | Tener alerta por Id                          |

---

**Dashboard**

![ReportEndpointsBackendV1](./assets/chapter05/dashboard_0.jpeg)
![PostReportBackendV1](./assets/chapter05/dashboard_1.jpeg)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/dashboard_2.jpeg)
![GetReportByIdBackendV1](./assets/chapter05/dashboard_3.jpeg)
![PostReportBackendV1](./assets/chapter05/dashboard_4.jpeg)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/dashboard_5.jpeg)
![GetReportByIdBackendV1](./assets/chapter05/dashboard_6.jpeg)
![PostReportBackendV1](./assets/chapter05/dashboard_7.jpeg)

**ReportController**

![ReportEndpointsBackendV1](./assets/chapter05/ReportEndpointsBackendV1.png)
![PostReportBackendV1](./assets/chapter05/PostReportBackendV1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/GetReportByEquipmentOrTenantIdBackendV1.png)
![GetReportByIdBackendV1](./assets/chapter05/GetReportByIdBackendV1.png)

**Equipment**

![ReportEndpointsBackendV1](./assets/chapter05/equipment_0.png)
![PostReportBackendV1](./assets/chapter05/equipment_1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/equipment_2.png)
![GetReportByIdBackendV1](./assets/chapter05/equipment_3.png)

**Site**

![ReportEndpointsBackendV1](./assets/chapter05/site_0.png)
![PostReportBackendV1](./assets/chapter05/site_1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/site_2.png)
![GetReportByIdBackendV1](./assets/chapter05/site_3.png)

**Report**

![ReportEndpointsBackendV1](./assets/chapter05/report_0.png)
![PostReportBackendV1](./assets/chapter05/report_1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/report_2.png)
![GetReportByIdBackendV1](./assets/chapter05/report_3.png)

**User**

![ReportEndpointsBackendV1](./assets/chapter05/users_0.png)
![PostReportBackendV1](./assets/chapter05/users1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/users2.png)

**Authentication**

![ReportEndpointsBackendV1](./assets/chapter05/authentication_0.png)
![PostReportBackendV1](./assets/chapter05/authentication_1.png)
![GetReportByEquipmentOrTenantIdBackendV1](./assets/chapter05/authentication_2.png)

**Alerts**
![ReportEndpointsBackendV1](./assets/chapter05/metodos-alertas.png)
![ReportEndpointsBackendV1](./assets/chapter05/post-alertas.png)

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Para esta entrega, desplegamos una nueva versión del Frontend, primera versión del backend y además desplegamos nuestra base de datos para que pueda ser conectada en nuestro backend.

**Frontend Deployment**
![FrontEndDeployment](./assets/chapter05/deploy-frontend-tb2.png)

**Backend Deployment**
![BackEndDeployment](./assets/chapter05/deploy-backend-tb2.png)

**Database Deployment**
![DatabaseDeployment](./assets/chapter05/deploy-database-tb2.jpg)

**Swagger desde el deploy de nuestro backend**
![BACKDEPLOY1.png](assets/chapter05/BACKDEPLOY1.png)

![BACKDEPLOY2.png](assets/chapter05/BACKDEPLOY2.png)

![BACKDEPLOY3.png](assets/chapter05/BACKDEPLOY3.png)

#### 5.2.3.8. Team Collaboration Insights during Sprint

Frontend:
![Insights-TB2FRONT.png](assets/chapter05/Insights-TB2FRONT.png)

Backend:
![InsightsTB2BACKEND.png](assets/chapter05/InsightsTB2BACKEND.png)

### 5.2.4. Sprint 4

#### 5.2.4.1. Sprint Planning 4

<table>
<tr>
    <th colspan="5">Sprint 4</th>
    <th colspan="9">Sprint 4</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-10-03</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">6:00 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Kenyi Ramirezy</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alejandro Galindo, Julio Guillen, Ivan La Madrid, Pedro Nanfuñay, Kenyi Ramírez</td>
</tr>
<tr>
    <td colspan="5">Sprint 3 Review Summary</td>
    <td colspan="8">Se realizó el despliegue del Frontend y Backend, implementando funcionalidades orientadas al primer y segundo segmento objetivo.</td>
</tr>
<tr>
    <td colspan="5">Sprint 3 Retrospective Summary</td>
    <td colspan="8">El equipo acordó encargarse de las tareas asignadas y colaborar con las demás áreas del proyecto del Frontend y Backend para alcanzar nuestro objetivo.</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 4 Goal</td>
       <td colspan="8">El objetivo de este sprint es completar la integración principal de IceTrack conectando directamente el frontend con el backend. Esto implica enlazar la página con la aplicación de usuario y establecer la comunicación operativa con el sistema de gestión de datos. Con esta conexión final, los usuarios podrán ingresar y navegar sin problemas desde la página de inicio hasta la aplicación central, mientras que el backend proporcionará el soporte necesario para manejar entidades clave como equipos, solicitudes de servicio, técnicos, reportes y alertas. La integración entre la interfaz y el sistema de datos confirmará que ambos lados de la aplicación funcionan juntos, marcando un paso crucial hacia la finalización de la plataforma.</td>
</tr>
<tr>
    <td colspan="5">Sprint 4 Velocity</td>
    <td colspan="8">90</td>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">90</td>
</tr>
</table>

#### 5.2.4.2. Aspect Leaders and Collaborators

Durante este cuarto Sprint, el equipo se enfocó en avanzar y refinar tanto la estructura y el diseño del frontend como la mayor parte de los endpoints del backend, con el objetivo de dejar ambas partes listas para su integración. Además, para organizar de forma más eficiente el trabajo colaborativo, se creó la matriz de Liderazgo y Colaboración (LACX), donde se asignan claramente las responsabilidades de cada miembro en los aspectos centrales del Sprint.

<table border="1">
  <tr>
    <td colspan="2"><strong>Team Member (Last Name, First Name)</strong></td>
    <td><strong>GitHub Username</strong></td>
    <td><strong>Service Request Management<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Assets Managements and Equipment<br>Leader (L) / Collaborator (C)</strong></td>
	<td><strong>Dashboard and Analytics<br>Leader (L) / Collaborator (C)</strong></td>
    <td><strong>Despliegue de la aplicación web<br>Leader (L) / Collaborator (C)</strong></td>
  </tr>
  <tr>
    <td colspan="2">Ramírez Cabrera, Kenyi Efrain</td>
    <td>Kenyi15upc</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
	<td>C</td>
  </tr>
  <tr>
    <td colspan="2"> Galindo Montero, Alejandro Manuel </td>
    <td>AlejandroG12970</td>
    <td>C</td>
    <td>C</td>
    <td>C</td>
	<td>L</td>
  </tr>
  <tr>
    <td colspan="2"> Guillen Galindo, Julio Adolfo </td>
    <td>julio645</td>
    <td>C</td>
    <td>L</td>
    <td>C</td>
	<td>C</td>
  </tr>
  <tr>
    <td colspan="2">La Madrid Lozano, Ivan Jeanpierre</td>
    <td>ivanlamadrid</td>
    <td>C</td>
    <td>C</td>
    <td>L</td>
	<td>C</td>
  </tr>
  <tr>
    <td colspan="2">Nanfuñay Liza, Pedro Jesus</td>
    <td>PedroJ18</td>
    <td>L</td>
    <td>C</td>
    <td>C</td>
	<td>C</td>
  </tr>
</table>

#### 5.2.4.3. Sprint Backlog 4

En este Sprint nos enfocamos principalmente en la integración completa entre el frontend y el backend de IceTrack. Todas las funcionalidades desarrolladas en sprints anteriores fueron conectadas, probadas y ajustadas para asegurar que la plataforma funcione de manera coherente y estable. Organizamos el trabajo basándonos en las User Stories correspondientes, garantizando un avance ordenado y alineado con los objetivos técnicos y operativos del proyecto.

Enlace: 

![Sprint1-Trello.png](assets/chapter05/Sprint3-Trello.png)
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Sprint Backlog 4.
  </figcaption>

<table border="1">
<tr>
    <th colspan="3">Sprint #</th>
    <th colspan="10">Sprint 4</th>
</tr>

<tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
</tr>

<tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1">Estimation (Hours)</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status</td>
</tr>
<tr>
    <td colspan="1">US-01</td>
    <td colspan="2">Integración de registro de usuario</td>
    <td colspan="1">UT-01</td>
    <td colspan="2">Conectar formulario con API final</td>
    <td colspan="3">Validar envío al endpoint real y manejar errores de backend (mail duplicado, contraseña inválida).</td>
    <td colspan="1">3</td>
    <td colspan="2">Julio Guillén</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-02</td>
    <td colspan="2">Integración de inicio de sesión</td>
    <td colspan="1">UT-02</td>
    <td colspan="2">Sincronizar JWT con frontend</td>
    <td colspan="3">Guardar token seguro, manejar expiración y redirección correcta al dashboard.</td>
    <td colspan="1">4</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-03</td>
    <td colspan="2">Gestión de equipos</td>
    <td colspan="1">UT-03</td>
    <td colspan="2">Integrar listado de equipos con API</td>
    <td colspan="3">Conectar tabla con Equipment y mostrar estados reales.</td>
    <td colspan="1">4</td>
    <td colspan="2">Kenyi Ramirez</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-06</td>
    <td colspan="2">Control de encendido/apagado</td>
    <td colspan="1">UT-04</td>
    <td colspan="2">Integrar botón de encendido con API</td>
    <td colspan="3">Enviar comando con el Id y actualizar estado visual.</td>
    <td colspan="1">3</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-07</td>
    <td colspan="2">Control de temperatura</td>
    <td colspan="1">UT-05</td>
    <td colspan="2">Integrar slider con endpoint de temperatura</td>
    <td colspan="3">Actualizar temperatura en tiempo real llamando el tipo de equipo del usuario.</td>
    <td colspan="1">4</td>
    <td colspan="2">Pedro Nanfuñay</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-08</td>
    <td colspan="2">Solicitar mantenimiento</td>
    <td colspan="1">UT-06</td>
    <td colspan="2">Integrar formulario con API de servicios</td>
    <td colspan="3">Enviar solicitudes a endpoints y confirmar recepción.</td>
    <td colspan="1">3</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-09</td>
    <td colspan="2">Seguimiento del servicio</td>
    <td colspan="1">UT-07</td>
    <td colspan="2">Conectar tracking con API</td>
    <td colspan="3">Actualizar estados (pendiente, en camino, en proceso, finalizado) desde backend.</td>
    <td colspan="1">4</td>
    <td colspan="2">Iván La Madrid</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-12</td>
    <td colspan="2">Historial de servicios</td>
    <td colspan="1">UT-08</td>
    <td colspan="2">Leer servicios desde API</td>
    <td colspan="3">Mostrar tabla real de pagina desde Site.</td>
    <td colspan="1">3</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US-21</td>
    <td colspan="2">Notificaciones</td>
    <td colspan="1">UT-09</td>
    <td colspan="2">Integrar sistema de notificaciones</td>
    <td colspan="3">Conectar con WebSockets o servicio push y mostrar alertas en frontend.</td>
    <td colspan="1">5</td>
    <td colspan="2">Alejandro Galindo</td>
    <td colspan="1">Done</td>
</tr>
</table>

#### 5.2.4.4. Development Evidence for Sprint Review

En esta sección se presentan los commits realizados en el repositorio de backend y frontend durante el sprint 4.

**Commits realizados en el repositorio de frontend durante el sprint 4:**

<table>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): create login UI for monitoring platform</td>
	    <td colspan="2">Implemented login screen with form validation and error messages.</td>
	    <td colspan="2">02/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): integrate login API with JWT</td>
	    <td colspan="2">Connected login form with authentication endpoint, added token handling.</td>
	    <td colspan="2">01/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">fix(ui): correct login redirection</td>
	    <td colspan="2">Fixed landing-page navigation to correctly route users to login.</td>
	    <td colspan="2">04/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Frontend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">chore: merge develop into feature/frontend-sprint2</td>
	    <td colspan="2">Merged all completed frontend features from Sprint 2.</td>
	    <td colspan="2">03/12/2025</td>
	</tr>
</table>

**Commits realizados en el repositorio de backend durante el sprint 4:**

<table>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): create user registration endpoint</td>
	    <td colspan="2">Added POST /api/v1/auth/register with DTO, validation, hashing and persistence.</td>
	    <td colspan="2">02/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): implement user registration service & mapper</td>
	    <td colspan="2">Connected controller → service → repository for user registration flow.</td>
	    <td colspan="2">01/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">feat(auth): add login endpoint with JWT</td>
	    <td colspan="2">Created POST /api/v1/auth/login issuing JWT tokens and refresh tokens.</td>
	    <td colspan="2">01/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">fix(auth): correct login redirect & unauthorized handler</td>
	    <td colspan="2">Fixed unauthorized responses returning 401 and improved error messages.</td>
	    <td colspan="2">03/12/2025</td>
	</tr>
	<tr>
	    <td colspan="2">FrostShield/IceTrack---Backend</td>
	    <td colspan="2">develop</td>
	    <td colspan="2">N/A</td>
	    <td colspan="2">Merge branch 'develop' into feature/backend-sprint4</td>
	    <td colspan="2">Merged backend tasks for Sprint 2 including auth, technicians & equipment modules.</td>
	    <td colspan="2">04/12/2025</td>
	</tr>
</table>

#### 5.2.4.5. Execution Evidence for Sprint Review

En el Sprint 4 se desplegó la última versión de la Web Application de IceTrack, implementando mejoras complementarias y esenciales para garantizar la eficiencia de cada una de las secciones de la aplicación. A continuación, se presentan las evidencias:

*Owner View:*

**Register:**

![RegisterFrontVF](assets/chapter05/RegisterFrontVF.png)

**Login:**

![LoginFrontVF](assets/chapter05/LoginFrontVF.png)

**Dashboard:**

![DashboardFrontVF](assets/chapter05/DashboardFrontVF.png)

![DashboardAddCardFrontVF](assets/chapter05/DashboardAddCardFrontVF.png)

![DashboardEditCardFrontVF](assets/chapter05/DashboardEditCardFrontVF.png)

**Sites:**

![SitesFrontVF](assets/chapter05/SitesFrontVF.png)
![SitesDetailFrontVF](assets/chapter05/SiteDetailFrontVF.png)

**Equipments:**

![EquipmentsFrontVF](assets/chapter05/EquipmentsFrontVF.png)
![EquipmentsDetailFrontVF](assets/chapter05/EquipmentDetailFrontVF.png)

**Services Requests:**

![ServicesFrontVF](assets/chapter05/ServicesFrontVF.png)
![AddServicesFrontVF](assets/chapter05/AddServiceRequestFrontVF.png)

**Alerts:**

![AlertsFrontVF](assets/chapter05/AlertsFrontVF.png)

**Reports:**

![ReportsFrontVF](assets/chapter05/ReportsFrontVF.png)
![AddReportFrontVF](assets/chapter05/AddReportFrontVF.png)
![ReportsDetailFrontVF](assets/chapter05/ReportDetailFrontVF.png)
![EditReportFrontVF](assets/chapter05/EditReportFrontVF.png)

<br>

*Service Provider View:*

**Dashboard:**

![DashboardProviderFrontVF](assets/chapter05/ProviderDashboardVF.png)

**Provider Services:**

![ServicesHubFrontVF](assets/chapter05/ServicesHubFrontVF.png)
![ServicesRequestsFrontVF](assets/chapter05/ProviderServicesFrontVF.png)

**Technician Management:**

![TechnicianManagementFrontVF](assets/chapter05/TechnicianManagementFrontVF.png)


#### 5.2.4.6. Services Documentation Evidence for Sprint Review

**DashboardConfigs**

| Verbo HTTP | Endpoint 		 					    | Descripción 				   |
| :--------: | :--------------------------------------- | :--------------------------- |
| GET		 | /api/v1/dashboard-configs/{id}     		| Obtener ID				   |
| PUT		 | /api/v1/dashboard-configs/{id}  	  	    | Actualizar ID 			   |
| DELETE 	 | /api/v1/dashboard-configs/{id}			| Eliminar ID 				   |
| GET 		 | /api/v1/dashboard-configs/user/{userId}   | Obtener configuracion por ID |
| POST 		 | /api/v1/dashboard-configs					| Crea configuracion		   |
| POST 		 | /api/v1/dashboard-configs/{id}/cards 		| Añade cartas				   |
| GET 		 | /api/v1/dashboard-configs/available-cards | Obtener cartas disponible	   |
| PATCH		 | /api/v1/dashboard-configs/{id}/cards/{cardId}/visibility | Actualizar visibilidad	   |

**Report**

| Verbo HTTP | Endpoint 		   | Descripción 										 |
| :--------: | :------------------ | :-------------------------------------------------- |
| POST		 | /api/v1/reports     | Crear un nuevo reporte 							 |
| GET		 | /api/v1/reports 	   | Obtener un reporte por el ID de un equipo o empresa |
| GET 		 | /api/v1/report/{id} | Obtener un reporte por su ID 						 |
| PUT		 | /api/v1/report/{id} | Actualizar un reporte por su ID 						 |
| DELETE 		 | /api/v1/report/{id} | Eliminar un reporte por su ID 						 |

**Equipment**

| Verbo HTTP | Endpoint 		  	  | Descripción	 			|
| :--------: | :--------------------- | :---------------------- |
| POST		 | /api/v1/equipment	  | Crear equipo 			|
| GET		 | /api/v1/equipment 	  | Tener todos los equipos |
| GET		 | /api/v1/equipment/{id} | Tener equipo por ID     |

**Site**

| Verbo HTTP | Endpoint 	     | Descripción	 		  |
| :--------: | :---------------- | :--------------------- |
| POST		 | /api/v1/site	  	 | Crear site 			  |
| GET		 | /api/v1/site 	 | Tener todos los sitios |
| GET		 | /api/v1/site/{id} | Tener sitio por ID     |
| DELETE		 | /api/v1/site/{id} | Eliminar sitio por ID     |


**User**

| Verbo HTTP | Endpoint      	   | Descripción	   |
| :--------: | :------------------ | :---------------- |
| GET		 | /api/v1/report/{id} | Tener user por ID |
| GET		 | /api/v1/users 	   | Tener usuarios    |
| GET		 | /api/v1/users/role/{role} 	   | Tener usuarios por rol    |

**Authentication**

| Verbo HTTP | Endpoint 		  			  | Descripción	   |
| :--------: | :----------------------------- | :------------- |
| POST		 | /api/v1/authentication/sign-in | Iniciar sesión |
| POST		 | /api/v1/authentication/sign-up | Registrarse    |

**Alerts**

| Verbo HTTP | Endpoint 		  			  | Descripción	                                 |
| :--------: | :----------------------------- | :--------------------------------------------|                          
| POST		 | /api/v1/authentication/sign-in | Crear alerta                                 |
| GET		 | /api/v1/alert                  | Tener alerta por equipmentid y tenantid      |
| GET		 | /api/v1/alert/{id}             | Tener alerta por Id                          |

**Reviews**

| Verbo HTTP | Endpoint 	     | Descripción	 		  |
| :--------: | :---------------- | :--------------------- |
| POST		 | /api/v1/reviews	  	 | Crear reseña 			  |
| GET		 | /api/v1/reviews 	 | Tener todas los reseñas |
| GET		 | /api/v1/site/{id} | Tener reseña por ID     |

**ServiceRequests**

| Verbo HTTP | Endpoint 	     | Descripción	 		  |
| :--------: | :---------------- | :--------------------- |
| POST		 | /api/v1/service-requests	  	 | Crear request 			  |
| GET		 | /api/v1/service-requests/{serviceRequestId}		 | Tener todos los requests |
| GET		 | /api/v1/service-requests/requester/{requesterId} | Tener request por requester ID     |
| PATCH		 | /api/v1/service-requests/{serviceRequestId}/accept | aceptar request por requester ID     |
| PATCH		 | /api/v1/service-requests/{serviceRequestId}/reject | Denegar request por requester ID     |
| PATCH		 | /api/v1/service-requests/{serviceRequestId}/cancel | cancelar request por requester ID     |
| PATCH		 | /api/v1/service-requests/{serviceRequestId}/assign-technician | asignar tecnico a request   |

**Interventions**

| Verbo HTTP | Endpoint 	     | Descripción	 		  |
| :--------: | :---------------- | :--------------------- |
| POST		 | /api/v1/interventions	  	 | Crear intervencion 			  |
| GET		 | /api/v1/interventions/{interventionId} 	 | Tener intervenciones por Id |


**Technicians**

| Verbo HTTP | Endpoint 		   | Descripción 										 |
| :--------: | :------------------ | :-------------------------------------------------- |
| POST		 | /api/v1/reports     | Crear un nuevo tecnico 							 |
| GET		 | /api/v1/reports 	   | Obtener un tecnico por el ID de un proveedor |
| GET 		 | /api/v1/report/{id} | Obtener un tecnico por su ID 						 |
| PUT		 | /api/v1/report/{id} | Actualizar un tecnico por su ID 						 |
| DELETE 		 | /api/v1/report/{id} | Eliminar un tecnico por su ID 	


**Technicians**
![technicians-swagger](./assets/chapter05/technicians-swagger.png)

**Interventions**
![interventions-swagger](./assets/chapter05/interventions-swagger.png)

**ServiceRequests**
![Service-requests-swagger](./assets/chapter05/service-request-swagger.png)

**Authentication**
![autentication-swagger](./assets/chapter05/autentication-swagger.png)

**Users**
![users-swagger](./assets/chapter05/users-swagger.png)

**Reviews**
![review-swagger](./assets/chapter05/review-swagger.png)

**DashboardConfigs**
![dashboard-configs-swagger](./assets/chapter05/dashboard-configs-swagger.png)

**Alert**
![alert-swagger](./assets/chapter05/alert-swagger.png)

**Equipment**
![equipment-swagger](./assets/chapter05/equipment-swagger.png)

**Report**
![report-swagger](./assets/chapter05/report-swagger.png)

**Site**
![site-swagger](./assets/chapter05/site-swagger.png)

---

#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Para esta entrega, desplegamos una nueva versión del Frontend, segunda versión del backend y además desplegamos una nueva base de datos para que pueda ser conectada en nuestro backend.

**Frontend Deployment**
![FrontEndDeployment](./assets/chapter05/deploy-frontend-tf.png)

**Backend Deployment**
![BackEndDeployment](./assets/chapter05/deploy-backend-tf.png)

**Database Deployment**
![DatabaseDeployment](./assets/chapter05/deploy-database-tf.png)

#### 5.2.4.8. Team Collaboration Insights during Sprint

Frontend:
![Insights-TB2FRONT.png](assets/chapter05/Insights-TFFRONT.png)

Backend:
![InsightsTB2BACKEND.png](assets/chapter05/InsightsTFBACKEND.png)

## 5.3. Validation Interviews

### 5.3.1. Diseño de Entrevistas

## **Objetivo de la Entrevista**

Validar la usabilidad, efectividad y propuesta de valor de la plataforma IceTrack enfocada en el monitoreo de equipos de refrigeración para los segmentos clave. Se evaluará si las funcionalidades cubren las necesidades reales de operación, mantenimiento y supervisión, y si los flujos son intuitivos para usuarios con distintos perfiles técnicos.

## **Elementos de Validación**

**Landing Page**

- Claridad de la propuesta de valor.
- Acceso rápido a funcionalidades clave.

**Aplicación Web**

- Registro de equipos de refrigeración.
- Configuración de sensores (temperatura, humedad, consumo). 
- Visualización del estado en tiempo real.
- Generación y recepción de alertas.
- Solicitud de mantenimiento.
- Visualización de reportes de uso, consumo y fallas.
- Gestión de técnicos y mantenimientos programados.

## **Para el Segmento 1: Negocios con equipos de refrigeración**

- Agregar equipos
- Monitoreo y alertas
- Ver dashboards
- Recibir alertas por alta temperatura, apertura prolongada, fallas eléctricas
- Visualización de reportes
- Histórico de temperatura
- Consumo energético
- Horas de funcionamiento

## **Para el Segmento 2: Técnicos y empresas de mantenimiento**

- Gestión de técnicos
- Ver disponibilidad y ubicación
- Intervenciones previas por equipo
- Generación de reportes
- Rendimiento de técnicos
- Equipos por cliente
- Mantenimientos programados

## **Formato de Registro de Entrevista**

- Nombre completo
- Edad
- Distrito de residencia
-  Rol en su empresa
-  Dispositivo utilizado para la prueba

## **Preguntas para el Segmento**

**Registro y Autenticación de Usuario**
- ¿Los campos solicitados (nombre, email, contraseña) te parecieron apropiados para crear tu cuenta?
- ¿El inicio de sesión fue rápido y sin errores inesperados?
  
**Dashboard**

- Al ingresar al panel principal, ¿lograste entender rápidamente cómo navegar por las diferentes secciones?
- ¿La información de resumen que se muestra es útil para tener una visión general?
  
**Sites**

- ¿La información de los sitios en listas facilita su identificación y organización?
- ¿Encontraste sin problemas la opción para ver el listado de equipos de refrigeración?
- ¿La visualización de direcciones o IDs fue clara y coherente con lo esperado?
  
**Equipments**

- Al visualizar los equipos, ¿la información mostrada es relevante para tus necesidades?
- ¿Pudiste distinguir fácilmente el estado de cada equipo?
- ¿Los botones de acción (por ejemplo, “More”, “Equipment detail”) respondieron correctamente?
  
**Alertas y Reportes**

- ¿Te resultó fácil interpretar las alertas (colores, tipo, severidad)?
- ¿Pudiste acceder fácilmente a los reportes generados?
- ¿Los filtros y botones (por ejemplo, “Ver Reporte” o “View Equipment”) funcionaron como esperabas?

**Servicios**

- ¿Cómo fue tu experiencia solicitando un servicio?
- ¿La opción para programar mantenimiento estaba visible y disponible?¿Qué te pareció su implementación?

**Configuración y Perfil**

- ¿Ubicaste la sección de Configuración sin dificultad?
- ¿Los cambios realizados (idioma, tema) se mantuvieron al recargar la página o volver a iniciar sesión?

**Experiencia General**

- ¿La aplicación te pareció visualmente atractiva y coherente en todas sus secciones?
- ¿Consideras que el flujo general (inicio, navegación, reportes) es lógico e intuitivo?
- ¿Tuviste algún problema técnico (errores, lentitud, fallos de carga)?

### 5.3.2. Registro de Entrevistas.

## Segmento objetivo #1: Negocios con equipos de refrigeración

**Entrevista 1:**

- **Nombres y apellidos:** Henrry Aiquipa
- **Edad:** 25
- **Distrito:** San Martín de Porres

![Interview-1-segment-1.png](assets/chapter05/entrevista-2-segmento-1.png)

- **Inicio:** 0:00
- **Duración:** 14:49 min
- **URL:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a352_upc_edu_pe/IQDZJDCV5rVLQJHq_pq3M0RWAZbT8M6ee7V0Eo77-ESq_0U?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=fUbOGP
- **Resumen:** Henrry Aiquipa, 25 años, dueño de una bodega en San Martín de Porres, tuvo una experiencia en general positiva con la plataforma para negocios con equipos de refrigeración. Percibió el registro e inicio de sesión como simples y sin errores, y encontró el dashboard intuitivo, con un resumen útil del estado de sus equipos. Destacó que las secciones de “Sites” y “Equipments” están bien organizadas, con información relevante y estados de equipos fáciles de identificar. Valoró también la claridad de las alertas y la facilidad para acceder a reportes y solicitar servicios o programar mantenimientos. Ubicó sin problema la sección de configuración y confirmó que los cambios se guardan correctamente. En conjunto, considera que la aplicación es visualmente agradable, coherente e intuitiva, mencionando solo pequeños retrasos puntuales que no afectan su uso general.

**Entrevista 2:**

- **Nombres y apellidos:** Sonia Rocio
- **Edad:** 59
- **Distrito:** Lima

![Interview-1-segment-1.png](assets/chapter05/entrevista-1-segmento-1.png)

- **Inicio:** 0:00
- **Duración:** 5:21 min
- **URL:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a352_upc_edu_pe/IQCK3Oq7XMaZRL7U5QnkIAKuAeHFhMJhaovEMp5L-PuTANE?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=5HVhkd
- **Resumen:** La señora Rocío Galindo, comenta que la plataforma para negocios con equipos de refrigeración le resultó clara y sencilla de usar: el registro y el ingreso fueron fáciles, el panel principal le mostró de inmediato el estado de sus equipos y las secciones de “Sites” y “Equipments” le parecieron muy ordenadas. Destaca que las alertas son comprensibles, los reportes y las solicitudes de mantenimiento están al alcance y que la configuración permite hacer cambios sin dificultad. En general, afirma que la aplicación es visualmente agradable, coherente y práctica para su día a día.

**Entrevista 3:**

- **Nombres y apellidos:** Mauricio Mego
- **Edad:** 22
- **Distrito:** Lima

![Interview-1-segment-1.png](assets/chapter05/entrevista-alejandro.png)

- **Inicio:** 0:00
- **Duración:** 6:02 min
- **URL:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a352_upc_edu_pe/IQBJ0SiZQ9aMR6QPa0IBM5jrAQxA99usZN4RQIdTMA8w49Y?e=Yl7TId&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Resumen:** Mauricio administra junto a su padre un minimarket que contiene varios equipos de refrigeración, por lo que depende de ellos para poder conservar alimentos. Él en la entrevista menciona que le pareció atractiva e intuitiva. El dashboard le pareció conciso y facil de entender, al igual que las alertas, servicios, equipos y sitios. Sí recomendaría utilizar la aplicación a otras personas y la utilizaría para poder tener mejor control sobre sus equipos y poder solicitar servicios por si alguno falla.

---

## Segmento Objetivo 2 - Técnicos y empresas de mantenimiento:

**Entrevista 1:**

- **Nombres y apellidos:** Alvaro Piettro Salazar Urbina
- **Edad:** 24
- **Distrito:** Comas

![Interview-1-segment-1.png](assets/chapter05/ValidationInterview1-Segmento2.png)

- **Inicio:** 0:28 min
- **Duración:** 14:49 min
- **URL:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a352_upc_edu_pe/IQDZJDCV5rVLQJHq_pq3M0RWAZbT8M6ee7V0Eo77-ESq_0U?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=fUbOGP
- **Resumen:** Alvaro Salazar, 24 años, técnico especializado en servicios de mantenimiento en máquinas de refrigeración. Ante su experiencia en este rubro, comparte su opinión y retroalimentación acerca de nuestra aplicación IceTrack. Tras haber hecho uso de la aplicación, comenta que la interfaz fue sencilla y fácil de entender. Así mismo, cree que el flujo de la aplicación es sencilla y no cuenta con dificultades o elementos que distraigan la atención. Considera que el tiempo de espera se encuentra en el tiempo promedio que se espera de este tipo de aplicaciones y considera apropiado la creación de reportes para mejorar su eficiencia en servicios de mantenimiento. En conclusión, Alvaro considera que nuestra aplicación cumple con el objetivo de resolver las necesidades de los usuarios con una interfaz sencilla de entender y visualmente agradable.

---

### 5.3.3. Evaluaciones según heurísticas

**Esta evaluacion fue hecho con el Grupo 4:**

## Evaluación Heurística de Usabilidad y Diseño Inclusivo para la Aplicación: "IceTrack"

**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**

**CARRERA	: Ingeniería de Software**

**CURSO	: Aplicaciones Web**

**SECCIÓN	: 7452**

**PROFESORES	: Todos**

**AUDITOR	: Samuel Jesus Bonifacio Jaramillo**

**CLIENTE(S)	:**

	   **Galindo Montero, Alejandro Manuel**   

	   **Guillen Galindo, Julio Adolfo**   

	   **La Madrid Lozano, Ivan Jeanpierre** 

	   **Nanfuñay Liza, Pedro Jesus**

	   **Ramirez Cabrera, Kenyi Efrain**

**SITE o APP A EVALUAR:** IceTrack

## TAREAS A EVALUAR:

El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Ambigüedad en la terminología y las unidades de las temperaturas máximas.
2. Falta de retroalimentación visual prominente al seleccionar un elemento en el menú lateral.
3. La acción "Acknowledge (ACK)" aparece en alertas cuyo estado ya es "Resolved" o "Closed".
4. Etiquetado "5 puntos" en el filtro del gráfico de temperatura es poco claro.
5. Botones de acción principal (ej. "Equipment detail") están mal etiquetados, no indican la acción de creación.
6. Uso de identificadores internos ("e1", "s1", "t2") en las tablas principales de activos y alertas.
7. Las fechas y horas en los detalles de equipos se muestran en formato UTC/Z sin conversión a hora local.
8. Confusión visual entre campos editables y no editables en la sección de información de usuario.
9. Redundancia o falta de claridad en los filtros de la sección "My Service Requests".

## ESCALA DE SEVERIDAD:

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad

| Nivel | Descripción                                                                                                                                                                                    |
| :---: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Problema superficial: puede ser fácilmente superador por el usuario ó ocurre con muy poco frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo.                  |
| 2     | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente reléase |
| 3     | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.                                |
| 4     | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.                              |

## TABLA RESUMEN:

| \#  | Problema                                                                                                      | Escala de severidad | Heurística/Principio violada(o)                                          |
| :-: | :------------------------------------------------------------------------------------------------------------ | :-----------------: | :----------------------------------------------------------------------- |
| 1   | Ambigüedad en la terminología y las unidades de las temperaturas máximas.                                     | 3                   | Visibility of System Status / Consistency and Standards                  |
| 2   | Falta de retroalimentación visual prominente al seleccionar un elemento en el menú lateral.                   | 2                   | Visibility of System Status                                              |
| 3   | La acción "Acknowledge (ACK)" aparece en alertas cuyo estado ya es "Resolved" o "Closed".                     | 3                   | Error Prevention / Consistency and Standards                             |
| 4   | Etiquetado "5 puntos" en el filtro del gráfico de temperatura es poco claro.                                  | 2                   | Recognition Rather Than Recall / Aesthetic and Minimalist Design         |
| 5   | Botones de acción principal (ej. "Equipment detail") están mal etiquetados, no indican la acción de creación. | 3                   | Consistency and Standards / Match Between System and the Real World      |
| 6   | Uso de identificadores internos ("e1", "s1", "t2") en las tablas principales de alertas.                      | 3                   | Recognition Rather Than Recall / Match Between System and the Real World |
| 7   | Las fechas y horas en los detalles de equipos se muestran en formato UTC/Z sin conversión a hora local.       | 4                   | Match Between System and the Real World                                  |
| 8   | Confusión visual entre campos editables y no editables en la sección de información de usuario.               | 3                   | Visibility of System Status / Aesthetic and Minimalist Design            |
| 9   | Redundancia o falta de claridad en los filtros de la sección "My Service Requests".                           | 2                   | Aesthetic and Minimalist Design / Flexibility and Efficiency of Use      |

## DESCRIPCIÓN DE PROBLEMAS:

## PROBLEMA \#1: Ambigüedad en la terminología y las unidades de las temperaturas máximas.

- **Severidad: 3 Heurística violada: Visibility of System Status / Consistency and Standards**
- Problema: En el Dashboard, la sección superior derecha muestra "Max: 3.8°" y "Max: 4.3°". No hay una etiqueta que explique si estos son límites preconfigurados, los máximos históricos, o los máximos registrados en las últimas 24h. Esta falta de contexto clave impide al usuario entender el significado de estas métricas. Además, la unidad de temperatura usa ° en estos máximos, mientras que el promedio usa °C, mostrando una inconsistencia.
- Recomendación: Etiquetar claramente los valores, por ejemplo, "Límite Alto" o "Máximo Histórico". Unificar el símbolo de temperatura a °C en toda la interfaz.

## PROBLEMA \#2: Falta de retroalimentación visual prominente al seleccionar un elemento en el menú lateral.

- **Severidad: 2 Heurística violada: Visibility of System Status**
- Problema: El elemento del menú lateral activo ("Equipments" en su vista) se indica con un sutil color de fondo azul que podría no ser lo suficientemente visible o contrastante para algunos usuarios. Esto dificulta la confirmación instantánea de la ubicación actual del usuario en la aplicación.
- Recomendación: Reforzar la indicación del elemento activo. Sugerencia: Añadir un borde vertical (ej. una línea gruesa azul) al lado izquierdo del elemento seleccionado para un contraste más fuerte.

## PROBLEMA \#3: La acción "Acknowledge (ACK)" aparece en alertas cuyo estado ya es "Resolved" o "Closed".

- **Severidad: 3 Heurística violada: Error Prevention / Consistency and Standards**
- Problema: En la tabla "Recent Alerts" del Dashboard, se ofrece la acción "Acknowledge (ACK)" para alertas que ya tienen un estado de "Resolved" o "Closed". Lógicamente, no se requiere o no debería ser posible "reconocer" una alerta que el sistema ya considera - - finalizada. Esto genera confusión e impulsa acciones innecesarias.
- Recomendación: Hacer que la columna ACTION sea contextual: debe desaparecer o cambiar a una opción como "View Log" o "View Details" cuando el Status sea finalizado.

## PROBLEMA \#4: Etiquetado "5 puntos" en el filtro del gráfico de temperatura es poco claro.

- **Severidad: 2 Heurística violada: Recognition Rather Than Recall / Aesthetic and Minimalist Design**
- Problema: El texto "5 pontos" sobre el gráfico de temperatura es técnico o está mal traducido/etiquetado. El usuario no puede saber fácilmente si se refiere a 5 sensores, 5 días, o la granularidad de los datos. Esto obliga al usuario a recordar su significado.
- Recomendación: Utilizar una etiqueta clara y orientada al usuario, como "5 Sensores", "Granularidad" o el parámetro real que se esté filtrando.

## PROBLEMA \#5: Botones de acción principal (ej. "Equipment detail") están mal etiquetados, no indican la acción de creación.

- **Severidad: 3 Heurística violada: Consistency and Standards / Match Between System and the Real World**
- Problema: En las vistas de listas de activos (Sites y Equipments), el botón azul global en la esquina superior derecha está etiquetado como "Site detail" o "Equipment detail". Este etiquetado sugiere que llevará al detalle de un elemento seleccionado, cuando lo más probable es que su función principal sea agregar un nuevo activo. Esto es inconsistente con el estándar de UX de usar verbos de acción.
- Recomendación: Cambiar la etiqueta del botón por un texto que indique la acción de creación, como "+ New Site" o "+ New Equipment". Si su función es realmente ver el detalle, esta acción debe estar en la fila del activo o deshabilitada si no hay selección.

## PROBLEMA \#6: Uso de identificadores internos ("e1", "s1", "t2") en las tablas principales de activos y alertas.

- **Severidad: 3 Heurística violada: Recognition Rather Than Recall / Match Between System and the Real World**
- Problema: La tabla de Alerts utiliza IDs del sistema como e1 (Equipment), s1 (Site) y t2 (Tenant). Estos IDs no son significativos para el usuario, obligándolo a recordar o consultar constantemente su significado. Esta abstracción aumenta la carga cognitiva y reduce la velocidad de comprensión del estado del sistema.
- Recomendación: Reemplazar los IDs en las vistas de lista con los nombres reales de los activos (mostrar "Minimarket San Miguel" en lugar de s1, y el "Model" del equipo en lugar de e1).

## **PROBLEMA \#7: Las fechas y horas en los detalles de equipos se muestran en formato UTC/Z sin conversión a hora local.**

- **Severidad: 4 Heurística violada: Match Between System and the Real World**
- Problema: En la vista "Equipment detail", las fechas como 2025-09-21T14:10:00Z están en formato UTC. En un sistema de monitoreo, donde el tiempo es crítico, obligar al usuario a calcular la diferencia horaria manualmente para correlacionar eventos con la hora local es un error crítico que puede llevar a errores operacionales.
- Recomendación: Implementar la conversión automática de todas las marcas de tiempo a la zona horaria local del usuario y mostrarlas en un formato legible (ej. DD/MM/AAAA HH:MM:SS).

## **PROBLEMA \#8: Confusión visual entre campos editables y no editables en la sección de información de usuario.**

- **Severidad: 3 Heurística violada: Visibility of System Status / Aesthetic and Minimalist Design**
- Problema: En la sección "User information" (Admin), la información de solo lectura (ej. Email, Register Date, Plans) se presenta dentro de cajas de texto de color gris, que visualmente son demasiado similares a los campos editables (cajas blancas). Esto añade desorden visual y hace que el usuario se pregunte qué campos puede modificar y cuáles no.
- Recomendación: Los datos de sólo lectura deben mostrarse como texto plano (sin bordes ni sombreado de caja) para una clara diferenciación visual.

## **PROBLEMA \#9: Redundancia o falta de claridad en los filtros de la sección "My Service Requests".**

- **Severidad: 2 Heurística violada: Aesthetic and Minimalist Design / Flexibility and Efficiency of Use**
- Problema: En la sección "My Service Requests", los filtros están agrupados de forma redundante ("Filter by: ALL | Pending | Assigned | In progress | Done" y luego "ALL | Repair (Corrective) | Maintenance (Preventive)"). El doble uso de "ALL" es confuso. Además, el primer conjunto de filtros parece enfocarse en el Status, y el segundo en el Type, pero la repetición de "ALL" no es eficiente.
- Recomendación: Fusionar los filtros en un único conjunto que permita seleccionar una opción de Status Y una opción de Type, o unificar el botón "ALL" si es un reset general de ambos filtros.

**Respositorio de auditoria:** `https://docs.google.com/document/d/12K22DituAE1HPKc8xQM8qvzI5G8edJ3c5FYTELsxBZM/edit?usp=sharing`

---

## Proceso de Evaluacion para el grupo 1"

## Evaluación Heurística de Usabilidad y Diseño Inclusivo para la Aplicación: "AgroApp"

**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**

**CARRERA:** Ingeniería de Software

**CURSO:** Aplicaciones Web

**SECCIÓN:** 7380  

**PROFESORES:** Todos

**AUDITOR:** Ramirez Cabrera, Kenyi Efrain

**CLIENTE(S)	:**

	   **Bonifacio Jaramillo, Samuel Jesus**   

	   **Castro Pariona, Jefferson Ernesto**   

	   **Morales Sosa, Arnold Gabriel** 

	   **Romero Meza, Jhimy Pool**

	   **Seminario Castillo, Diego Vicente**

**SITE o APP A EVALUAR:** AgroApp

## TAREAS A EVALUAR:

El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Visualización y navegación en la página principal
2. Visualización del campo de Cultivo (galería, fichas, presentación de información)
3. Navegación por la sección de Cultivos (flujo, claridad de información, pasos a seguir)
4. Accesibilidad y claridad del menú lateral (ubicación, iconos, estructura)
5. Visualizacion de los atributos de los campos y cultivos (nombre, dimensiones, producto, estado, etc)
6. Diferenciación entre las secciones “Cultivos” y “Campos”
7. Visualización de detalles del campo (tareas, estado, producto)
8. Gestión de cultivos y sus campos (tareas, recordatorios)
9. Claridad de iconografía y etiquetas
10. Navegación lateral y localización de sección activa
11. Estructura y claridad del formulario de registros
12. Proceso de cambio de idioma
13. Personalización y curva de aprendizaje

## ESCALA DE SEVERIDAD:

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad

| Nivel | Descripción                                                                                                                                                                                    |
| :---: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | Problema superficial: puede ser fácilmente superador por el usuario ó ocurre con muy poco frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo.                  |
| 2     | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente reléase |
| 3     | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.                                |
| 4     | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.                              |

## TABLA RESUMEN:

| \#    | Problema                                                                                               | Escala de severidad | Heurística/Principio violada(o)                                     |
| :---: | :----------------------------------------------------------------------------------------------------- | :-----------------: | :------------------------------------------------------------------ |
| 1	    | Dificultad para identificar el contenido principal y navegar desde la página inicial.	                 | 3	               | Visibility of System Status / Aesthetic and Minimalist Design       |
| 2	    | La visualización del campo de Cultivo no es consistente entre galería, fichas y vista detallada.	     | 3	               | Consistency and Standards / Match Between System and the Real World |
| 3	    | El flujo dentro de la sección de Cultivos no guía al usuario en los pasos a seguir.                    | 3	               | User Control and Freedom / Recognition Rather Than Recall           | 
| 4	    | El menú lateral presenta baja claridad en su estructura e iconos poco representativos.	             | 2	               | Recognition Rather Than Recall / Aesthetic and Minimalist Design    |
| 5	    | Los atributos de campos y cultivos no están claramente organizados o priorizados.	                     | 3	               | Aesthetic and Minimalist Design / Visibility of System Status       |
| 6	    | Confusión entre las secciones “Cultivos” y “Campos”, sin una diferenciación conceptual o visual clara. | 3	               | Match Between System and the Real World / Consistency and Standards |
| 7	    | La vista de detalles del campo muestra información incompleta o poco jerarquizada.	                 | 3	               | Visibility of System Status / Aesthetic and Minimalist Design       |
| 8	    | El proceso de gestión de cultivos y tareas no es intuitivo, generando pérdida de control.	             | 3	               | User Control and Freedom / Flexibility and Efficiency of Use        |
| 9	    | La iconografía y etiquetas no son claras ni coherentes con su propósito.	                             | 2	               | Recognition Rather Than Recall / Consistency and Standards          |
| 10	| El usuario no puede identificar fácilmente qué sección del menú está activa.	                         | 2	               | Visibility of System Status                                         |
| 11	| El formulario de registros presenta desorden visual y campos sin jerarquía clara.	                     | 3	               | Aesthetic and Minimalist Design / Error Prevention                  |
| 12	| El proceso de cambio de idioma no es visible o requiere demasiados pasos.	                             | 2	               | Visibility of System Status / Flexibility and Efficiency of Use     |
| 13    | Falta de personalización y una curva de aprendizaje elevada para nuevos usuarios.	                     | 2	               | Flexibility and Efficiency of Use / Help and Documentation          |

## DESCRIPCIÓN DE PROBLEMAS:

## PROBLEMA #1: Dificultad para identificar el contenido principal y navegar desde la página inicial.

- Severidad: 3 — Heurística violada: Visibility of System Status / Aesthetic and Minimalist Design
- Problema: En la página principal, la información está distribuida de manera poco jerárquica, lo que dificulta identificar rápidamente el contenido más relevante. No existe un punto focal claro ni un orden visual que guíe la exploración inicial del usuario. Esto genera incertidumbre sobre qué acciones pueden realizarse desde esta vista.
- Recomendación: Organizar el contenido siguiendo una estructura clara de prioridades (ej. “Resumen del campo”, “Acciones rápidas”, “Alertas”). Incorporar títulos visibles, secciones delimitadas y un diseño que facilite la exploración inicial.

## PROBLEMA #2: La visualización del campo de Cultivo no es consistente entre galería, fichas y vista detallada.

- Severidad: 3 — Heurística violada: Consistency and Standards / Match Between System and the Real World
- Problema: Las vistas del Cultivo presentan variaciones en etiquetas, tamaños de tarjeta, iconografía y disposición del contenido. En la galería el Cultivo aparece con un estilo visual, mientras que en las fichas o vista detallada adopta otro, generando confusión y dificultando la continuidad visual.
- Recomendación: Unificar criterios de diseño: usar la misma estructura básica, iconografía, tipografía y orden de atributos en todas las vistas relacionadas al Cultivo.

## PROBLEMA #3: El flujo dentro de la sección de Cultivos no guía al usuario en los pasos a seguir.

- Severidad: 3 — Heurística violada: User Control and Freedom / Recognition Rather Than Recall
- Problema: La sección de Cultivos no ofrece una guía clara sobre qué debe hacerse primero (visualizar el campo, asignar tareas, seleccionar un cultivo, ver su detalle, etc.). El usuario debe recordar rutas previas y elementos relacionados, lo cual incrementa la carga cognitiva.
- Recomendación: Agregar breadcrumbs, indicadores de progreso o acciones guiadas (ej. “Ver cultivos”, “Seleccionar un campo”, “Asignar tarea”). Presentar una navegación más lineal o explicar mediante subtítulos qué representa cada sección.

## PROBLEMA #4: El menú lateral presenta baja claridad en su estructura e iconos poco representativos.

- Severidad: 2 — Heurística violada: Recognition Rather Than Recall / Aesthetic and Minimalist Design
- Problema: Los iconos del menú lateral no representan claramente la función de cada sección. Algunos iconos son genéricos y requieren que el usuario memorice su propósito. La estructura del menú tampoco facilita diferenciar secciones que son conceptualmente distintas.
- Recomendación: Actualizar iconografía para que represente directamente la función (ej. “Campos”, “Cultivos”, “Tareas”). Organizar el menú en categorías o grupos visuales para mejorar la escaneabilidad.

## PROBLEMA #5: Los atributos de campos y cultivos no están claramente organizados o priorizados.

- Severidad: 3 — Heurística violada: Aesthetic and Minimalist Design / Visibility of System Status
- Problema: Los atributos, como nombre del campo, dimensiones, estado del cultivo o características del producto, aparecen sin una jerarquía visual clara. Algunos datos críticos quedan en posiciones secundarias o con poca visibilidad, y datos menos relevantes aparecen más destacados.
- Recomendación: Crear una estructura estándar: encabezado para nombre, sección para atributos clave, subsección para información secundaria. Utilizar tipografías y colores que indiquen importancia.

## PROBLEMA #6: Confusión entre las secciones “Cultivos” y “Campos”.

- Severidad: 3 — Heurística violada: Match Between System and the Real World / Consistency and Standards
- Problema: Las secciones “Cultivos” y “Campos” presentan información que parece solaparse, generando confusión sobre cuál es la unidad principal que se está gestionando. No existe una distinción clara entre ambas categorías ni visual ni conceptual.
- Recomendación: Definir de manera explícita la diferencia entre un Campo y un Cultivo y reflejarlo en los textos, iconos, títulos y estructura de navegación.

## PROBLEMA #7: La vista de detalles del campo muestra información incompleta o poco jerarquizada.

- Severidad: 3 — Heurística violada: Visibility of System Status / Aesthetic and Minimalist Design
- Problema: La vista de detalles del campo combina tareas, estado del producto, información del cultivo y datos generales sin un orden claro. Esto dificulta que el usuario encuentre rápidamente lo que busca, como tareas pendientes o etapas críticas del cultivo.
- Recomendación: Separar la información en secciones: “Información del Campo”, “Estado del Cultivo”, “Tareas asociadas”, “Historial”. Utilizar encabezados y etiquetas visualmente claras.

## PROBLEMA #8: El proceso de gestión de cultivos y tareas no es intuitivo, generando pérdida de control.

- Severidad: 3 — Heurística violada: User Control and Freedom / Flexibility and Efficiency of Use
- Problema: Asignar tareas, crear recordatorios o gestionar el avance del cultivo requiere varios pasos no evidentes o difíciles de encontrar. El flujo no ofrece atajos ni una vista clara del estado actual.
- Recomendación: Simplificar el flujo: agregar botones directos como “+ Tarea”, “Añadir recordatorio”, y resaltar el estado actual del cultivo. Permitir acciones rápidas desde la vista principal.

## PROBLEMA #9: La iconografía y etiquetas no son claras ni coherentes con su propósito.

- Severidad: 2 — Heurística violada: Recognition Rather Than Recall / Consistency and Standards
- Problema: Muchas etiquetas no describen la acción real que ejecutan (ej. botones genéricos como “Details” o “Info”). Algunas iconografías no representan claramente su función, generando ambigüedad.
- Recomendación: Usar verbos de acción (ej. “Ver campo”, “Editar cultivo”, “Registrar tarea”) y elegir iconos universales relacionados con agricultura, edición, tareas, alertas y navegación.

## PROBLEMA #10: El usuario no puede identificar fácilmente qué sección del menú está activa.

- Severidad: 2 — Heurística violada: Visibility of System Status
- Problema: La sección activa del menú no presenta indicadores visuales fuertes. El contraste es insuficiente y no hay un borde resaltado o un marcador claro. El usuario debe detenerse a leer cada etiqueta para saber dónde se encuentra.
- Recomendación: Agregar indicadores claros: un borde lateral grueso, color de fondo más intenso o iconos resaltados cuando están activos.

## PROBLEMA #11: El formulario de registros presenta desorden visual y campos sin jerarquía clara.

- Severidad: 3 — Heurística violada: Aesthetic and Minimalist Design / Error Prevention
- Problema: Los formularios contienen campos sin orden lógico, sin separación entre categorías y sin ayudas visuales para evitar errores. Algunos campos obligatorios no están diferenciados y el usuario puede cometer errores fácilmente.
- Recomendación: Agrupar campos por categorías, usar títulos (“Datos del campo”, “Características del cultivo”), indicar claramente los campos obligatorios y validar entradas en tiempo real.

## PROBLEMA #12: El proceso de cambio de idioma no es visible o requiere demasiados pasos.

- Severidad: 2 — Heurística violada: Visibility of System Status / Flexibility and Efficiency of Use
- Problema: El cambio de idioma no está fácilmente accesible. Puede estar oculto en un menú profundo o no ser evidente para usuarios nuevos. Requiere varios clics o pasos innecesarios.
- Recomendación: Colocar el selector de idioma en una ubicación visible (preferiblemente en la parte superior derecha), usar iconos de banderas y reducir el proceso a un solo clic.

## PROBLEMA #13: Falta de personalización y una curva de aprendizaje elevada para nuevos usuarios.

- Severidad: 2 — Heurística violada: Flexibility and Efficiency of Use / Help and Documentation
- Problema: La plataforma no ofrece recomendaciones, guías iniciales o personalización de vistas. Los usuarios nuevos deben aprender la navegación por ensayo y error, lo cual incrementa la curva de aprendizaje y reduce la eficiencia.
- Recomendación: Agregar un onboarding inicial, brindar tooltips explicativos y permitir que el usuario configure vistas rápidas o favoritos.

**Respositorio de auditoria:** `https://docs.google.com/document/d/1yUM-z9TAOwkcqBh12h8XKnBpV6gf2EIMYIysLJnMgsc/edit?usp=sharing`

# Conclusiones

## Conclusiones y recomendaciones

- El desarrollo del backend permitió establecer una base sólida para garantizar el funcionamiento estable y seguro de la plataforma IceTrack. Gracias a la implementación de servicios bien estructurados y una arquitectura organizada, se logró asegurar la comunicación eficiente entre el frontend y los registros almacenados en el servidor.
- La API creada permitió gestionar de manera centralizada la información de los equipos de refrigeración, asegurando que los datos enviados y recibidos por los usuarios se mantengan consistentes, actualizados y accesibles en tiempo real. Esto contribuyó a mejorar la confiabilidad del sistema y su capacidad para escalar en futuros módulos y nuevas funcionalidades.
- La integración de controladores, modelos y rutas permitió manejar de forma ordenada cada funcionalidad del sistema. Este enfoque de diseño facilita la mantenibilidad del código y asegura que nuevas implementaciones o actualizaciones puedan realizarse sin comprometer la estabilidad general de la plataforma.
- El trabajo con bases de datos permitió estructurar adecuadamente la información de los equipos monitoreados, lo que contribuyó a garantizar integridad, seguridad y disponibilidad de los datos. La correcta definición de entidades y relaciones permitió optimizar consultas, mejorar tiempos de respuesta y garantizar un acceso eficiente a la información clave.
- En el entorno colaborativo, la organización del backend mediante ramas, commits descriptivos y revisiones en GitHub permitió mantener un flujo de trabajo ordenado. Cada integrante aportó código claro, documentado y funcional, lo que facilitó la integración continua y la resolución rápida de incidencias.
- Se recomienda continuar optimizando la arquitectura del backend mediante la implementación de patrones de diseño que faciliten la escalabilidad, como el uso de servicios independientes o microservicios, considerando el crecimiento futuro de IceTrack.
- Es importante añadir pruebas unitarias y pruebas de integración que aseguren que cada funcionalidad del backend responda correctamente ante diferentes escenarios, reduciendo errores y fortaleciendo la calidad del producto final.
- Se sugiere mejorar los mecanismos de autenticación y autorización mediante tokens más seguros y control de accesos avanzado, con el fin de garantizar que solo usuarios autorizados puedan acceder a los servicios sensibles de la plataforma.
- Para garantizar un rendimiento óptimo, se recomienda implementar técnicas de caché, balanceo de carga o manejo eficiente de solicitudes en caso de alto tráfico, especialmente cuando IceTrack escale a más usuarios o clientes.
- Se debe documentar continuamente los endpoints, modelos y procesos internos a través de herramientas como Swagger, facilitando el mantenimiento del backend y permitiendo que futuros desarrolladores comprendan rápidamente la estructura del sistema.

