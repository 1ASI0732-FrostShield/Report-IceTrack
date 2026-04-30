<div align = "center">
 <h1>Universidad Peruana de Ciencias Aplicadas</h1>
 <img style="height: 200px" src="assets/chapter01/upc.png">
  <h2>Carrera: Ingeniería de Software</h2>
  <h2>Periodo: 2026-10</h2>
<br>
  <h2>Curso: Diseño de Experimentos de Ingeniería de Software</h2>
  <h2>Codigo del Curso: 1ASI0732</h2>
  <h2>NRC: 12316</h2>
  <h2>Profesor: Julio Manuel Noriega Melendez</h2>
<br>
 <h1>Informe del Trabajo Final</h1>
  <h2>Startup: Frostshield </h2>
  <h2>Producto: IceTrack </h2>
<br>
  <h2>Integrantes</h2>
 
<div align="center">
 
| <div style="width:500px">Alumno</div> | <div style="width:200px">Código</div> |
| :-----------------------------------: | :-----------------------------------: |
|  Gonzales Alvarado, Javier Sebastian  |           U202312966                  |
|  Gordon Salas, Gabriel Fernando       | U20221E229                            |
|  Guillen Galindo, Julio Adolfo    	|              u20241a352               |
|  Jiménez Guerra, Gianmarco Fabian     |     u202123843                        |
|  Melgarejo Gomez, Marcia Victoria     |U20231C505                             |
|  Quijada Magro, Jeremy Alexander      |              u202219657               |

</div>

<br>

   <h3>Abril 2026</h3>

</div>

## Registro de Versiones del Informe

<div align="center">
 
| Versión | Fecha      | Autor             | Descripción de modificación                        	|
| :-----: | :--------: | :---------------: | :----------------------------------------------------- |
| 1.1     | 03/12/2025 | Julio Guillen     | Desarrollo BackEnd para Assets-Management y Monitoring |
| 1.2     | 04/12/2025 | Jeremy Quijada    | Refactorizacion de la aplicación                       |

</div>

## Project Report Collaboration Insights

- **URL de la organización del proyecto:** 
  https://github.com/1ASI0730-2520-7452-G1-FrostShield
  <br>
- **URL del repositorio del reporte:** 
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/Report
  <br>
  
- **URL del repositorio de la Landing Page:**
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page
  <br>
- **URL del repositorio del Frontend:** 
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack-Frontend
  <br>
- **URL del repositorio del Backend:** 
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack-Platform

Durante la fase de preparación del informe, se llevaron a cabo las siguientes actividades:

**Avance 1:** Las tareas asignadas a la TB1 han sido finalizadas y se encuentran correctamente documentadas en el repositorio de GitHub:

- Se redactaron y crearon los contenidos asignados a cada miembro utilizando formato Markdown, y se realizaron "Conventional Commits" para documentar el avance en el repositorio.
- Se generaron los recursos necesarios y se añadieron las imágenes al repositorio en la carpeta "assets" correspondiente a cada rama del informe.
- Se organizaron reuniones para coordinar el progreso de los componentes del informe y del Sprint 1, que estuvo enfocado en el desarrollo de la Landing Page.
  
![InsightsTB1](assets/chapter01/Insights-TB1.png)

![NetworkGraph](assets/chapter01/NetworkGraph-TB1.png)

## Contenido

- [Student Outcome](#student-outcome)

- [Capítulo I: Introducción](#c1)
    - [1.1. Startup Profile](#11-startup-profile)
        - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
        - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
    - [1.2. Solution Profile](#12-solution-profile)
        - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problematica)
        - [1.2.2 Lean UX Process](#122-lean-ux-process)
            - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
            - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumption)
            - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
            - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
    - [1.3. Segmentos objetivo](#13-segmentos-objetivos)

- [Capítulo II: Requirements Elicitation & Analysis](#c2)
    - [2.1. Competidores](#21-competidores)
        - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
        - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
    - [2.2. Entrevistas](#22-entrevistas)
        - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
        - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
        - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
    - [2.3. Needfinding](#23-needfinding)
        - [2.3.1. User Personas](#231-user-personas)
        - [2.3.2. User Task Matrix](#232-user-task-matrix)
        - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
        - [2.3.4. Empathy Mapping](#234-empathy-mapping)
    - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
    - [2.5. Ubiquitous Language](#25-ubiquitous-language)

- [Capítulo III: Requirements Specification](#c3)
    - [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
    - [3.2. User Stories](#32-user-stories)
    - [3.3. Impact Mapping](#33-impact-mapping)
    - [3.4. Product Backlog](#34-product-backlog)

- [Capítulo IV: Product Design](#c4)
    - [4.1. Style Guidelines](#41-style-guidelines)
        - [4.1.1. General Style Guidelines](#411-general-style-guidelines)
        - [4.1.2. Web Style Guidelines](#412-web-style-guidelines)
    - [4.2. Information Architecture](#42-information-architecture)
        - [4.2.1. Organization Systems](#421-organization-systems)
        - [4.2.2. Labeling Systems](#422-labeling-systems)
        - [4.2.3. SEO Tags and Meta Tags](#423-seo-tags-and-meta-tags)
        - [4.2.4. Searching Systems](#424-searching-systems)
        - [4.2.5. Navigation Systems](#425-navigation-systems)
    - [4.3. Landing Page UI Design](#43-landing-page-ui-design)
        - [4.3.1. Landing Page Wireframe](#431-landing-page-wireframe)
        - [4.3.2. Landing Page Mock-up](#432-landing-page-mock-up)
    - [4.4. Web Applications UX/UI Design](#44-web-applications-uxui-design)
        - [4.4.1. Web Applications Wireframes](#441-web-applications-wireframes)
        - [4.4.2. Web Applications Wireflow Diagrams](#442-web-applications-wireflow-diagrams)
        - [4.4.3. Web Applications Mock-ups](#443-web-applications-mock-ups)
        - [4.4.4. Web Applications User Flow Diagrams](#444-web-applications-user-flow-diagrams)
    - [4.5. Web Applications Prototyping](#45-web-applications-prototyping)
    - [4.6. Domain-Driven Software Architecture](#46-domain-driven-software-architecture)
        - [4.6.1. Design-Level EventStorming](#461-design-level-eventstorming)
        - [4.6.2. Software Architecture Context Diagram](#462-software-architecture-context-diagram)
        - [4.6.3. Software Architecture Container Diagrams](#463-software-architecture-container-diagrams)
        - [4.6.4. Software Architecture Components Diagrams](#464-software-architecture-components-diagrams)
    - [4.7. Software Object-Oriented Design](#47-software-object-oriented-design)
        - [4.7.1. Class Diagrams](#471-class-diagrams)
    - [4.8. Database Design](#48-database-design)
        - [4.8.1. Database Diagrams](#481-database-diagrams)

- [Capítulo V: Product Implementation, Validation & Deployment](#c5)
    - [5.1. Software Configuration Management](#51-software-configuration-management)
        - [5.1.1. Software Development Environment Configuration](#511-software-development-environment-configuration)
        - [5.1.2. Source Code Management](#512-source-code-management)
        - [5.1.3. Source Code Style Guide & Conventions](#513-source-code-style-guide--conventions)
        - [5.1.4. Software Deployment Configuration](#514-software-deployment-configuration)
    - [5.2. Landing Page, Services & Applications Implementation](#52-landing-page-services--applications-implementation)
        - [5.2.1. Sprint 1](#521-sprint-1)
            - [5.2.1.1. Sprint Planning 1](#5211-sprint-planning-1)
            - [5.2.1.2. Aspect Leaders and Collaborators](#5212-aspect-leaders-and-collaborators)
            - [5.2.1.3. Sprint Backlog 1](#5213-sprint-backlog-1)
            - [5.2.1.4. Development Evidence for Sprint Review](#5214-development-evidence-for-sprint-review)
            - [5.2.1.5. Execution Evidence for Sprint Review](#5215-execution-evidence-for-sprint-review)
            - [5.2.1.6. Services Documentation Evidence for Sprint Review](#5216-services-documentation-evidence-for-sprint-review)
            - [5.2.1.7. Software Deployment Evidence for Sprint Review](#5217-software-deployment-evidence-for-sprint-review)
            - [5.2.1.8. Team Collaboration Insights during Sprint](#5218-team-collaboration-insights-during-sprint)
        - [5.2.2. Sprint 2](#522-sprint-2)
            - [5.2.2.1. Sprint Planning 2](#5221-sprint-planning-2)
            - [5.2.2.2. Aspect Leaders and Collaborators](#5222-aspect-leaders-and-collaborators)
            - [5.2.2.3. Sprint Backlog 2](#5223-sprint-backlog-2)
            - [5.2.2.4. Development Evidence for Sprint Review](#5224-development-evidence-for-sprint-review)
            - [5.2.2.5. Execution Evidence for Sprint Review](#5225-execution-evidence-for-sprint-review)
            - [5.2.2.6. Services Documentation Evidence for Sprint Review](#5226-services-documentation-evidence-for-sprint-review)
            - [5.2.2.7. Software Deployment Evidence for Sprint Review](#5227-software-deployment-evidence-for-sprint-review)
            - [5.2.2.8. Team Collaboration Insights during Sprint](#5228-team-collaboration-insights-during-sprint)
        - [5.2.3. Sprint 3](#523-sprint-3)
            - [5.2.3.1. Sprint Planning 3](#5231-sprint-planning-3)
            - [5.2.3.2. Aspect Leaders and Collaborators](#5232-aspect-leaders-and-collaborators)
            - [5.2.3.3. Sprint Backlog 3](#5233-sprint-backlog-3)
            - [5.2.3.4. Development Evidence for Sprint Review](#5234-development-evidence-for-sprint-review)
            - [5.2.3.5. Execution Evidence for Sprint Review](#5235-execution-evidence-for-sprint-review)
            - [5.2.3.6. Services Documentation Evidence for Sprint Review](#5236-services-documentation-evidence-for-sprint-review)
            - [5.2.3.7. Software Deployment Evidence for Sprint Review](#5237-software-deployment-evidence-for-sprint-review)
            - [5.2.3.8. Team Collaboration Insights during Sprint](#5238-team-collaboration-insights-during-sprint)
        - [5.2.4. Sprint 4](#524-sprint-4)
            - [5.2.4.1. Sprint Planning 4](#5241-sprint-planning-4)
            - [5.2.4.2. Aspect Leaders and Collaborators](#5232-aspect-leaders-and-collaborators)
            - [5.2.4.3. Sprint Backlog 4](#5243-sprint-backlog-4)
            - [5.2.4.4. Development Evidence for Sprint Review](#5244-development-evidence-for-sprint-review)
            - [5.2.4.5. Execution Evidence for Sprint Review](#5245-execution-evidence-for-sprint-review)
            - [5.2.4.6. Services Documentation Evidence for Sprint Review](#5246-services-documentation-evidence-for-sprint-review)
            - [5.2.4.7. Software Deployment Evidence for Sprint Review](#5247-software-deployment-evidence-for-sprint-review)
            - [5.2.4.8. Team Collaboration Insights during Sprint](#5248-team-collaboration-insights-during-sprint)
    - [5.3. Validation Interviews](#53-validation-interviews)
        - [5.3.1. Diseño de Entrevistas](#531-diseño-de-entrevistas)
        - [5.3.2. Registro de Entrevistas](#532-registro-de-entrevistas)
        - [5.3.3. Evaluaciones según heurísticas](#533-evaluaciones-según-heurísticas)
    - [5.4. Video About-the-Product](#54-video-about-the-product)

- [Conclusiones](#conclusiones)
- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
- [Video About-the-Team](#video-about-the-team)
- [Bibliografía](#bibliografía)
- [Anexos](#anexos)

## Student Outcome
El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 5**

**Criterio**: *La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.*

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5.

| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| Trabaja en equipo para proporcionar liderazgo en forma conjunta | <ul><li><b>Quijada Magro, Jeremy Alexander:</b> Lideró la arquitectura del sistema y la fase de QA para validación de variables de monitoreo.</li><li><b>Guillen Galindo, Julio Adolfo:</b> Lideró el desarrollo del Backend API y la gestión de la base de datos distribuida.</li><li><b>Gonzales Alvarado, Javier:</b> Lideró el diseño de la Landing Page y la estrategia de comunicación del producto.</li><li><b>Jiménez Guerra, Gianmarco:</b> Lideró el análisis de requerimientos y la validación de escenarios de usuario.</li><li><b>Melgarejo Gomez, Marcia Victoria:</b> Lideró el diseño visual (UI) y la creación de prototipos de alta fidelidad.</li><li><b>Gordon Salas, Gabriel Fernando:</b> Lideró la planificación de Sprints y la organización del equipo mediante el Lean UX Canvas.</li></ul> | <ul><li>El equipo distribuyó el liderazgo de forma equitativa según la especialidad de cada capítulo, logrando la integración exitosa del proyecto.</li></ul> |
| Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos. | <ul><li><b>Quijada Magro, Jeremy Alexander:</b> Desarrolló el prototipo funcional y configuró los entornos de despliegue continuo.</li><li><b>Guillen Galindo, Julio Adolfo:</b> Implementó los servicios de seguridad JWT y la lógica de negocio del servidor.</li><li><b>Gonzales Alvarado, Javier:</b> Elaboró la documentación técnica y el manual de estilo de la aplicación.</li><li><b>Jiménez Guerra, Gianmarco:</b> Definió los User Personas y realizó el mapeo de experiencias (As-Is Scenario).</li><li><b>Melgarejo Gomez, Marcia Victoria:</b> Creó los flujos de usuario y garantizó la accesibilidad en la interfaz móvil.</li><li><b>Gordon Salas, Gabriel Fernando:</b> Gestionó el Backlog y supervisó el cumplimiento de los hitos académicos en los plazos establecidos.</li></ul> | <ul><li>Se estableció un flujo de trabajo ágil que permitió cumplir con el 100% de los objetivos planteados para el TB1 mediante el uso de herramientas colaborativas.</li></ul> |

## 5.4. Video About-the-Product

En esta parte, el equipo ofrece una síntesis de los puntos más importantes de IceTrack. El contenido audiovisual describe detalladamente las funciones principales de la aplicación, mostrando cómo cada una fue creada para atender las necesidades de los sistemas de refrigeración, ya sea en entornos domésticos o comerciales.

El video incluye demostraciones visuales del uso de la app, mostrando pasos esenciales como el monitoreo de temperatura y consumo energético, alertas de fallos, historial de rendimiento y reportes generales sobre los equipos registrados.

La narración guía al espectador por toda la experiencia de uso, mientras que testimonios reales aportan credibilidad al compartir cómo la aplicación ha facilitado la supervisión de sistemas de refrigeración, tanto para técnicos como para usuarios sin experiencia. Estos relatos destacan la facilidad de uso y la mejora en la eficiencia y confiabilidad de los equipos.

En conjunto, el video no solo presenta el producto, sino que lo posiciona como una solución digital efectiva para apoyar el mantenimiento y control responsable de la refrigeración, demostrando su utilidad, su usabilidad y su impacto positivo.

**Video Explicativo**

<p align="center">
    <img src="assets/chapter05/about_product.png" alt="about_product"/>    
</p>

URL de la Versión Publicada

- **Link de OneDrive:** https://www.youtube.com/watch?v=BIWXxVJlkKk

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

# Bibliografía

- Axios. (s.f.). *Axios: Promise based HTTP client for the browser and node.js*. https://axios-http.com/docs/intro

- Conventional Commits. (s.f.). *Conventional commits*. https://www.conventionalcommits.org/

- Google. (s.f.). *Google HTML/CSS style guide*. https://google.github.io/styleguide/htmlcssguide.html

- PrimeVue. (s.f.). *PrimeVue: The most complete UI component library for Vue.js*. https://primevue.org

- REST API Tutorial. (s.f.). *What is REST?*. https://www.restapitutorial.com/introduction/whatisrest

- RESTfulAPI.net. (s.f.). *REST API tutorial*. https://restfulapi.net

- W3Schools. (s.f.). *HTML style guide and coding conventions*. https://www.w3schools.com/html/html5_syntax.asp

# Anexos

## Recursos y enlaces del proyecto
  
- **URL de la organización del proyecto:** <br>
  https://github.com/1ASI0730-2520-7452-G1-FrostShield
  
- **URL del repositorio del reporte:** <br>
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/Report
  
- **URL del repositorio de la Landing Page:** <br>
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack---Landing-Page
  
- **URL del repositorio del Frontend:** <br>
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack-Frontend
  
- **URL del repositorio del Backend:** <br>
  https://github.com/1ASI0730-2520-7452-G1-FrostShield/IceTrack-Platform
  
- **URL del Landing Page desplegado:** <br>
  https://1asi0730-2520-7452-g1-frostshield.github.io/IceTrack---Landing-Page/
  
- **URL del Frontend desplegado:** <br>
  https://ice-track-frontend.vercel.app/
  
- **URL del Backend desplegado:** <br>
  https://icetrack-platform.onrender.com
  
- **Video About-The-Team:** <br>
  - YouTube: https://www.youtube.com/watch?v=Au_UI13KXkM
    
- **Video About-The-Product:**
  - YouTube: https://www.youtube.com/watch?v=BIWXxVJlkKk
