# Capítulo IV: Product Design

## 4.1. Style Guidelines
El diseño del logo de IceTrack busca transmitir los conceptos de protección, tecnología y monitoreo constante. Se eligió como elemento central un escudo estilizado con un copo de nieve integrado, simbolizando la protección de la cadena de frío. El escudo representa confianza y seguridad, mientras que el copo de nieve refleja el enfoque en la refrigeración. De manera complementaria, las líneas suaves y geométricas refuerzan la idea de precisión, estabilidad y eficiencia tecnológica.

### 4.1.1. General Style Guidelines
- Branding:
(En proceso...)

- Typography:
La tipografía seleccionada es Roboto Serif, por su claridad, legibilidad y llamativa, ideal para interfaces digitales enfocadas en datos técnicos. Para el cuerpo de texto, se utiliza Inter 14px con un interlineado de 1.5, garantizando una lectura fluida. Los tamaños se adaptan en contexto web según la jerarquía: títulos, subtítulos y párrafos.
   - Escala:
    <div align="center">
      <img src="assets/chapter01/GSG_Escala.png" alt="escala" width="250" height="200">
    </div>
    
   - Weights:
    <div align="center">
      <img src="assets/chapter01/GSG_Weights.png" alt="weights" width="150" height="250">
    </div>
    
   - Nomenclatura:
    <div align="center">
      <img src="assets/chapter01/GSG_Nomenclatura.png" alt="nomenclatura" width="250" height="200">
    </div>
    
   - Example:
    <div align="center">
      <img src="assets/chapter01/GSG_Example.png" alt="example" width="500" height="1000">
    </div>
  
- Colors:
La paleta de colores de IceTrack prioriza la tecnología, frescura y acción. El celeste transmite frescura, usado para botones y acentos principales. El rojo, asociado con la energía y acción. Este color incrementa la sensación de emergencia, siendo ideal para captar la atención de manera inmediata. Gris oscuro/azulado (Deep Navy): aporta seriedad y profesionalismo, usado en textos y fondos secundarios. El gris claro aporta seriedad, usado en fondos. Por ultimo, el azul oscuro transmite estabilidad y tecnología. Es el color base de botones o avisoos.

- Spacing:
El espaciado está diseñado para ofrecer una experiencia clara y ordenada, facilitando la lectura de datos técnicos y alertas:
  - Entre secciones principales: mínimo 20px para marcar el cambio de contexto.
  - Entre encabezados y párrafos: 16px para reforzar jerarquía visual.
  - Entre párrafos consecutivos: 14px para mantener continuidad y evitar bloques densos.
  - Espaciado de botones e inputs: mínimo 10px entre elementos para garantizar usabilidad.

- Tono de comunicación:
IceTrack transmite profesionalismo, confianza y proactividad, claves para un sistema que protege inventarios y garantiza la continuidad operativa:
  - Profesional y técnico, de modo que sea comprensible para empresas, técnicos y proveedores.
  - Preventivo y confiable, orientado a la acción rápida sin generar alarma innecesaria.
  - Empático y cercano, resaltando que IceTrack está diseñado para apoyar y facilitar el trabajo, no para complicarlo.

- Lenguaje aplicado:
  - Claro y directo, evitando tecnicismos complejos cuando no son necesarios.
  - Orientado a la acción, con instrucciones breves y fáciles de seguir.
  - Consistente en terminología técnica, garantizando coherencia en alertas, reportes y documentación.

### 4.1.2. Web Style Guidelines
Elegimos la paleta basada en azules, rojo blanco y negro, porque queremos representar los valores de tecnología, confianza y alerta crítica. El azul oscuro transmite estabilidad y profesionalismo, siendo el color principal de fondos y tipografías. El azul claro simboliza frescura, innovación y eficiencia, usado en botones y elementos interactivos. El rojo se reserva para alertas y notificaciones, comunicando de manera inmediata fallas o eventos críticos en los equipos de refrigeración.

El uso balanceado de estos tonos asegura que la información clave sea rápidamente perceptible sin perder sobriedad visual. Los contrastes se aplican estratégicamente para mantener un diseño ordenado, moderno y fácil de interpretar en cualquier dispositivo.

En cuanto a la tipografía, dado que IceTrack se orienta a la gestión técnica y empresarial, optamos por una fuente clara y contemporánea, como el Inter, que refuerza la legibilidad de dashboards y reportes. Los tamaños son medianos a grandes para asegurar claridad en datos críticos, mientras que los títulos y botones aplican variaciones de peso y tamaño para resaltar lo más importante en cada sección.

  <div align="center">
    <img src="assets/chapter01/WSG_Colors.png" alt="colors.png" width="250" height="500">
  </div>

- Tipografía:
Se respetará la relación tipográfica establecida en los General Style Guidelines.

- Responsive Design Standards:
IceTrack está diseñado como una aplicación mobile-first, adaptándose fluidamente a distintos dispositivos:

  - Mobile (360px – 768px)
    - Navegación tipo hamburguesa.
    - Cards apiladas en columna.
    - Botones grandes y legibles.

  - Tablet (769px – 1024px)
    - Layout en 2 columnas.
    - Menú lateral colapsable.

  - Desktop (1025px en adelante)
    - Menú principal siempre visible.
    - Layout de 3 columnas en dashboards y secciones de métricas.

- Interactivity
  - Botones:
    - Bordes redondeados en 12px.
    - Hover: cambio de fondo a azul claro o sombra suave.
    - Feedback claro al una animación sutil.

  - Transiciones y animaciones:
    - Duración: 200–300ms.
    - Curva: ease-in-out.

- Accessibility
  - Todo ícono debe tener alternativa textual (aria-label o alt).
  - Navegación totalmente compatible con teclado (Tab, Enter, Esc).
  - Fuente mínima: 16px para garantizar legibilidad.
  - Colores con contraste suficiente para cumplir con WCAG AA.

- UI Consistency
  - Iconografía uniforme, estilo outline con grosor consistente.
  - Botones y formularios con la misma geometría y espaciado.
  - Uso consistente de colores: azul para acciones, rojo solo para alertas.
  - Estándar de espaciado basado en múltiplos de 8px para mantener ritmo visual.

## 4.2. Information Architecture

### 4.2.1. Organization Systems
Se utilizaran diversos métodos para organizar la información según su relevancia, y su presentación visual se ha realizado de las siguientes maneras:

- Organización Jerárquica: Se usara en el dashboard principal, donde se prioriza mostrar primero las alertas críticas, luego los indicadores de consumo energético, y en reportes históricos.

- Organización Secuencial: En los flujos de interacción, como el registro de equipos, creación de solicitudes de servicio o configuración de alertas de mantenimiento.

- Organización Matricial: Para la comparación de datos energéticos y desempeño de equipos en los sistemas.

### 4.2.2. Labeling Systems
En IceTrack, el sistema de etiquetado ha sido diseñado para maximizar la claridad y reducir la carga cognitiva de los usuarios. Todas las etiquetas en la navegación, en los reportes o en la gestión de equipos, priorizan la simplicidad, la consistencia semántica y un lenguaje directo, profesional y fácil de comprender, sin sacrificar precisión técnica.

- Principios clave del sistema de etiquetado:
  - Las etiquetas evitarán tecnicismos innecesarios y ambigüedades. Se emplearán términos comunes que puedan ser entendidos tanto por empresarios como por técnicos.
  - Un mismo concepto siempre se representará con la misma palabra en todos los entornos (web, app móvil, correos de notificación).
  - Las etiquetas se limitarán a 1–3 palabras, descriptivas y directas.
  - Las etiquetas más críticas tendrán un mayor peso visual en la jerarquía tipográfica definida en la guía de estilo.

- Etiquetas principales por área
  - Navegación global: Inicio, Equipos, Servicios, Reportes, Alertas, Administración, Ayuda
  - Landing Page: Bienvenido a IceTrack, Soluciones, Funcionalidades, Casos de uso, Contáctanos
  - Gestión de equipos: Añadir equipo, Control remoto, Ajustar temperatura, Historial
  - Servicios de mantenimiento:, Solicitudes, Progreso, Confirmación, Historial
  - Reportes y métricas:, Consumo, Comparar, Descargar, Desempeño técnico

- Acciones del usuario Crear cuenta, Iniciar sesión, Solicitar servicio, Ver reporte, Configurar alerta, Descargar PDF, Cerrar sesión

- Asociaciones entre etiquetas: “Equipo crítico”, “Alerta preventiva”, “Reporte generado”

### 4.2.3. SEO Tags and Meta Tags
- Landing Page
  - Title: Gestión inteligente de equipos de refrigeración.
  - Meta Description: Optimiza la gestión de tu cadena de frío con monitoreo en tiempo real, alertas automáticas y mantenimiento predictivo, protegiendo tu inventario y reduciendo pérdidas.
  - Meta Keywords: gestión de refrigeración, mantenimiento predictivo, monitoreo en tiempo real, cadena de frío, eficiencia energética, equipos de refrigeración
  - Meta Author: Frostshield 

- Web Application:
  - Title: Monitoreo y gestión de tus equipos de refrigeración
  - Meta Description: Supervisa el estado de tus equipos, recibe alertas inmediatas y gestiona servicios de mantenimiento desde una sola plataforma.
  - Meta Keywords: monitoreo de refrigeración, gestión de equipos, alertas preventivas, mantenimiento en línea, reportes energéticos, técnicos de refrigeración
  - Meta Author: Frostshield 

### 4.2.4. Searching Systems
Las decisiones de búsqueda en IceTrack están orientadas a garantizar que los usuarios —empresarios, técnicos y proveedores— encuentren rápidamente la información crítica de sus equipos y servicios, sin sentirse abrumados por grandes volúmenes de datos.

- Opciones de Búsqueda
  - Barra de búsqueda
    - Permite ingresar términos específicos como nombre del equipo, tipo de servicio o estado del equipo.
    - Los resultados se muestran de forma instantánea conforme el usuario escribe.
  
  - Categorías
    - Congeladoras
    - Refrigeradores
    - Equipos de frío industrial
    - Mantenimiento preventivo
    - Alertas de fallas
    - Historial de consumo
  
  - Etiquetas populares
    - Mantenimiento programado
    - Alerta crítica
    - Servicio completado

- Filtros disponibles
  - Por tipo de equipo: Congeladoras o refrigeradores.
  - Por estado del equipo: Activo, en reparación, necesita mantenimiento.
  - Por fecha de última revisión: Últimos 7 días, últimos 30 días.
  - Por consumo energético: Rango mínimo–máximo según eficiencia.

- Apariencia de los datos después de la búsqueda
  - Listados de resultados: Incluyen nombre del equipo, estado, próxima fecha de mantenimiento y consumo energético.
  - Resumen y descripción: Cada resultado presenta un historial de mantenimiento o alertas recientes.
  - Ordenación y filtros aplicados: El usuario puede ordenar por relevancia, estado del equipo, consumo energético. Los filtros activos se muestran claramente en la parte superior.
  - Revisiones y comentarios: Cada resultado puede incluir reseñas o comentarios de técnicos/clientes sobre el desempeño y la calidad del servicio.

### 4.2.5. Navigation Systems
La estructura de navegación en IceTrack está diseñada para ofrecer una experiencia de usuario fluida, asegurando acceso rápido a funcionalidades críticas y manteniendo coherencia visual con la identidad de la marca.

- Páginas principales
  - Inicio: Dashboard con estado general de equipos y alertas críticas.
  - Funcionalidades: Descripción de herramientas clave como monitoreo en tiempo real, alertas automáticas y reportes.
  - Beneficios: Explicación de ventajas competitivas (ahorro energético, reducción de pérdidas, eficiencia operativa).
  - Nosotros: Información sobre la misión, visión y el equipo de IceTrack.
  - Contacto: Formulario de contacto y datos de soporte.

- Opciones de usuario
  - Inicias Sesion: Acceso para usuarios registrados.
  - Registrarme: Registro de nuevos clientes, técnicos y proveedores.
  - Perfil: Configuración y gestión de información personal o empresarial.
  - Cerrar sesión: Salida segura de la cuenta.

- Búsqueda y navegación
  - Barra de búsqueda: Disponible en todas las páginas para localizar equipos, servicios o reportes.
  - Categorías: Filtrado por tipo de equipo o tipo de servicio.
  - Explorar: Navegación rápida hacia módulos principales (Equipos, Servicios, Reportes, Administración).

- Branding e identidad
 - El logo y nombre IceTrack estarán visibles en la esquina superior izquierda de todas las vistas, asegurando coherencia de marca.
 - Los colores y tipografía seguirán los lineamientos definidos en la guía de estilo, reforzando la identidad visual y la confianza del usuario.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe
El wireframe del landing page de IceTrack se diseñó para guiar la creación de una interfaz clara e intuitiva. Este esquema visual, enfocado en la usabilidad y el flujo de información, define la estructura de cada sección:

**Header:** Contiene el logo de IceTrack y una navegación simple que facilita el acceso a las diferentes secciones de la página.

**Hero Section:** Muestra la propuesta de valor de forma impactante. Es la primera impresión del usuario y comunica de inmediato el valor principal de la solución.

**Beneficios:** Detalla los puntos clave que los clientes ganarán al usar la aplicación, explicando cómo IceTrack resuelve sus problemas específicos.

**Sobre Nosotros:** Presenta la misión y visión de la empresa, construyendo confianza y conectando con el usuario a través de los valores de la marca.

**Testimonios:** Incluye el feedback de clientes satisfechos, sirviendo como prueba social para validar la efectividad y calidad del servicio.

**Contacto (Formulario):** Ofrece un formulario sencillo para que los usuarios puedan solicitar información o una demostración, facilitando la conversión.

**Footer:** Contiene información legal, enlaces a redes sociales y datos de contacto, ofreciendo un cierre profesional y completo.

El objetivo principal de este wireframe es asegurar que el diseño final sea lógico, atractivo y, sobre todo, que guíe al usuario hacia una acción clara, como registrarse o contactar a la empresa.

<figure style="page-break-inside: avoid; text-align: center;">
	<div align="center">
    	<img src="assets/chapter04/LandingPageWireframe.png" height="50%">
  	</div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Wireframe del Landing Page.
  </figcaption>
</figure>

### 4.3.2. Landing Page Mock-up

Los mockups del landing page de IceTrack elevan la estructura del wireframe a un nivel visual y estético. Aquí, el enfoque ya no es solo la funcionalidad, sino también el diseño, los colores, la tipografía y las imágenes, con el objetivo de crear una experiencia de usuario atractiva y profesional.

**Inicio**
Presenta la propuesta de valor principal con una imagen atractiva y un texto impactante, capturando la atención del visitante de inmediato.

<figure style="page-break-inside: avoid; text-align: center;">
  <img src="assets/chapter04/LPMockupInicio.png"
       alt="Landing Page Mockup"
       style="max-width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Inicio.
  </figcaption>
</figure>

---

**Beneficios**
Usa íconos personalizados y un diseño limpio para destacar las ventajas clave de la app, facilitando la lectura y comprensión.

<figure style="page-break-inside: avoid; text-align: center;">
  <img src="assets/chapter04/LPMockupBeneficios.png"
       alt="Landing Page Mockup 2"
       style="max-width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 2:</strong> Beneficios.
  </figcaption>
</figure>

---

**Sobre Nosotros**
Comunica la misión y visión de la empresa con un estilo visual que inspira confianza y conecta con los valores del usuario.

<figure style="page-break-inside: avoid; text-align: center;">
  <img src="assets/chapter04/LPMockupSobreNosotros.png"
       alt="Landing Page Mockup 3"
       style="max-width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 3:</strong> Sobre Nosotros.
  </figcaption>
</figure>

---

**Testimonios**
Incluye citas y fotos de clientes reales, proporcionando prueba social para validar la calidad del servicio.

<figure style="page-break-inside: avoid; text-align: center;">
  <img src="assets/chapter04/LPMockupTestimonios.png"
       alt="Landing Page Mockup 4"
       style="max-width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 4:</strong> Testimonios.
  </figcaption>
</figure>

---

**Contacto**
Ofrece un formulario simple y directo con campos bien organizados para que los interesados puedan solicitar información fácilmente.

<figure style="page-break-inside: avoid; text-align: center;">
  <img src="assets/chapter04/LPMockupContacto.png"
       alt="Landing Page Mockup 5"
       style="max-width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 5:</strong> Contacto.
  </figcaption>
</figure>

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

Los wireframes de las aplicaciones web de IceTrack muestran cómo se estructuran las pantallas y dónde se ubican los elementos de navegación. Estos esquemas visuales, que se centran en la funcionalidad y la facilidad de uso, guían el diseño final. Su objetivo es asegurar que la aplicación sea intuitiva y que la interacción del usuario sea fluida y eficiente, lo que ayuda a diseñadores y desarrolladores a optimizar la disposición de cada componente.

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe1.png" alt="WebWireframe1.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Wireframe Registro.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe2.png" alt="WebWireframe2.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 2:</strong> Wireframe Dashboard.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe3.png" alt="WebWireframe3.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 3:</strong> Wireframe Sitios y equipos.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe4.png" alt="WebWireframe4.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 4:</strong> Wireframe Detalle del equipo.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe5.png" alt="WebWireframe5.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 5:</strong> Wireframe Alertas.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe6.png" alt="WebWireframe6.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 6:</strong> Wireframe Órdenes.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
  <div align="center">
    <img src="assets/chapter04/WebWireframe7.png" alt="WebWireframe7.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 7:</strong> Wireframe Reportes.
  </figcaption>
</figure>

---

<figure style="page-break-inside: avoid; text-align: center;">
 <div align="center">
    <img src="assets/chapter04/WebWireframe8.png" alt="WebWireframe8.png">
  </div>
  <figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 8:</strong> Wireframe Administración.
  </figcaption>
</figure>

### 4.4.2. Web Applications Wireflow Diagrams
<img width="2576" height="916" alt="Web Applications Wireflow Diagram" src="https://github.com/user-attachments/assets/4d5247bc-d766-4593-ba97-cc59d411e93e" />

### 4.4.3. Web Applications Mock-ups

**Login**
En esta sección, los usuarios pueden crear sus cuentas para acceder a la aplicación. Es el punto de entrada que les permite gestionar y monitorear sus equipos.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/1eaa860c-ea4b-41d0-9690-d1f125456392" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Login Mockup.
  </figcaption>

---

**Registro**
Es el centro de control de la app. Aquí se visualiza un resumen ejecutivo de las operaciones clave: estado de los equipos, cantidad de órdenes pendientes y alertas activas. Es una vista rápida para tomar decisiones.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/ac78a44f-fbf5-4b7d-b418-150a94d8e401" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 2:</strong> Register Mockup.
  </figcaption>

---

**Órdenes**
Esta sección es para gestionar los servicios técnicos. Se pueden crear, asignar y hacer seguimiento a las órdenes de trabajo para mantenimiento preventivo o correctivo, garantizando que cada tarea se complete de forma eficiente.

<img width="1600" height="1181" alt="screen" src="https://github.com/user-attachments/assets/05ea25f4-0c4d-49e7-8905-0481c0c25ec2" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 3:</strong> Order Mockup.
  </figcaption>

---

**Reportes**
Aquí los usuarios pueden generar informes detallados. Estos reportes analizan el rendimiento de los equipos, el historial de mantenimiento y la eficiencia de los servicios, lo cual es vital para la toma de decisiones estratégicas.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/e8f13a84-bb00-4868-8f5a-49b1f955b3a3" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 4:</strong> Register Mockup.
  </figcaption>

---

**Sitios y Equipos**
Esta sección funciona como un inventario centralizado. Aquí se listan y gestionan todos los sitios (ubicaciones físicas) y los equipos de refrigeración que tienen asignados.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/be14d1d6-edd5-4da2-b89b-c9c31644dab9" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 5:</strong> Sites & Equipment Mockup.
  </figcaption>

---

**Detalles del Equipo**
Al seleccionar un equipo en particular, se accede a esta sección. Aquí se puede ver toda la información detallada del equipo: especificaciones técnicas, historial de mantenimiento, estado actual y alertas recientes.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/edd67335-1168-434c-96be-2c0fd00fbbd8" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 6:</strong> Equipment details.
  </figcaption>

---

**Panel de Control**
<img width="1600" height="1460" alt="screen" src="https://github.com/user-attachments/assets/5faadadd-f97d-41f5-b089-dc97c797a5fc" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 7:</strong> Dashboard Mockup.
  </figcaption>

---

**Alertas**
Aquí se notifican y gestionan todas las incidencias importantes. Por ejemplo, si un equipo de refrigeración presenta una falla, una alerta automática aparece en esta sección, permitiendo una respuesta inmediata.

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/62f6fa99-9b06-4268-a299-fecb636f753f" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 8:</strong> Alerts Mockup.
  </figcaption>

---

**Administración**

<img width="1600" height="1000" alt="screen" src="https://github.com/user-attachments/assets/1d86befd-8e5f-456c-99a9-eea34027cda4" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 9:</strong> Admin Mockup.
  </figcaption>

---

### 4.4.4. Web Applications User Flow Diagrams
<img width="2576" height="1682" alt="Web Applications User Flow Diagram" src="https://github.com/user-attachments/assets/8e5073cf-0112-48be-8c50-8981410ef2c1" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Web Applications User Flow Diagram.
  </figcaption>

## 4.5. Web Applications Prototyping

La sección de Prototipado de Aplicaciones Web muestra un modelo interactivo y funcional de la aplicación IceTrack antes de su desarrollo final. Este proceso permite simular el flujo de usuario, la navegación y las interacciones principales, garantizando que el diseño sea intuitivo y que la experiencia de usuario sea la mejor posible. Es la fase donde las ideas se validan con un producto tangible.

URL: https://www.figma.com/proto/ssl7G9KRip9XbC0tBXqUnc/Untitled?node-id=1-2&p=f&t=Kj4CziPHI6VX6P3M-1&scaling=contain&content-scaling=responsive&page-id=0%3A1

---

## 4.6. Domain-Driven Software Architecture
### 4.6.1. Design-Level EventStorming

### 4.6.2. Software Architecture Context Diagram
<img width="1297" height="591" alt="4 6 2  Software Architecture Context Diagram" src="assets/chapter05/context-diagram.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Context Diagram.
  </figcaption>

### 4.6.3. Software Architecture Container Diagrams
<img width="1170" height="579" alt="4 6 3  Software Architecture Container Diagrams" src="assets/chapter05/containers-diagram.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Container Diagrams.
  </figcaption>

### 4.6.4. Software Architecture Components Diagrams
<img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/apirest-diagram.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> API REST Component Diagrams.
  </figcaption>

  <img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/assetsmanagement-component.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 2:</strong> Assets Management BC Component Diagrams.
  </figcaption>

  <img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/dashboard-component.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 3:</strong> Dashboard BC Component Diagrams.
  </figcaption>

   <img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/monitoring-component.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 4:</strong> Monitoring BC Component Diagrams.
  </figcaption>

  <img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/reporting-component.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 5:</strong> Reporting BC Component Diagrams.
  </figcaption>

   <img width="1614" height="1354" alt="4 6 4  Software Architecture Components Diagrams" src="assets/chapter05/services-component.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 6:</strong> Services BC Component Diagrams.
  </figcaption>

## 4.7. Software Object-Oriented Design
### 4.7.1. Class Diagrams
<img width="2669" height="1621" alt="Diagrama de Clases" src="https://github.com/user-attachments/assets/96c0cbb8-7cf3-4527-98c7-6384ad68307e" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Class Diagram.
  </figcaption>

## 4.8. Database Design
### 4.8.1. Database Diagrams
<img width="1800" height="850" alt="base de datos diseño" src="assets/chapter04/Database diagram.png" />
<figcaption style="font-size: 0.9em; color: #555;">
    <strong>Figura 1:</strong> Database Diagram.
  </figcaption>
