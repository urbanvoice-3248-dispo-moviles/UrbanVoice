# <p align="center" id="caratula"> Universidad Peruana de Ciencias Aplicadas </p>

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png" alt="Logo UPC">
</div>

### <p align="center"> Informe Trabajo Final </p>

<br>
<div align="center">
  <p> Carrera: Ingeniería de Software </p>
  <br>
  <p> Ciclo: 2026-10 </p>
  <br>
  <p> Curso: Aplicaciones para dispositivos móviles </p>
  <br>
  <p> NRC: 3248 </p>
  <br>
  <p> Profesor: David Gerardo Quevedo </p>
  <br>
  <p> Nombre del Startup: UrbanVoice </p>
  <br>
  <p> Nombre del Producto: UrbanVoice </p>
  <br>
  <p> Relación de Integrantes: </p>
  <p>  - Ivan La Madrid - (u202113432). </p>
  <p>  - Quijada Magro, Jeremy Alexander (u202219657). </p>
  <p>  - Ruiz Madrid, Billy Jake (u202116401) </p>
  <p>  - Gordillo Ramos, Santiago Alonso (u202215160) </p>
  <p>  - Awad Vargas, Giorgio Marzouk (u202324041) </p>
  <br>
  <p> Mes y Año: Abril del 2026 </p>
</div>

---

# Registro de Versiones del Informe

<table>
  <tr>
    <th style="text-align:center;">Versión</th>
    <th style="text-align:center;">Fecha</th>
    <th style="text-align:center;">Autor</th>
    <th style="text-align:center;">Descripción de la modificación</th>
  </tr>
  <tr>
    <td align="center">Avance 1</td>
    <td>22/04/2026</td>
    <td> Giorgio Marzouk Awad Vargas <br> Quijada Magro Jeremy <br> Billy Ruiz <br> Santiago Gordillo <br> Ivan La Madrid </td>
    <td> Hemos avanzado bastante en la estructuración del proyecto: ya tengo definidos los capítulos con la introducción de la startup, el perfil de la solución, los segmentos objetivo y un análisis completo de requerimientos. También incluimos entrevistas, user personas, mapas de tareas y journey maps, además de aplicar Lean UX y Domain-Driven Design en niveles estratégico y táctico. En resumen, logramos darle forma clara y ordenada al documento, con bases conceptuales y técnicas que sostienen el desarrollo. </td>
  </tr>
  <tr>
    <td align="center">TP1</td>
    <td>13/05/2026</td>
    <td> Giorgio Marzouk Awad Vargas <br> Quijada Magro Jeremy <br> Billy Ruiz <br> Santiago Gordillo <br> Ivan La Madrid </td>
    <td> Consolidación final del informe para el Trabajo Parcial. Se completó el diseño detallado de la arquitectura de software (Diagramas de Componentes y Base de Datos por Bounded Context) y el diseño de interfaz de alta fidelidad (Mockups y Wireflows) para los flujos críticos. Se integró la sección de Software Configuration Management detallando el flujo de GitFlow y despliegue. Asimismo, se incluyó la evidencia de ejecución del Sprint 1, el despliegue del Landing Page en GitHub Pages y la documentación de Web Services mediante Swagger/OpenAPI. </td>
  </tr>
</table>

---

# Tabla de contenidos

- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Tabla de contenidos](#tabla-de-contenidos)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
    - [1.1 Startup Profile](#11-startup-profile)
        - [1.1.1 Descripción de la Startup](#111-descripción-de-la-startup)
        - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
    - [1.2. Solution Profile](#12-solution-profile)
        - [1.2.1. Nombre del Producto](#121-nombre-del-producto)
        - [1.2.2. Antecedentes y problemática](#122-antecedentes-y-problemática)
        - [1.2.3. Lean UX Process](#123-lean-ux-process)
            - [1.2.3.1. Lean UX Problem Statements](#1231-lean-ux-problem-statements)
            - [1.2.3.2. Lean UX Assumptions](#1232-lean-ux-assumptions)
            - [1.2.3.3. Lean UX Hypothesis Statements](#1233-lean-ux-hypothesis-statements)
            - [1.2.3.4. Lean UX Canvas](#1234-lean-ux-canvas)
    - [1.3. Segmentos Objetivo](#13-segmentos-objetivo)

- [Capítulo II: Requirements Development and Software Solution Design](#capítulo-ii-requirements-development-and-software-solution-design)
   - [2.1. Competidores](#21-competidores)
   - [2.1.1 Analisis competitivo](#211-analisis-competitivo)
   - [2.1.2 Estrategias y tacticas frente a competidores](#212-estrategias-y-tacticas-frente-a-competidores)
   - [2.2. Entrevistas](#22-entrevistas)
   - [2.2.1 Diseño de entrevistas](#221-diseño-de-entrevistas)
   - [2.2.2 Registro de entrevistas](#222-registro-de-entrevistas)
   - [2.2.3 Análisis de entrevistas](#223-análisis-de-entrevistas)
   - [2.3. Needfinding](#23-needfinding)
      - [2.3.1. User Personas](#231-user-personas)
      - [2.3.2. User Task Matrix](#232-user-task-matrix)
      - [2.3.3. User Journey Map](#233-user-journey-map)
      - [2.3.4. Empathy Mapping](#234-empathy-mapping)
      - [2.3.5. Big Picture EventStorming ](#235-big-picture-eventstorming)
      - [2.3.6. Ubiquitous Language](#236-ubiquitous-language)
   - [2.4. Requirements specification](#24-requirements-specification)
      - [2.4.1. User Stories](#241-user-stories)
      - [2.4.2. Impact Mapping](#242-impact-mapping)
      - [2.4.3. Product Backlog](#243-product-backlog)
   - [2.5. Strategic-Level Domain-Driven Design](#25-strategic-level-domain-driven-design)
      - [2.5.1. EventStorming](#251-eventstorming)
         - [2.5.1.1. Candidate Context Discovery](#2511-candidate-context-discovery)
         - [2.5.1.2. Domain Message Flows Modeling](#2512-domain-message-flows-modeling)
         - [2.5.1.3. Bounded Context Canvases](#2513-bounded-context-canvases)
      - [2.5.2. Context Mapping](#252-context-mapping)
      - [2.5.3. Software Architecture](#253-software-architecture)
         - [2.5.3.1. Software Architecture Context Level Diagrams](#2531-software-architecture-context-level-diagrams)
         - [2.5.3.2. Software Architecture Container Level Diagrams](#2532-software-architecture-container-level-diagrams)
         - [2.5.3.3. Software Architecture Deployment Diagrams](#2533-software-architecture-deployment-diagrams)
      - [2.6 Tactical-Level Domain-Driven Design](#26-technical-level-domain-driven-design)
         - [2.6.1 Bounded Context:Identity and Access Managment](#261-bounded-context-Identity-and-Access-Managment)
            - [2.6.1.1. Domain Layer](#2611-domain-layer)
            - [2.6.1.2. Interface Layer](#2612-interface-layer)
            - [2.6.1.3. Application Layer](#2613-application-layer)
            - [2.6.1.4 Infrastructure Layer](#2614-infrastructure-layer)
            - [2.6.1.5 Bounded Context Software Architecture Component Level Diagrams](#2615-bounded-context-software-architecture-component-level-diagrams)
            - [2.6.1.6 Bounded Context Software Architecture Code Level Diagrams](#2616-bounded-context-software-architecture-code-level-diagrams)
            - [2.6.1.6.1. Bounded Context Domain Layer Class Diagrams](#26161-bounded-context-domain-layer-class-diagrams)
            - [2.6.1.6.2. Bounded Context Database Design Diagram](#26162-bounded-context-database-design-diagram)
         - [2.6.2 Bounded Context:Profile and Preferences Management](#262-bounded-context-Profile-and-Preferences-Management)
            - [2.6.2.1. Domain Layer](#2621-domain-layer)
            - [2.6.2.2. Interface Layer](#2622-interface-layer)
            - [2.6.2.3. Application Layer](#2623-application-layer)
            - [2.6.2.4 Infrastructure Layer](#2624-infrastructure-layer)
            - [2.6.2.5 Bounded Context Software Architecture Component Level Diagrams](#2625-bounded-context-software-architecture-component-level-diagrams)
            - [2.6.2.6 Bounded Context Software Architecture Code Level Diagrams](#2626-bounded-context-software-architecture-code-level-diagrams)
            - [2.6.2.6.1. Bounded Context Domain Layer Class Diagrams](#26261-bounded-context-domain-layer-class-diagrams)
            - [2.6.2.6.2. Bounded Context Database Design Diagram](#26262-bounded-context-database-design-diagram)
         - [2.6.3 Bounded Context:Location Managment](#263-bounded-context-Location-Managment)
            - [2.6.3.1. Domain Layer](#2631-domain-layer)
            - [2.6.3.2. Interface Layer](#2632-interface-layer)
            - [2.6.3.3. Application Layer](#2633-application-layer)
            - [2.6.3.4 Infrastructure Layer](#2634-infrastructure-layer)
            - [2.6.3.5 Bounded Context Software Architecture Component Level Diagrams](#2635-bounded-context-software-architecture-component-level-diagrams)
            - [2.6.3.6 Bounded Context Software Architecture Code Level Diagrams](#2636-bounded-context-software-architecture-code-level-diagrams)
            - [2.6.3.6.1. Bounded Context Domain Layer Class Diagrams](#26361-bounded-context-domain-layer-class-diagrams)
            - [2.6.3.6.2.  Bounded Context Database Design Diagram](#26362--bounded-context-database-design-diagram)
         - [2.6.4 Bounded Context:Report Managment](#264-bounded-context-Report-Managment)
            - [2.6.4.1. Domain Layer](#2641-domain-layer)
            - [2.6.4.2. Interface Layer](#2642-interface-layer)
            - [2.6.4.3. Application Layer](#2643-application-layer)
            - [2.6.4.4 Infrastructure Layer](#2644-infrastructure-layer)
            - [2.6.4.5 Bounded Context Software Architecture Component Level Diagrams](#2645-bounded-context-software-architecture-component-level-diagrams)
            - [2.6.4.6 Bounded Context Software Architecture Code Level Diagrams](#2646-bounded-context-software-architecture-code-level-diagrams)
            - [2.6.4.6.1. Bounded Context Domain Layer Class Diagrams](#26461-bounded-context-domain-layer-class-diagrams)
            - [2.6.4.6.2. Bounded Context Database Design Diagram](#26462-bounded-context-database-design-diagram)
         - [2.6.5 Bounded Context:Notification Managment](#265-bounded-context-Notification-Managment)
            - [2.6.5.1. Domain Layer](#2651-domain-layer)
            - [2.6.5.2. Interface Layer](#2652-interface-layer)
            - [2.6.5.3. Application Layer](#2653-application-layer)
            - [2.6.5.4 Infrastructure Layer](#2654-infrastructure-layer)
            - [2.6.5.5 Bounded Context Software Architecture Component Level Diagrams](#2655-bounded-context-software-architecture-component-level-diagrams)
            - [2.6.5.6 Bounded Context Software Architecture Code Level Diagrams](#2656-bounded-context-software-architecture-code-level-diagrams)
            - [2.6.5.6.1. Bounded Context Domain Layer Class Diagrams](#26561-bounded-context-domain-layer-class-diagrams)
            - [2.6.5.6.2. Bounded Context Database Design Diagram](#26562-bounded-context-database-design-diagram)

- [Capítulo III: Solution UI/UX Design](#capítulo-iii-solution-uiux-design)
  - [3.1. Product design](#31-product-design)
    - [3.1.1. Style Guidelines](#311-style-guidelines)
      - [3.1.1.1. General Style Guidelines](#3111-general-style-guidelines)
    - [3.1.2. Information Architecture](#312-information-architecture)   
      - [3.1.2.1. Organization Systems](#3121-organization-systems)
      - [3.1.2.2. Labelling Systems](#3122-labelling-systems)
      - [3.1.2.3. SEO Tags and Meta Tags](#3123-seo-tags-and-meta-tags)
      - [3.1.2.4. Searching Systems](#3124-searching-systems)
      - [3.1.2.5. Navigation Systems](#3125-navigation-systems)
    - [3.1.3. Landing Page UI Design](#313-landing-page-ui-design)
      - [3.1.3.1. Landing Page Wireframe](#3131-landing-page-wireframe)
      - [3.1.3.2. Landing Page Mock-up](#3132-landing-page-mock-up)
    - [3.1.4. Mobile Applications UX/UI Design](#314-mobile-applications-uxui-design)
      - [3.1.4.1. Mobile Applications Wireframes](#3141-mobile-applications-wireframes)
      - [3.1.4.2. Mobile Applications Wireflow Diagrams](#3142-mobile-applications-wireflow-diagrams)
      - [3.1.4.3. Mobile Applications Mock-ups](#3143-mobile-applications-mock-ups)
      - [3.1.4.4. Mobile Applications User Flow Diagrams](#3144-mobile-applications-user-flow-diagrams)
      - [3.1.4.5. Mobile Applications Prototyping](#3145-mobile-applications-prototyping)

- [Capítulo IV: Product Implementation & Validation](#capítulo-iv-product-implementation--validation)
  - [4. Product Implementation & Validation](#4-product-implementation--validation)
    - [4.1. Software Configuration Management](#41-software-configuration-management)
      - [4.1.1. Software Development Environment Configuration](#411-software-development-environment-configuration)
      - [4.1.2. Source Code Management](#412-source-code-management)
      - [4.1.3. Source Code Style Guide & Conventions](#413-source-code-style-guide--conventions)
      - [4.1.4. Software Deployment Configuration](#414-software-deployment-configuration)
    - [4.2. Landing Page & Mobile Application Implementation](#42-landing-page--mobile-application-implementation)
      - [4.2.1. Sprint 1](#421-sprint-1)
        - [4.2.1.1. Sprint Planning 1](#4211-sprint-planning-1)
        - [4.2.1.2. Sprint Backlog 1](#4212-sprint-backlog-1)
        - [4.2.1.3. Development Evidence for Sprint Review](#4213-development-evidence-for-sprint-review)  
        - [4.2.1.4. Testing Suite Evidence for Sprint Review](#4214-testing-suite-evidence-for-sprint-review)  
        - [4.2.1.5. Execution Evidence for Sprint Review](#4215-execution-evidence-for-sprint-review)  
        - [4.2.1.6. Services Documentation Evidence for Sprint Review](#4216-services-documentation-evidence-for-sprint-review)  
        - [4.2.1.7. Software Deployment Evidence for Sprint Review](#4217-software-deployment-evidence-for-sprint-review)  
        - [4.2.1.8. Team Collaboration Insights during Sprint](#4218-team-collaboration-insights-during-sprint)
      - [4.2.2. Sprint 2](#422-sprint-2)
        - [4.2.2.1. Sprint Planning 2](#4221-sprint-planning-2)
        - [4.2.2.2. Sprint Backlog 2](#4222-sprint-backlog-2)
        - [4.2.2.3. Development Evidence for Sprint Review](#4223-development-evidence-for-sprint-review)  
        - [4.2.2.4. Testing Suite Evidence for Sprint Review](#4224-testing-suite-evidence-for-sprint-review)  
        - [4.2.2.5. Execution Evidence for Sprint Review](#4225-execution-evidence-for-sprint-review)  
        - [4.2.2.6. Services Documentation Evidence for Sprint Review](#4226-services-documentation-evidence-for-sprint-review)  
        - [4.2.2.7. Software Deployment Evidence for Sprint Review](#4227-software-deployment-evidence-for-sprint-review)  
        - [4.2.2.8. Team Collaboration Insights during Sprint](#4228-team-collaboration-insights-during-sprint)
      - [4.2.3. Sprint 3](#423-sprint-3)
        - [4.2.3.1. Sprint Planning 3](#4231-sprint-planning-3)
        - [4.2.3.2. Sprint Backlog 3](#4232-sprint-backlog-3)
        - [4.2.3.3. Development Evidence for Sprint Review](#4233-development-evidence-for-sprint-review)
        - [4.2.3.4. Testing Suite Evidence for Sprint Review](#4234-testing-suite-evidence-for-sprint-review)
        - [4.2.3.5. Execution Evidence for Sprint Review](#4235-execution-evidence-for-sprint-review)
        - [4.2.3.6. Services Documentation Evidence for Sprint Review](#4236-services-documentation-evidence-for-sprint-review)
        - [4.2.3.7. Software Deployment Evidence for Sprint Review](#4237-software-deployment-evidence-for-sprint-review)
        - [4.2.3.8. Team Collaboration Insights during Sprint](#4238-team-collaboration-insights-during-sprint)

---

# Project Report Collaboration Insights
En esta sección se detalla el proceso de colaboración para la elaboración del informe en el repositorio de GitHub.

**URL del repositorio:** https://github.com/urbanvoice-3248-dispo-moviles/UrbanVoice

   - Se realizaron commits individuales para las secciones de perfiles y descripción de la startup.
   - Se coordinó de forma sincrónica la definición de las hipótesis de Lean UX y el análisis de la problemática.


<img src="assets/Evidence Sprint Review.png"/><br/>

<img src="assets/Network.png"/><br/>

---

# Student Outcome

**Criterio:** La capacidad de adquirir y aplicar nuevos conocimientos según sea necesario, utilizando estrategias de
aprendizaje apropiadas.

**ABET -- EAC - Student Outcome**

<table>
<colgroup>
<col style="width: 30%" />
<col style="width: 40%" />
<col style="width: 30%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Criterio específico</strong></th>
<th><strong>Acciones Realizadas</strong></th>
<th><strong>Conclusiones</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Actualiza conceptos y
conocimientos necesarios para su
desarrollo profesional y en especial
para su proyecto en soluciones de
software.</td>
<td>
            <strong>Ruiz Madrid, Billy Jake</strong> <br>
            Avance 1: Aprendió a utilizar Structurizr DSL para generar diagramas de arquitectura como código, optimizando la documentación técnica del equipo. <br>
            TP: Exploró algoritmos de agrupamiento espacial (clustering) para optimizar el rendimiento del renderizado de capas de calor en dispositivos móviles.  <br>Avance 2: Desarrolló la visualización del mapa interactivo con marcadores de incidentes y geolocalización del usuario, permitiendo identificar zonas de riesgo cercanas.<br><br>
            <strong>Gordillo Ramos, Santiago Alonso</strong> <br>
            Avance 1: Estudió pautas de accesibilidad universal (a11y) y Material Design para aplicarlas en la experiencia de usuario de las aplicaciones del proyecto. <br>
            TP: Investigó técnicas de optimización SEO y Meta Tags para mejorar el posicionamiento orgánico y visibilidad del Landing Page en buscadores. <br> Avance 2: Implementó el formulario de reportes ciudadanos, conectándolo con los endpoints del backend para almacenar incidentes con su ubicación. <br>
            <strong>La Madrid Lozano, Ivan Jeanpierre</strong> <br>
            Avance 1: Profundizó en el uso de contenedores y despliegue en la nube para asegurar entornos de ejecución consistentes en el backend del proyecto. <br>
            TP: Investigó la implementación de protocolos de seguridad JWT para proteger las comunicaciones sensibles entre la aplicación móvil y los microservicios. <br>Avance 2: Integró la carga de imágenes, audios y videos dentro de los reportes, permitiendo adjuntar pruebas al momento de registrar un incidente.<br>
            <strong>Awad Vargas, Giorgio Marzouk</strong> <br>
            Avance 1: Identificó la necesidad de aprender nuevas herramientas de modelado arquitectónico para representar correctamente los componentes de UrbanVoice. <br>
            TP: Investigó estándares de almacenamiento de archivos en la nube para gestionar eficientemente la evidencia multimedia de los reportes ciudadanos.<br>Avance 2: Añadió la opción de realizar reportes de forma anónima, protegiendo la identidad del usuario y reforzando la privacidad de la plataforma.<br>
            <strong>Quijada Magro, Jeremy Alexander</strong> <br>
            Avance 1: <br> Lideró la fase de investigación de usuarios y la construcción de arquetipos (User Personas) para alinear los requisitos con las necesidades de seguridad en Lima Metropolitana. <br>
            TP: <br> Implementó el Testing Suite bajo el enfoque BDD utilizando Gherkin para validar los criterios de aceptación del núcleo operativo de la aplicación móvil[cite: 694, 697]. <br> Avance 2:Implementó la lógica para calcular rutas seguras entre dos puntos, evaluando zonas de riesgo para sugerir trayectos alternativos.<br>
</td>
<td>
<em><strong>Avance 1</strong></em>
<br>El equipo logró consolidar una base metodológica sólida mediante Lean UX y DDD, lo que permitió transformar percepciones subjetivas de inseguridad en requerimientos técnicos accionables y bien estructurados.
<br><br>
<em><strong>TP1</strong></em>
<br>Se validó que la integración de pruebas automatizadas y el diseño de arquitectura táctica son esenciales para garantizar que el producto final sea escalable y cumpla con los estándares de calidad exigidos.
<br><br>
<em><strong>Avance 2</strong></em>
<br>Durante este sprint se consolidaron las funcionalidades principales de UrbanVoice: mapa de riesgo, reportes ciudadanos, evidencia multimedia, anonimato y rutas seguras. Además, se completó la infraestructura backend necesaria para soportar estas operaciones.
</td>
</tr>
<tr class="even">
<td>Reconoce la necesidad del
aprendizaje permanente para el
desempeño profesional y el
desarrollo de proyectos en
soluciones de software.</td>
<td>
            <strong>Ruiz Madrid, Billy Jake</strong> <br>
            Avance 1: Aprendió a utilizar Structurizr DSL para generar diagramas de arquitectura como código, optimizando la documentación técnica del equipo. <br>
            TP: Exploró algoritmos de agrupamiento espacial (clustering) para optimizar el rendimiento del renderizado de capas de calor en dispositivos móviles.  <br>Avance 2: Desarrolló la visualización del mapa interactivo con marcadores de incidentes y geolocalización del usuario, permitiendo identificar zonas de riesgo cercanas.<br><br>
            <strong>Gordillo Ramos, Santiago Alonso</strong> <br>
            Avance 1: Estudió pautas de accesibilidad universal (a11y) y Material Design para aplicarlas en la experiencia de usuario de las aplicaciones del proyecto. <br>
            TP: Investigó técnicas de optimización SEO y Meta Tags para mejorar el posicionamiento orgánico y visibilidad del Landing Page en buscadores. <br> Avance 2: Implementó el formulario de reportes ciudadanos, conectándolo con los endpoints del backend para almacenar incidentes con su ubicación. <br>
            <strong>La Madrid Lozano, Ivan Jeanpierre</strong> <br>
            Avance 1: Profundizó en el uso de contenedores y despliegue en la nube para asegurar entornos de ejecución consistentes en el backend del proyecto. <br>
            TP: Investigó la implementación de protocolos de seguridad JWT para proteger las comunicaciones sensibles entre la aplicación móvil y los microservicios. <br>Avance 2: Integró la carga de imágenes, audios y videos dentro de los reportes, permitiendo adjuntar pruebas al momento de registrar un incidente.<br>
            <strong>Awad Vargas, Giorgio Marzouk</strong> <br>
            Avance 1: Identificó la necesidad de aprender nuevas herramientas de modelado arquitectónico para representar correctamente los componentes de UrbanVoice. <br>
            TP: Investigó estándares de almacenamiento de archivos en la nube para gestionar eficientemente la evidencia multimedia de los reportes ciudadanos.<br>Avance 2: Añadió la opción de realizar reportes de forma anónima, protegiendo la identidad del usuario y reforzando la privacidad de la plataforma.<br>
            <strong>Quijada Magro, Jeremy Alexander</strong> <br>
            Avance 1: <br> Lideró la fase de investigación de usuarios y la construcción de arquetipos (User Personas) para alinear los requisitos con las necesidades de seguridad en Lima Metropolitana. <br>
            TP: <br> Implementó el Testing Suite bajo el enfoque BDD utilizando Gherkin para validar los criterios de aceptación del núcleo operativo de la aplicación móvil[cite: 694, 697]. <br> Avance 2:Implementó la lógica para calcular rutas seguras entre dos puntos, evaluando zonas de riesgo para sugerir trayectos alternativos.<br>
</td>
<td>
<em><strong>Avance 1</strong></em>
<br>Se evidenció que la adopción de herramientas de modelado como código y la investigación autónoma de metodologías ágiles son fundamentales para el éxito del diseño inicial del proyecto.
<br><br>
<em><strong>TP1</strong></em>
<br>El aprendizaje de herramientas de CI/CD y automatización demostró ser clave para optimizar los tiempos de entrega, reforzando la idea de que la actualización tecnológica constante es una ventaja competitiva en el desarrollo de software.
<br><br>
<em><strong>Avance 2</strong></em>
<br>Durante este sprint se consolidaron las funcionalidades principales de UrbanVoice: mapa de riesgo, reportes ciudadanos, evidencia multimedia, anonimato y rutas seguras. Además, se completó la infraestructura backend necesaria para soportar estas operaciones.
</td>

</tr>
</tbody>
</table>

# Student Outcome

Perfecto. Como el PDF exige **mínimo 2 objetivos SMART por integrante** y enfocados en el desarrollo profesional post-carrera , te propongo estos alineados a los perfiles del equipo y al proyecto:

# Objetivos SMART

### Jeremy Quijada Magro

Fortalecer mis competencias en **Quality Assurance y Testing Automation**, completando al menos **3 certificaciones especializadas** (ISTQB, Selenium y Cypress) durante los próximos **12 meses**, para especializarme profesionalmente en aseguramiento de calidad de software.

Implementar y documentar al menos **5 suites de pruebas automatizadas** en proyectos académicos o personales antes de finalizar el próximo ciclo académico, con el objetivo de consolidar experiencia práctica en testing funcional y BDD.

---

### Billy Jake Ruiz Madrid

Mejorar mis habilidades en **Data Structures y Performance Optimization**, desarrollando al menos **4 proyectos avanzados en C++ y Python** en un plazo de **10 meses**, orientados a optimización algorítmica.

Obtener experiencia profesional en desarrollo backend postulando a **mínimo 15 oportunidades laborales o prácticas** durante los próximos **8 meses**, fortaleciendo su perfil técnico.

---

### Santiago Alonso Gordillo Ramos

Especializarme en **Frontend Development y UX Engineering**, dominando **Vue, Angular y React** mediante la creación de **3 aplicaciones completas** en un periodo de **12 meses**.

Iniciar formación en **Ciberseguridad**, obteniendo una certificación inicial (como Security+ o equivalente) en los próximos **18 meses** para complementar mi perfil como desarrollador.

---

### Ivan Jeanpierre La Madrid Lozano

Profundizar en el ecosistema **.NET y arquitectura backend**, construyendo al menos **3 APIs escalables con microservicios** antes de finalizar el año 2027.

Adquirir experiencia en **Cloud Computing** obteniendo una certificación en **Azure Fundamentals o AWS Cloud Practitioner** dentro de los próximos **12 meses**.

---

### Giorgio Marzouk Awad Vargas


Especializarme en **Análisis de Datos**, completando al menos **2 certificaciones en Power BI y Machine Learning** durante los próximos **12 meses**.

Desarrollar al menos **3 soluciones de análisis de datos para casos empresariales reales** antes de graduarme, aplicando conocimientos de software engineering y business intelligence.

# Capítulo I: Introducción

## 1.1 Startup Profile

### 1.1.1 Descripción de la Startup

UrbanVoice es una iniciativa tecnológica enfocada en fortalecer la seguridad ciudadana en Lima Metropolitana. Ante la percepción de inseguridad del 89.9%, nuestra plataforma permite a los ciudadanos consultar niveles de riesgo en tiempo real y reportar incidentes de manera colaborativa.  

**Misión:**  
Nuestra misión es brindar seguridad a nuestros usuarios, permitiéndoles desplazarse con confianza por las distintas calles del Perú.  

**Visión:**  
Entendemos que el mundo está en constante transformación y queremos contribuir a ese cambio. Creemos que todas las personas tienen derecho a sentirse seguras en su país, y que es responsabilidad de los gobiernos garantizarlo. Por ello, aspiramos a posicionarnos como líderes en el sector de la seguridad, destacando por nuestro compromiso con el bienestar de nuestros usuarios.  

**¿Cómo lo logramos?**  
UrbanVoice se posiciona como una herramienta clave para quienes buscan mayor seguridad en su día a día. A través de nuestra aplicación, los usuarios pueden consultar un mapa interactivo que indica los niveles de seguridad en distintas zonas, facilitando la toma de decisiones informadas. Asimismo, ofrecemos la opción de reportar delitos de manera rápida y sencilla, incorporando fotos, audios o videos, de forma pública o anónima.  

Además, UrbamVoice ofrece una función adicional: compartir la ubicación en tiempo real con contactos de confianza, quienes podrán seguir el recorrido del usuario y brindarle mayor tranquilidad durante sus desplazamientos.  

### 1.1.2. Perfiles de integrantes del equipo

<table>
<colgroup>
<col style="width: 65%" />
<col style="width: 34%" />
</colgroup>
<thead>
<tr class="even">
<td><p><strong>Nombre:</strong> Jeremy Quijada Magro (U202219657)</p>
<p><strong> Mi nombre es Jeremy, me gusta el analisis de sistemas  y me gustaria especializarme en el area de calidad. </strong></p></td>
<td><img src="assets/Jeremy.jpeg"/></td>
</tr>
<tr class="even">
<td><p><strong>Nombre:</strong> Billy Jake Ruiz Madrid (U202116401)</p>
<p><strong> Tengo 22 años, soy una persona tranquila, colaborativa y adaptable. Me gusta trabajar en equipo, aportando ideas y soluciones. Cuento con conocimientos en C++ y Python y siempre busco formas de hacer las cosas de manera eficiente. </strong></p></td>
<td><img src="assets/Billy.jpg"/></td>
</tr>
<tr class="even">
<td><p><strong>Nombre:</strong> Santiago Alonso Gordillo Ramos (U202215160)</p>
<p><strong> Mi nombre es Santiago Gordillo, me gusta la programación, en específico el lado frontend y me gustaría especializarme en ciberseguridad. tengo 21 años, domino frameworks como vue, angular,etc y lenguajes como C++ , Python, Javascript.</strong></p></td>
<td><img src="assets/Santiago.jpg"/></td>
</tr>
<tr class="even">
<td><p><strong>Nombre:</strong> Ivan Jeanpierre La Madrid Lozano (u202113432)</p>
<p><strong> Me llamo Ivan La Madrid, tengo 22 años, me gusta el desarrollo de software. Últimamente me inclino más al desarrollo backend con frameworks como .NET </strong></p></td>
<td><img src="assets/ivan.jpeg"/></td>
<tr class="even">

<td><p><strong>Nombre:</strong> Giorgio Marzouk Awad Vargas (u202324041)</p>
<p><strong> Mi nombre es Giorgio Awad, tengo 23 años y estudio la carrera de Ingeniería de Software. Me gustaría especializarme en Análisis de Datos y en buscar soluciones a empresas através de los conocimientos adquiridos en la Ingeniería de Software. </strong></p></td>
<td><img src="assets/giorgio.jpeg"/></td>
</tr>

</table>

## 1.2. Solution Profile

### 1.2.1. Nombre del Producto

UrbanVoice, una aplicación móvil orientada a la seguridad ciudadana. Su propósito es brindar a los usuarios información en tiempo real sobre incidentes y zonas de riesgo en Lima Metropolitana, permitiendo tomar decisiones más seguras en sus desplazamientos y fomentando la colaboración entre ciudadanos y autoridades.

### 1.2.2. Antecedentes y problemática

* **Who (Quién):** Los ciudadanos residentes y transeúntes de Lima Metropolitana, especialmente aquellos que se movilizan por zonas con alta incidencia delictiva, falta de iluminación o escasa vigilancia. Asimismo, las víctimas directas e indirectas de robos, hurtos y acoso callejero.
* **What (Qué):** El incremento exponencial de la percepción de inseguridad (89.9%) y de la victimización delictiva real (27.7% de la población). El problema radica en la vulnerabilidad del ciudadano al transitar por espacios públicos sin información preventiva confiable.
* **Where (Dónde):** En las vías públicas, paraderos, parques y distritos de Lima Metropolitana con mayores índices de criminalidad. El peligro se agudiza en "puntos críticos" caracterizados por deficiencias en el diseño urbano y ausencia de autoridad.
* **When (Cuándo):** El riesgo es constante, aunque se intensifica durante los horarios nocturnos y en momentos de mayor flujo peatonal. La falta de actualización inmediata sobre incidentes recientes impide que el ciudadano tome precauciones en el momento oportuno.
* **Why (Por qué):** Debido a la ineficacia de los canales tradicionales de vigilancia y la desconfianza en los tiempos de respuesta de las autoridades. La ausencia de una red informativa colaborativa deja al ciudadano aislado y dependiente de métodos preventivos limitados a su entorno cercano.
* **How (Cómo):** La inseguridad se manifiesta a través de hechos delictivos frecuentes que afectan la libre circulación y la integridad física. El ciudadano intenta mitigar el riesgo de forma empírica (evitando calles o consultando familiares), pero sin datos precisos que respalden su toma de decisiones.
* **How Much (Cuánto):** Impacta negativamente en la calidad de vida de casi 10 millones de habitantes de la capital. Los costos se traducen en pérdidas económicas directas por robos, gastos en seguridad privada y, fundamentalmente, en un deterioro del bienestar emocional por el miedo constante al crimen.

### 1.2.3. Lean UX Process

#### 1.2.3.1. Lean UX Problem Statements

En la actualidad, Lima Metropolitana enfrenta una crisis de seguridad ciudadana que ha elevado la percepción de inseguridad al 89.9%, convirtiéndola en el principal problema para sus habitantes. Ante esta realidad, los ciudadanos se encuentran vulnerables al transitar por espacios públicos, especialmente en zonas con deficiente iluminación o escasa vigilancia, y dependen casi exclusivamente de redes de contacto directas o de evitar físicamente el peligro sin contar con información precisa sobre los riesgos en su entorno inmediato

Hemos detectado que existe una fuerte preocupación por la inseguridad en las calles, ya que los robos y delitos son situaciones frecuentes. De acuerdo con los resultados más recientes de la ENAPRES (Ene-Jun 2024) del INEI, el 27.7% de las personas mayores de 15 años en Perú ha sido víctima de algún delito.

¿Cómo podríamos mejorar la seguridad personal y colectiva de los ciudadanos, logrando que cuenten con información detallada y confiable en tiempo real para navegar de manera más segura por las calles de Lima y se sientan satisfechos con la protección que brinda el sistema?.

#### 1.2.3.2. Lean UX Assumptions

ahora que hemos analizado la problemática y contamos con una visión clara de cómo abordar la solución, es crucial identificar qué empresas comparten características similares a las nuestras y cómo han evolucionado con el tiempo. Esto nos permitirá aprender de su experiencia y adaptarnos mejor al mercado.

**Assumptions:**

1. **Las personas en Lima necesitan una app que les sugiera rutas más seguras.**  
   Debido al incremento de la delincuencia, los usuarios buscan formas de evitar zonas peligrosas al movilizarse.

2. **A los usuarios les interesa formar parte de una comunidad donde puedan reportar incidentes.**  
   El hecho de contribuir con información genera confianza y sentido de pertenencia.

3. **No hay una competencia fuerte que ofrezca una solución tan completa como la nuestra.**  
   Esto nos da la oportunidad de posicionarnos como una alternativa innovadora en seguridad ciudadana.

4. **Las instituciones que usen la app podrán aprovechar datos útiles para combatir la delincuencia.**  
   La información en tiempo real les permitirá actuar de manera más estratégica.

5. **Los ciudadanos estarán interesados en usar la aplicación.**  
   Al ser una herramienta práctica y fácil de usar, puede atraer a muchas personas.

6. **Las entidades públicas en Perú necesitan soluciones tecnológicas como esta.**  
   La app puede ayudarles a responder mejor ante situaciones de inseguridad.

**Business Outcomes:**

- Generar ingresos constantes mediante acuerdos con entidades públicas y privadas.  
- Aumentar la calidad de vida de las personas al reducir su exposición a riesgos.  
- Aportar a la reducción de la delincuencia mediante información útil y oportuna.

**User Outcomes:**

1. **¿Quién es el usuario?**  
   Cualquier persona que viva o trabaje en zonas donde la app esté disponible.

2. **¿Cómo encaja en su día a día?**  
   Se vuelve una herramienta clave para planificar rutas seguras y reportar incidentes.

3. **¿Qué dificultades enfrenta el producto?**  
   Depende bastante de lograr alianzas con entidades para sostener el modelo de negocio.

4. **¿Cuándo y cómo se usa?**  
   Principalmente al movilizarse por zonas desconocidas o al reportar situaciones de riesgo.

5. **¿Qué características son clave?**  
   Debe ser fácil de usar, rápida y con información actualizada en tiempo real.

6. **¿Cómo debería verse y funcionar?**  
   Con un diseño claro, atractivo y sencillo, que facilite la navegación y el registro.


**User Benefits:**

1. Reducir el riesgo de robos o incidentes al contar con información actualizada.
   
2. Tener acceso a un mapa que muestra zonas peligrosas y rutas más seguras.
   
3. Sentirse parte de una comunidad que aporta a la seguridad colectiva.


#### 1.2.3.3. Lean UX Hypothesis Statements

* **Hypothesis Statement 01:**
    **Creemos que** los ciudadanos están dispuestos a colaborar activamente para mitigar la percepción de abandono en sus comunidades si cuentan con una herramienta de reporte directo. 
    **Sabremos que funciona** cuando logremos una base de datos densa que permita identificar puntos críticos en tiempo real sin depender de fuentes oficiales lentas. 
    **Cuando veamos** que el 30% de los usuarios activos en distritos con alta incidencia delictiva realiza al menos un reporte semanal detallado con evidencia multimedia.

* **Hypothesis Statement 02:**
    **Creemos que** proporcionar un mapa de riesgo actualizado dinámicamente reducirá la exposición de los usuarios a hechos delictivos durante sus desplazamientos. 
    **Sabremos que funciona** cuando los usuarios integren la consulta de la aplicación como un paso preventivo habitual en su rutina diaria. 
    **Cuando veamos** que el flujo de "Consulta de Ruta Segura" sea utilizado por el 50% de nuestra base de usuarios antes de iniciar trayectos fuera de su zona de residencia habitual. 

* **Hypothesis Statement 03:**
    **Creemos que** la función de compartir la ubicación en tiempo real con contactos de confianza reducirá la ansiedad y sensación de vulnerabilidad del ciudadano al transitar por zonas desoladas. 
    **Sabremos que funciona** cuando la herramienta se convierta en el mecanismo de seguridad preventivo preferido sobre los métodos tradicionales de comunicación. 
    **Cuando veamos** que la funcionalidad "Live Tracking" se activa en promedio 5 veces por semana por cada usuario que se desplaza en horarios nocturnos. 

* **Hypothesis Statement 04:**
    **Creemos que** emitir alertas geolocalizadas automáticas sobre incidentes recientes en el entorno inmediato permitirá a los transeúntes evitar situaciones de peligro inminente. 
    **Sabremos que funciona** cuando los usuarios realicen cambios de ruta o tomen precauciones adicionales basándose exclusivamente en las notificaciones del sistema. 
    **Cuando veamos** que el 70% de las alertas de proximidad enviadas son calificadas como "Útiles" o "Verídicas" por los receptores a través del sistema de validación rápida. 

* **Hypothesis Statement 05:**
    **Creemos que** al centralizar la información de seguridad y facilitar la colaboración ciudadana, lograremos reducir la brecha de desconfianza y el sentimiento de desprotección en Lima. 
    **Sabremos que funciona** cuando los indicadores internos de satisfacción reflejen un cambio positivo en la experiencia de movilidad urbana del usuario. 
    **Cuando veamos** una disminución del 20% en la tasa de "Sensación de Vulnerabilidad" reportada por los usuarios en sus encuestas mensuales de perfil dentro de la aplicación. 

#### 1.2.3.4. Lean UX Canvas

![](assets/LeanUXCanvas.jpg)

## 1.3. Segmentos Objetivo

Nuestro público objetivo son personas de 18 a 65 años que residen o trabajan en Lima Metropolitana y se movilizan frecuentemente por la ciudad. Estos usuarios valoran su seguridad y están dispuestos a usar tecnología para mitigar riesgos.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 77%" />
</colgroup>
<thead>
<tr>
<th><strong>Variables</strong></th>
<th>Personas que buscan mayor seguridad al movilizarse en espacios públicos</th>
</tr>
</thead>
<tbody>

<tr>
<td><strong>Geográfica</strong></td>
<td>
<ul>
<li>Ubicación: Lima Metropolitana, priorizando zonas con alta incidencia delictiva y gran flujo de personas.</li>
<li>Alcance: Distritos urbanos y zonas concurridas dentro de Lima.</li>
</ul>
</td>
</tr>

<tr>
<td><strong>Demográfica</strong></td>
<td>
<ul>
<li>Edad: Personas entre 18 y 65 años.</li>
<li>Género: Público masculino y femenino.</li>
<li>Nivel socioeconómico: Sectores C1, C2 y C3 que se movilizan constantemente por trabajo, estudios u otras actividades.</li>
<li>Ocupación: Incluye estudiantes, trabajadores dependientes e independientes, y amas de casa.</li>
</ul>
</td>
</tr>

<tr>
<td><strong>Psicológica</strong></td>
<td>
<ul>
<li>Actitudes y valores: Individuos que valoran su seguridad y la de su entorno, atentos a situaciones de riesgo.</li>
<li>Motivaciones: Desean sentirse más tranquilos al desplazarse y contar con información confiable para tomar decisiones.</li>
<li>Estilo de vida: Personas dinámicas que se movilizan con frecuencia dentro de la ciudad.</li>
</ul>
</td>
</tr>

<tr>
<td><strong>Función de comportamiento</strong></td>
<td>
<ul>
<li>Necesidades: Información actualizada sobre niveles de seguridad en las zonas que transitan.</li>
<li>Comportamiento de uso: Usuarios que utilizan aplicaciones móviles para informarse y que están abiertos a usar tecnología para mejorar su seguridad.</li>
<li>Lealtad: Prefieren plataformas confiables donde puedan informarse y también aportar con reportes a la comunidad.</li>
</ul>
</td>
</tr>

</tbody>
</table>

# Capítulo II Requirements Development and Software Solution Design

## 2.1. Competidores

<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 29%" />
<col style="width: 30%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Principales Competidores</strong></th>
<th><strong>Características</strong></th>
<th><strong>Diferencias</strong></th>
<th><strong>Limitaciones</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>SafeCity</td>
<td><p>Reportes Anónimos: Permite a los usuarios reportar incidentes de manera completamente anónima.</p>
<p>Mapeo de Seguridad: Los datos se usan para crear mapas interactivos que muestran las áreas donde se reportan más incidentes.</p>
<p>Colaboración con ONG: SafeCity colabora con organizaciones no gubernamentales para utilizar los datos recopilados en campañas de concientización y políticas públicas.</p></td>
<td><p>Foco en el Acoso: Mientras que UrbanVoice abarca una amplia gama de incidentes, SafeCity se especializa en el reporte y la prevención del acoso.</p>
<p>Análisis de Datos: SafeCity ofrece un análisis más profundo de los datos para propósitos educativos y de políticas públicas.</p></td>
<td><p>Especificidad: El enfoque en el acoso puede limitar su utilidad para usuarios que buscan una herramienta más general de seguridad.</p>
<p>Cobertura Limitada: SafeCity no está disponible en todas las ciudades, a diferencia de UrbanVoice que se enfoca en Lima Metropolitana.</p></td>
</tr>
<tr class="even">
<td>Nextdoor</td>
<td><p>Foros Comunitarios: Espacios donde los vecinos pueden discutir temas de seguridad, reportar incidentes, y organizar eventos.</p>
<p>Alertas de Seguridad: Los usuarios pueden recibir notificaciones sobre incidentes de seguridad en su área.</p>
<p>Redes de Vecindario: Permite la creación de grupos privados basados en la ubicación del usuario.</p></td>
<td><p>Enfoque en la Comunidad: Nextdoor es más una red social con un enfoque amplio, mientras que UrbanVoice está específicamente diseñada para la seguridad ciudadana.</p>
<p>Cobertura: Disponible en varias ciudades a nivel internacional, no se limita solo a Lima.</p></td>
<td><p>No Específica de Seguridad: Aunque tiene funcionalidades de seguridad, Nextdoor es una plataforma de propósito general, no una aplicación de seguridad dedicada.</p>
<p>Privacidad: La naturaleza social de la plataforma puede plantear preocupaciones sobre la privacidad, especialmente en temas de seguridad.</p></td>
</tr>
<tr class="odd">
<td>Waze</td>
<td><p>Alcance: Aunque es principalmente una aplicación de navegación, Waze permite reportar incidentes en la vía pública, incluyendo accidentes y peligros.</p>
<p>Interacción: Los usuarios pueden reportar incidentes que otros conductores verán en tiempo real.</p>
<p>Popularidad: Amplia base de usuarios, lo que incrementa la cantidad de reportes en tiempo real.</p></td>
<td><p>Waze no está específicamente diseñada para la seguridad personal o la prevención de delitos, sino para la navegación y tráfico.</p>
<p>Su comunidad está más orientada a conductores que a peatones o personas que transitan a pie.</p></td>
<td><p>No está enfocada en la seguridad ciudadana de forma específica.</p>
<p>La información sobre incidentes podría no ser tan detallada ni orientada a la prevención de delitos.</p></td>
</tr>
</tbody>
</table>

### 2.1.1. Análisis Competitivo 

<table>
<colgroup>
<col style="width: 9%" />
<col style="width: 11%" />
<col style="width: 21%" />
<col style="width: 19%" />
<col style="width: 19%" />
<col style="width: 17%" />
</colgroup>
<thead>
<tr class="header">
<th colspan="6"><strong>Competitive Analysis Landscape</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td colspan="6"><em>¿Por qué llevar al cabo este análisis</em>? Para conocer a nuestros competidores, conocer sus estrategias y poder aprender de estos.</td>
</tr>
<tr class="even">
<td colspan="2">Empresas (Aplicación)</td>
<td><p>SafeCity</p></td>
<td><p>Nextdoor</p></td>
<td><p>Waze</p></td>
<td>UrbanVoice</td>
</tr>
<tr class="odd">
<td rowspan="2"><strong>Perfil</strong></td>
<td>Overview</td>
<td>SafeCity es una aplicación que permite a los usuarios reportar incidentes de acoso y violencia en tiempo real, principalmente enfocada en la seguridad de las mujeres. Utiliza los reportes para crear mapas de calor y prevenir riesgos.</td>
<td>Nextdoor es una red social privada para vecindarios, que conecta a residentes para discutir temas locales, compartir recomendaciones y alertas de seguridad en su entorno inmediato.</td>
<td>Waze es una aplicación de navegación que utiliza crowdsourcing para ofrecer rutas en tiempo real, evitando tráfico, accidentes y obstáculos viales.</td>
<td>UrbanVoice es una aplicación móvil enfocada en mejorar la seguridad ciudadana en Lima Metropolitana, proporcionando información y alertas de riesgo en tiempo real mediante colaboración ciudadana.</td>
</tr>
<tr class="even">
<td>¿Qué valor ofrece los clientes?</td>
<td><p>Seguridad y prevención: Identificación de áreas peligrosas.</p>
<p>Empoderamiento: Plataforma para denunciar incidentes de acoso.</p>
<p>Anonimato: Reportes seguros sin temor a represalias.</p></td>
<td><p>Conexión comunitaria: Facilita la interacción vecinal.</p>
<p>Vigilancia vecinal: Red de apoyo para reportar incidentes locales.</p>
<p>Recursos locales: Recomendaciones de servicios cercanos.</p></td>
<td><p>Eficiencia: Rutas optimizadas en tiempo real.</p>
<p>Seguridad vial: Información sobre peligros en carretera.</p>
<p>Comunidad activa: Datos precisos gracias a la contribución de usuarios.</p></td>
<td><p>Seguridad en tiempo real: Alertas inmediatas de situaciones de riesgo.</p>
<p>Colaboración: Nexo entre ciudadanos y autoridades.</p>
<p>Prevención: Información accionable para evitar áreas de alta criminalidad.</p></td>
</tr>
<tr class="odd">
<td rowspan="2"><strong>Perfil de Marketing</strong></td>
<td>Mercado objetivo</td>
<td>Mujeres en áreas urbanas preocupadas por el acoso y la seguridad de género.</td>
<td>Adultos y residentes locales interesados en la vida comunitaria y seguridad del vecindario.</td>
<td>Conductores que buscan optimizar sus tiempos de viaje en zonas urbanas congestionadas.</td>
<td>Ciudadanos de Lima Metropolitana que buscan herramientas proactivas para su seguridad personal y comunitaria.</td>
</tr>
<tr class="even">
<td>Estrategias de Marketing</td>
<td>Campañas con ONGs, movimientos sociales y marketing comunitario enfocado en género.</td>
<td>Marketing de boca en boca, publicidad en redes sociales segmentada por vecindarios y alianzas vecinales.</td>
<td>Alianzas con empresas automotrices, publicidad geolocalizada y programas de incentivos para colaboradores.</td>
<td>Campañas de concienciación en Lima, publicidad digital segmentada y relaciones públicas en medios locales.</td>
</tr>
<tr class="odd">
<td rowspan="3"><strong>Perfil del producto</strong></td>
<td>Producto &amp; Servicios</td>
<td>App móvil (iOS/Android) y plataforma de datos agregados para organizaciones de seguridad.</td>
<td>Red social vecinal, alertas de seguridad y servicios de anuncios locales para negocios.</td>
<td>Navegación GPS, alertas de tráfico en tiempo real e integración con servicios de música/mapas.</td>
<td>App móvil con mapas interactivos de seguridad, alertas basadas en ubicación y plataforma de datos para análisis criminalístico local.</td>
</tr>
<tr class="even">
<td>Precios &amp; Costos</td>
<td>Modelo freemium: Gratis para usuarios; suscripciones para acceso a analítica de datos avanzada.</td>
<td>Gratuito para usuarios; ingresos mediante publicidad pagada de empresas y servicios locales.</td>
<td>Gratuito; ingresos generados por publicidad geolocalizada dentro de la interfaz.</td>
<td>Modelo freemium: Gratis para ciudadanos; suscripción para empresas o entidades que requieran análisis de datos detallados.</td>
</tr>
<tr class="odd">
<td>Canales de distribución</td>
<td>Móvil (App Store/Play Store) y plataforma Web complementaria.</td>
<td>Móvil y plataforma Web para acceso desde escritorio.</td>
<td>Principalmente Móvil; herramientas de planificación vía Web.</td>
<td>Móvil (Android/iOS) y plataforma Web interactiva para mapas de riesgo.</td>
</tr>
<tr class="even">
<td rowspan="4"><strong>Análisis SWOT</strong></td>
<td>Fortalezas</td>
<td>Especialización en seguridad personal y fuerte impacto social positivo.</td>
<td>Red hiperlocal consolidada y gran base de usuarios internacionales.</td>
<td>Líder en navegación en tiempo real con integración tecnológica avanzada.</td>
<td>Enfoque específico en la problemática de Lima y colaboración directa con autoridades locales.</td>
</tr>
<tr class="odd">
<td>Debilidades</td>
<td>Alcance limitado fuera de áreas urbanas; dependencia total de los reportes.</td>
<td>Problemas de privacidad de datos y complejidad en la moderación de contenido.</td>
<td>Alto consumo de batería y datos; no orientado a la seguridad criminal personal.</td>
<td>Focalización geográfica inicial limitada; costos operativos de mantenimiento tecnológico.</td>
</tr>
<tr class="even">
<td>Oportunidades</td>
<td>Expansión geográfica a nuevas ciudades con crisis de seguridad.</td>
<td>Integración de nuevas funciones de Marketplace y eventos comunitarios.</td>
<td>Colaboración con gobiernos para Smart Cities y gestión de tráfico masivo.</td>
<td>Escalabilidad a otras capitales de Latinoamérica con desafíos similares de inseguridad.</td>
</tr>
<tr class="odd">
<td>Amenazas</td>
<td>Nuevas regulaciones de datos y competencia de apps de seguridad generalistas.</td>
<td>Competencia de grandes plataformas (Facebook/Nextdoor clones) y saturación.</td>
<td>Mejoras constantes en Google Maps y Apple Maps que absorben sus funciones.</td>
<td>Cambios normativos de privacidad en Perú y competencia de aplicaciones estatales.</td>
</tr>
</tbody>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores 

**1. Diferenciación por Especialización Local:**

 El valor principal de UrbanVoice reside en su enfoque exclusivo en Lima Metropolitana. A diferencia de competidores globales que manejan datos genéricos, nosotros nos enfocamos en entender la dinámica de seguridad de cada distrito limeño. La idea es posicionarnos como la herramienta que mejor conoce la realidad de nuestras calles, logrando una relevancia que aplicaciones más grandes no pueden alcanzar por su falta de contexto local.

**2. Fomento de la Participación Ciudadana:**

Para que la aplicación sea útil, necesitamos que la comunidad sea el motor de la información. No se trata solo de que los usuarios miren el mapa, sino de incentivarlos a ser parte activa del cambio. Implementaremos dinámicas que reconozcan el compromiso de los ciudadanos que reportan, creando un sentido de pertenencia y asegurando que la información siempre esté actualizada y sea confiable para todos.

**3. Alianzas Estratégicas:**

 Buscamos que UrbanVoice no sea una isla, sino un puente entre el ciudadano y las instituciones de seguridad. El objetivo es trabajar de la mano con serenazgos, ONGs y juntas vecinales para que los reportes de la app tengan un respaldo real. Estas alianzas nos darán la credibilidad necesaria para que el usuario sienta que su participación realmente contribuye a una respuesta efectiva en su seguridad.

**4. Expansión Geográfica Controlada:**

 Nuestra visión a largo plazo es llevar este modelo a otras ciudades del Perú que enfrentan desafíos similares. Una vez que hayamos perfeccionado el sistema en Lima, replicaremos la estrategia en regiones clave, adaptando la comunicación y el análisis a las necesidades específicas de cada ciudad para asegurar que el impacto sea igual de positivo que en la capital.

**5. Innovación en Funcionalidades:**

 Para mantenernos un paso adelante de la competencia, UrbanVoice integrará funciones diseñadas específicamente para situaciones críticas de seguridad ciudadana. Esto incluye desde alertas personalizadas según la ubicación del usuario hasta botones de asistencia rápida. Queremos ofrecer una herramienta integral que no solo informe, sino que brinde soluciones prácticas y directas cuando el usuario más lo necesita.

## 2.2. Entrevistas

El propósito de estas entrevistas es profundizar en las preocupaciones, necesidades y expectativas reales de nuestro segmento objetivo: ciudadanos que transitan por espacios públicos y priorizan su seguridad personal. A través de este diálogo, buscamos identificar patrones de comportamiento y oportunidades de solución que validen la propuesta de valor de UrbanVoice.

### 2.2.1. Diseño de entrevistas

Para el registro inicial y perfilamiento del entrevistado, se solicitarán los siguientes datos:
*Nombres y Apellidos, edad, ocupación y pasatiempos.*

**Segmento Objetivo: Ciudadanos preocupados por su seguridad en espacios públicos**

1. ¿Podría describir alguna situación reciente en la que se haya sentido vulnerable o preocupado por su integridad en un espacio público?
*Objetivo: Identificar contextos específicos y factores detonantes de la sensación de inseguridad.*

2. ¿Qué medidas o precauciones toma habitualmente para mitigar riesgos cuando se desplaza por la ciudad?
*Objetivo: Conocer los métodos preventivos y herramientas actuales que utiliza el usuario.*

3. ¿Qué elementos del entorno (falta de iluminación, escasa vigilancia, zonas desoladas, etc.) influyen más en su percepción de peligro?
*Objetivo: Determinar los factores del entorno urbano que UrbanVoice debería priorizar en sus reportes.*

4. Ante un incidente de inseguridad (como testigo o víctima), ¿cuál suele ser su reacción inmediata y qué dificultades encuentra para actuar?
*Objetivo: Entender la respuesta emocional y operativa del ciudadano frente al riesgo.*

5. ¿Qué información o alertas específicas consideraría indispensables recibir en su celular para sentirse más protegido mientras transita?
*Objetivo: Definir las funcionalidades críticas y el tipo de contenido más valioso para la app.*

6. ¿Cuál es su nivel de confianza al usar herramientas digitales para reportar delitos o recibir alertas de seguridad?
*Objetivo: Medir la disposición tecnológica y posibles barreras de adopción.*

7. ¿Ha tenido experiencia previa con aplicaciones de seguridad? Si es así, ¿qué aspectos resultaron útiles y cuáles fueron frustrantes?
*Objetivo: Analizar la competencia desde la experiencia del usuario para evitar errores de diseño.*

8. ¿Considera que compartir su ubicación en tiempo real con sus contactos de confianza es una función esencial o secundaria para su tranquilidad?
*Objetivo: Validar el interés en herramientas de monitoreo preventivo.*

9. Más allá de las alertas, ¿qué otra funcionalidad creativa o herramienta adicional cree que le daría un mayor control sobre su seguridad diaria?
*Objetivo: Explorar ideas innovadoras que puedan diferenciar a UrbanVoice en el mercado.*

### 2.2.2. Registro de entrevistas 

**Entrevista N°1:**

![Entrevista3](assets/Entrevista3.png)

**Timing:** 19:27

**Nombre**: Marcia Mascco  

**Edad:** 21 años

**Pasatiempos:** Jugar videojuegos con su enamorado o amigos

**Ocupación:** Estudiante de la carrera de Administración y Marketing

La entrevistada no se siente segura en lugares donde no hay mucha iluminación ya que, como menciona, habia una zona por su residencia que estaba totalmente oscura y era zona donde robaban mucho. Afortunadamente, no ha sido victima de algún robo o alguna situación peligrosa, pero ante situaciones peligrosas ella indica que auxiliaria al afectado, dando su celular para llamar o bloquear dependiendo de lo que le hayan robado. Ella se siente cómoda y segura recibiendo alertas en su celuar, argumenta que revisa cada tanto algunas situaciones con alertas como, por ejemplo, google maps que manda alertas de tráfico o accidentes en alguna carretera. No ha usado apps de seguridad antes pero esta abierta a recibir una que le permita sentirse más segura en la vía pública y valora mucho las funcionalidades de alertas y de compartir ubicación en tiempo real.

### 2.2.3. Análisis de entrevistas

A continuación, se presenta la síntesis de los datos obtenidos durante la fase de entrevistas, categorizando las preocupaciones principales, los factores del entorno y las funcionalidades priorizadas por el segmento objetivo.

#### Factores de Inseguridad Identificados
| Categoría | Hallazgo del Usuario | Impacto en la Percepción |
| :--- | :--- | :--- |
| **Zonas Críticas** | Áreas cercanas a universidades y parques públicos. | Alta sensación de vulnerabilidad en trayectos cotidianos. |
| **Entorno Físico** | Deficiente iluminación en calles residenciales y paraderos. | Factor determinante para evitar rutas específicas. |
| **Vigilancia** | Escasa presencia de autoridades o seguridad privada. | Sensación de abandono ante posibles incidentes. |
| **Experiencia Social** | Alta frecuencia como testigos de actos delictivos en su entorno. | Necesidad apremiante de soluciones tecnológicas de mitigación. |

#### Requerimientos y Funcionalidades Prioritarias
| Requerimiento | Descripción Técnica / Interés del Usuario | Valor Agregado Identificado |
| :--- | :--- | :--- |
| **Reportes en Tiempo Real** | Capacidad de registrar incidencias de forma inmediata y sencilla. | Mecanismo de alerta ciudadana y facilitador para autoridades. |
| **Alertas Geofencing** | Recepción de notificaciones automáticas al ingresar a áreas de riesgo. |Prevención activa ante robos o delitos recientes en el entorno. |
| **Seguimiento en Vivo** |Compartir ubicación en tiempo real con red de contactos. | Incremento de la tranquilidad durante desplazamientos críticos. |
| **Privacidad / Anonimato** | Opción de reportar y compartir ubicación sin revelar identidad. | Mitigación de temor a represalias y protección de datos. |

#### Disposición Tecnológica y Barreras
| Dimensión | Estado Actual | Observación de los Entrevistados |
| :--- | :--- | :--- |
| **Confianza Digital** | Media / Alta. | Los usuarios ya utilizan apps de mapas para informarse (tráfico/accidentes). |
| **Experiencia Previa** |Baja. | La mayoría no ha utilizado aplicaciones dedicadas exclusivamente a seguridad. |
| **Apertura al Cambio** | Muy Alta. | Existe una disposición inmediata a adoptar herramientas que mejoren la seguridad pública. |

## 2.3. Needfinding

### 2.3.1. User Personas 

![](assets/Adriana%20Valdivia.png)


### 2.3.2. User Task Matrix

La siguiente matriz detalla las tareas y acciones que el segmento objetivo realiza actualmente para gestionar su seguridad. Esto nos permite identificar los "gaps" donde la app puede intervenir para mejorar la experiencia del usuario.

| Categoría de Tarea | Tareas Específicas del Usuario | Frecuencia | Importancia |
| :--- | :--- | :--- | :--- |
| **Prevención y Planificación** | Consultar con familiares o amigos sobre la seguridad de una ruta o zona antes de visitarla. | Siempre | Alta |
| | Evitar desplazamientos en horarios nocturnos o por lugares con reputación de peligrosidad. | Siempre | Alta |
| | Buscar noticias sobre incidentes recientes en redes sociales (Facebook, grupos de WhatsApp). | A veces | Media |
| **Acción y Respuesta** | Contactar a la policía o servicios de emergencia (105 / Serenazgo) ante una amenaza directa. | Casi nunca | Alta |
| | Organizarse activamente con vecinos o juntas locales para mejorar la seguridad comunitaria. | Nunca | Media |
| | Portar objetos de autodefensa personal (gas pimienta, alarmas sonoras, etc.). | Nunca | Media |
| **Uso de Tecnología** | Utilizar aplicaciones de mapas (Google Maps/Waze) específicamente para evadir zonas peligrosas. | Nunca | Media |
| | Reportar incidentes en tiempo real a través de plataformas digitales o aplicaciones móviles. | Nunca | Media |

---

#### Análisis de la Matriz
* Los usuarios dependen casi exclusivamente de su red de contactos directa y de evitar el peligro físicamente, lo que indica una falta de herramientas digitales confiables.
* Aunque llamar a la policía es de alta importancia, la frecuencia es "Casi nunca", lo que sugiere desconfianza en los tiempos de respuesta o dificultad para realizar la llamada en una emergencia.
* Existe un uso nulo ("Nunca") de aplicaciones para reportar o evadir zonas peligrosas, lo que representa un océano azul para UrbanVoice si logra simplificar esta tarea.

### 2.3.3. Empathy Journey Mappping

![Empathy Journey Mappping](assets/Matrix.png)

### 2.3.4. Empathy Mappping

![Empathy Journey Mappping](assets//Empathy%20map.png)

Con ayuda del gráfico Empathy Mapping podemos conocer las necesidades, frustraciones de nuestro segmento objetivo: **Ciudadanos preocupados por su seguridad en espacios públicos**. Esto nos ofrece una comprensión más profunda de cómo se siente nuestro usuario y abordar una solución que
realmente los ayuden.

### 2.3.5. Big Picture EventStorming

Para la definición del ecosistema de UrbanVoice, el equipo llevó a cabo una sesión colaborativa de Big Picture Event Storming, un método visual que nos permitió mapear de extremo a extremo el dominio del negocio.

![EventStorming](assets/EventStoarming%20-%20UrbanVoice.jpg)

Puedes explorar el flujo completo, los eventos de dominio y las definiciones técnicas en tiempo real a través de nuestro tablero de Miro en el siguiente enlace:
https://miro.com/app/board/uXjVGhQGySg=/?share_link_id=739088953987

### 2.3.6. Ubiquitous Language
En esta sección se definen los términos clave del dominio de negocio. Estas definiciones eliminan ambigüedades y aseguran que todos los involucrados compartan una comprensión común de los conceptos de seguridad ciudadana.

| Término | Definición |
| :--- | :--- |
| **Seguridad Ciudadana** | Acción integrada que desarrolla el Estado, con la colaboración de la ciudadanía, para asegurar su convivencia pacífica, la erradicación de la violencia y la utilización pacífica de las vías y espacios públicos. |
| **Incidente** | Cualquier evento o suceso que represente un riesgo para la integridad física o patrimonial del ciudadano, incluyendo robos, hurtos, acoso o actos vandálicos. |
| **Punto Crítico** | Zona geográfica específica dentro de la ciudad que presenta una alta recurrencia o densidad de incidentes reportados en un periodo determinado. |
| **Alerta en Tiempo Real** | Notificación inmediata enviada a los usuarios sobre un peligro o incidente que está ocurriendo o acaba de ocurrir en su cercanía geográfica. |
| **Ruta Segura** | Trayecto sugerido entre dos puntos que prioriza vías con menor índice de criminalidad, mejor iluminación y mayor presencia de autoridades. |
| **Reporte Ciudadano** | Acto voluntario de un usuario de registrar y compartir información sobre un incidente presenciado o experimentado para alertar a la comunidad. |
| **Mapa de Riesgo** | Representación visual interactiva que utiliza datos históricos y en tiempo real para mostrar los niveles de inseguridad en diferentes sectores de la ciudad. |
| **Acoso Callejero** | Prácticas de naturaleza sexual no consentidas que ocurren en espacios públicos, que afectan la dignidad y el derecho a la libre circulación de las personas. |
| **Botón de Pánico** | Funcionalidad de emergencia que permite al usuario enviar una señal de auxilio inmediata a sus contactos de confianza y a las autoridades competentes. |
| **Círculo de Confianza** | Grupo selecto de contactos (familiares o amigos) con los cuales el usuario decide compartir su ubicación o recibir notificaciones de emergencia. |
| **Espacio Público** | Áreas de la ciudad de libre acceso y circulación, como calles, parques, paraderos y plazas, donde se desarrolla la vida comunitaria. |
| **Tiempo de Respuesta** | Intervalo que transcurre desde que se reporta una emergencia hasta que las autoridades (Serenazgo o Policía) intervienen en el lugar del suceso. |

## 2.4. Requirements specification
### 2.4.1. User Stories
A continuación se detalla la especificación de requisitos del sistema dividida en Épicas, Historias de Usuario y Criterios de Aceptación por escenarios.

  
<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US01</td>
    <td align="center">Visitante</td>
    <td align="center">Alta</td>
    <td align="center">EP01</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Registrarse en la plataforma</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como visitante, quiero registrarme en UrbanVoice proporcionando mis datos básicos para acceder a las funcionalidades de la plataforma.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Registro exitoso.</b><br>
      <b>Given</b> que el visitante ingresa nombre, correo y contraseña válidos,<br>
      <b>When</b> envía el formulario de registro,<br>
      <b>Then</b> el sistema crea la cuenta y redirige al inicio de sesión.<br><br>
      <b>Escenario 2: Correo duplicado.</b><br>
      <b>Given</b> que el correo ya está registrado,<br>
      <b>When</b> el visitante intenta registrarse,<br>
      <b>Then</b> el sistema muestra un mensaje de error indicando que el correo ya existe.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US02</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP01</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Iniciar sesión en la plataforma</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano registrado, quiero iniciar sesión con mis credenciales para acceder a las funcionalidades de UrbanVoice.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Inicio de sesión exitoso.</b><br>
      <b>Given</b> que el ciudadano ingresa correo y contraseña correctos,<br>
      <b>When</b> presiona el botón de iniciar sesión,<br>
      <b>Then</b> el sistema autentica al usuario y muestra el mapa principal.<br><br>
      <b>Escenario 2: Credenciales inválidas.</b><br>
      <b>Given</b> que el ciudadano ingresa una contraseña incorrecta,<br>
      <b>When</b> intenta iniciar sesión,<br>
      <b>Then</b> el sistema muestra un mensaje de error y no concede el acceso.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US03</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP01</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Recuperar contraseña olvidada</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero recuperar mi contraseña mediante mi correo electrónico para restablecer el acceso a mi cuenta.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Envío de correo de recuperación.</b><br>
      <b>Given</b> que el ciudadano solicita restablecer su contraseña,<br>
      <b>When</b> ingresa su correo registrado,<br>
      <b>Then</b> el sistema envía un enlace de recuperación al correo.<br><br>
      <b>Escenario 2: Correo no registrado.</b><br>
      <b>Given</b> que el ciudadano ingresa un correo no registrado,<br>
      <b>When</b> solicita la recuperación,<br>
      <b>Then</b> el sistema muestra un mensaje indicando que el correo no existe.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US04</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Visualizar mapa de incidentes</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero visualizar un mapa con los incidentes reportados cerca de mi ubicación para estar informado sobre la situación de seguridad en mi zona.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Carga inicial del mapa.</b><br>
      <b>Given</b> que el ciudadano accede a la pantalla principal,<br>
      <b>When</b> el mapa se carga,<br>
      <b>Then</b> el sistema muestra marcadores de incidentes en un radio de 5 km.<br><br>
      <b>Escenario 2: Sin incidentes cercanos.</b><br>
      <b>Given</b> que no hay reportes en la zona,<br>
      <b>When</b> el mapa se renderiza,<br>
      <b>Then</b> el sistema muestra un mensaje indicando que no hay incidentes cercanos.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US05</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Registrar incidente en el mapa</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero registrar un incidente de inseguridad seleccionando su ubicación en el mapa para alertar a otros usuarios.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Registro con geolocalización.</b><br>
      <b>Given</b> que el ciudadano completa los datos del reporte,<br>
      <b>When</b> selecciona publicar,<br>
      <b>Then</b> el sistema almacena el incidente con su ubicación GPS.<br><br>
      <b>Escenario 2: GPS desactivado.</b><br>
      <b>Given</b> que el GPS está desactivado,<br>
      <b>When</b> el ciudadano intenta reportar,<br>
      <b>Then</b> el sistema solicita habilitar la ubicación antes de continuar.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US06</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Adjuntar evidencia multimedia al reporte</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero adjuntar fotos o videos al reporte de incidente para proporcionar evidencia visual del suceso.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Adjuntar desde galería.</b><br>
      <b>Given</b> que el ciudadano está creando un reporte,<br>
      <b>When</b> selecciona una imagen de la galería,<br>
      <b>Then</b> el sistema la adjunta y muestra una vista previa.<br><br>
      <b>Escenario 2: Archivo muy pesado.</b><br>
      <b>Given</b> que el ciudadano intenta subir un archivo de más de 10 MB,<br>
      <b>When</b> el sistema valida el tamaño,<br>
      <b>Then</b> muestra un mensaje indicando que el tamaño máximo es 10 MB.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US07</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Visualizar detalle de un incidente</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero ver el detalle de un incidente específico para conocer tipo, fecha, descripción y evidencia disponible.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Visualización de información completa.</b><br>
      <b>Given</b> que el ciudadano selecciona un marcador en el mapa,<br>
      <b>When</b> presiona "Ver detalle",<br>
      <b>Then</b> el sistema muestra tipo, fecha, descripción, evidencia y estado del incidente.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US08</td>
    <td align="center">Visitante</td>
    <td align="center">Baja</td>
    <td align="center">EP06</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Explorar landing page informativa</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como visitante, quiero explorar la landing page de UrbanVoice para conocer las funcionalidades y beneficios de la plataforma.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Navegación por secciones.</b><br>
      <b>Given</b> que el visitante ingresa a la URL de UrbanVoice,<br>
      <b>When</b> se desplaza por la página,<br>
      <b>Then</b> el sistema muestra las secciones de funcionalidades, beneficios y contacto.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US09</td>
    <td align="center">Visitante institucional</td>
    <td align="center">Media</td>
    <td align="center">EP06</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Registrar solicitud de alianza institucional</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como visitante institucional, quiero enviar una solicitud de contacto desde la landing page para proponer alianzas con UrbanVoice.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Envío exitoso.</b><br>
      <b>Given</b> que el visitante completa el formulario de contacto,<br>
      <b>When</b> presiona enviar,<br>
      <b>Then</b> el sistema muestra un mensaje de confirmación y notifica al equipo.<br><br>
      <b>Escenario 2: Campos obligatorios vacíos.</b><br>
      <b>Given</b> que el visitante deja campos requeridos sin completar,<br>
      <b>When</b> intenta enviar,<br>
      <b>Then</b> el sistema resalta los campos faltantes y no envía el formulario.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US10</td>
    <td align="center">Visitante</td>
    <td align="center">Baja</td>
    <td align="center">EP06</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Consultar información de contacto y redes sociales</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como visitante, quiero consultar la información de contacto y redes sociales de UrbanVoice para seguir la plataforma y comunicarme con el equipo.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Visualización de contacto.</b><br>
      <b>Given</b> que el visitante se encuentra en la landing page,<br>
      <b>When</b> se desplaza a la sección de contacto,<br>
      <b>Then</b> el sistema muestra correo, redes sociales y enlaces funcionales.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US11</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Realizar reporte anónimo</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero realizar un reporte de incidente de forma anónima para proteger mi identidad mientras contribuyo a la seguridad ciudadana.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Publicación anónima.</b><br>
      <b>Given</b> que el ciudadano activa el modo anónimo en el formulario,<br>
      <b>When</b> envía el reporte,<br>
      <b>Then</b> el sistema oculta el nombre del autor en el mapa público.<br><br>
      <b>Escenario 2: Desactivación de anonimato.</b><br>
      <b>Given</b> que el ciudadano desactiva el modo anónimo,<br>
      <b>When</b> envía el reporte,<br>
      <b>Then</b> el sistema muestra su nombre de usuario como autor.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US12</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Filtrar incidentes por tipo y fecha</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero filtrar los incidentes en el mapa por tipo y rango de fechas para enfocarme en la información relevante.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Filtro por categoría.</b><br>
      <b>Given</b> que el ciudadano abre el panel de filtros,<br>
      <b>When</b> selecciona una categoría específica,<br>
      <b>Then</b> el mapa actualiza los marcadores mostrando solo los de esa categoría.<br><br>
      <b>Escenario 2: Filtro por rango de fechas.</b><br>
      <b>Given</b> que el ciudadano define una fecha inicio y fin,<br>
      <b>When</b> aplica el filtro,<br>
      <b>Then</b> el mapa muestra solo los incidentes dentro de ese período.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US13</td>
    <td align="center">Administrador</td>
    <td align="center">Alta</td>
    <td align="center">EP05</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Moderar reportes ciudadanos</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como administrador, quiero moderar los reportes de incidentes para aprobar o rechazar contenido inapropiado o falso.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Aprobación de reporte.</b><br>
      <b>Given</b> que el administrador revisa un reporte pendiente,<br>
      <b>When</b> selecciona aprobar,<br>
      <b>Then</b> el reporte se publica en el mapa público.<br><br>
      <b>Escenario 2: Rechazo de reporte.</b><br>
      <b>Given</b> que el administrador detecta un reporte falso,<br>
      <b>When</b> selecciona rechazar,<br>
      <b>Then</b> el reporte se elimina y el usuario recibe una notificación.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US14</td>
    <td align="center">Administrador</td>
    <td align="center">Media</td>
    <td align="center">EP05</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Gestionar categorías de incidentes</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como administrador, quiero gestionar las categorías de incidentes (crear, editar, desactivar) para mantener actualizada la taxonomía de reportes.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Crear nueva categoría.</b><br>
      <b>Given</b> que el administrador accede al panel de categorías,<br>
      <b>When</b> completa el formulario de nueva categoría,<br>
      <b>Then</b> la categoría se agrega a la lista disponible.<br><br>
      <b>Escenario 2: Desactivar categoría.</b><br>
      <b>Given</b> que una categoría ya no es relevante,<br>
      <b>When</b> el administrador la desactiva,<br>
      <b>Then</b> la categoría deja de aparecer en el formulario de reportes.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US15</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP04</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Recibir notificaciones de incidentes cercanos</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero recibir notificaciones push cuando ocurra un incidente cerca de mi ubicación para tomar precauciones inmediatas.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Notificación por proximidad.</b><br>
      <b>Given</b> que el sistema registra un nuevo incidente,<br>
      <b>When</b> el ciudadano se encuentra en un radio de 1 km,<br>
      <b>Then</b> el sistema envía una notificación push con los detalles del incidente.<br><br>
      <b>Escenario 2: Notificación con app en segundo plano.</b><br>
      <b>Given</b> que la aplicación está en segundo plano,<br>
      <b>When</b> ocurre un incidente cercano,<br>
      <b>Then</b> el sistema muestra la notificación en la barra de estado del dispositivo.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US16</td>
    <td align="center">Ciudadano</td>
    <td align="center">Alta</td>
    <td align="center">EP04</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Compartir ubicación en tiempo real</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero compartir mi ubicación en tiempo real con contactos de confianza para que puedan monitorear mi desplazamiento.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Inicio de compartición.</b><br>
      <b>Given</b> que el ciudadano selecciona un contacto de confianza,<br>
      <b>When</b> activa el seguimiento en tiempo real,<br>
      <b>Then</b> el sistema genera un enlace de monitoreo y lo envía al contacto.<br><br>
      <b>Escenario 2: Detener compartición.</b><br>
      <b>Given</b> que el ciudadano tiene la compartición activa,<br>
      <b>When</b> presiona "Detener",<br>
      <b>Then</b> el sistema finaliza el seguimiento y notifica al contacto.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US17</td>
    <td align="center">Contacto de confianza</td>
    <td align="center">Media</td>
    <td align="center">EP04</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Monitorear ubicación de un contacto</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como contacto de confianza, quiero monitorear la ubicación en tiempo real de un ciudadano que comparte su trayecto para velar por su seguridad.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Visualización en mapa.</b><br>
      <b>Given</b> que el contacto accede al enlace de monitoreo,<br>
      <b>When</b> el ciudadano se desplaza,<br>
      <b>Then</b> el mapa muestra la posición actualizada en tiempo real.<br><br>
      <b>Escenario 2: Contacto desconectado.</b><br>
      <b>Given</b> que el ciudadano detiene la compartición,<br>
      <b>When</b> el contacto intenta ver la ubicación,<br>
      <b>Then</b> el sistema muestra un mensaje indicando que el seguimiento terminó.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US18</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP04</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Activar o desactivar alertas por zona geográfica</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero activar o desactivar las alertas de incidentes cercanos para ciertas zonas geográficas para personalizar mi experiencia.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Desactivar alertas en una zona.</b><br>
      <b>Given</b> que el ciudadano configura sus preferencias,<br>
      <b>When</b> desactiva las alertas para una zona específica,<br>
      <b>Then</b> el sistema deja de notificar incidentes en esa zona.<br><br>
      <b>Escenario 2: Reactivar alertas.</b><br>
      <b>Given</b> que las alertas estaban desactivadas,<br>
      <b>When</b> el ciudadano las reactiva,<br>
      <b>Then</b> el sistema reanuda el envío de notificaciones de esa zona.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US19</td>
    <td align="center">Ciudadano</td>
    <td align="center">Baja</td>
    <td align="center">EP01</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Editar perfil de usuario</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero editar mi perfil (nombre, foto, preferencias) para mantener mis datos actualizados.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Actualización exitosa.</b><br>
      <b>Given</b> que el ciudadano accede a su perfil,<br>
      <b>When</b> modifica sus datos y guarda,<br>
      <b>Then</b> el sistema actualiza la información y muestra confirmación.<br><br>
      <b>Escenario 2: Foto de perfil inválida.</b><br>
      <b>Given</b> que el ciudadano intenta subir una foto en formato no soportado,<br>
      <b>When</b> el sistema valida el archivo,<br>
      <b>Then</b> muestra un mensaje indicando los formatos aceptados (JPG, PNG).
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US20</td>
    <td align="center">Ciudadano</td>
    <td align="center">Baja</td>
    <td align="center">EP01</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Cerrar sesión</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero cerrar sesión en la aplicación para proteger mi cuenta en dispositivos compartidos.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Cierre de sesión exitoso.</b><br>
      <b>Given</b> que el ciudadano está autenticado,<br>
      <b>When</b> selecciona "Cerrar sesión",<br>
      <b>Then</b> el sistema invalida el token y redirige a la pantalla de inicio de sesión.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US21</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP04</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Gestionar contactos de confianza</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero gestionar mi lista de contactos de confianza (agregar, eliminar) para compartir mi ubicación con personas de confianza.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Agregar contacto.</b><br>
      <b>Given</b> que el ciudadano accede a sus contactos,<br>
      <b>When</b> ingresa el correo de un usuario registrado,<br>
      <b>Then</b> el sistema agrega el contacto a la lista.<br><br>
      <b>Escenario 2: Eliminar contacto.</b><br>
      <b>Given</b> que el ciudadano selecciona un contacto existente,<br>
      <b>When</b> confirma la eliminación,<br>
      <b>Then</b> el sistema remueve el contacto de la lista.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US22</td>
    <td align="center">Ciudadano</td>
    <td align="center">Media</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Visualizar heatmap de zonas de riesgo</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero visualizar un heatmap (mapa de calor) sobre el mapa para identificar las zonas con mayor concentración de incidentes.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Activación de heatmap.</b><br>
      <b>Given</b> que el ciudadano está en el mapa,<br>
      <b>When</b> activa la capa de heatmap,<br>
      <b>Then</b> el sistema superpone un gradiente de color según la densidad de incidentes.<br><br>
      <b>Escenario 2: Desactivación de heatmap.</b><br>
      <b>Given</b> que el heatmap está activo,<br>
      <b>When</b> el ciudadano desactiva la capa,<br>
      <b>Then</b> el mapa vuelve a la vista de marcadores normal.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US23</td>
    <td align="center">Administrador</td>
    <td align="center">Media</td>
    <td align="center">EP05</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Generar reporte estadístico de incidentes</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como administrador, quiero generar reportes estadísticos de incidentes por período, zona y categoría para analizar tendencias de seguridad.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Generación de reporte.</b><br>
      <b>Given</b> que el administrador selecciona filtros de fecha y zona,<br>
      <b>When</b> solicita generar reporte,<br>
      <b>Then</b> el sistema muestra gráficos y tablas con los datos agregados.<br><br>
      <b>Escenario 2: Exportación de reporte.</b><br>
      <b>Given</b> que el reporte está generado,<br>
      <b>When</b> el administrador selecciona exportar,<br>
      <b>Then</b> el sistema descarga el reporte en formato PDF o CSV.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US24</td>
    <td align="center">Administrador</td>
    <td align="center">Baja</td>
    <td align="center">EP05</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Enviar notificaciones masivas desde administración</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como administrador, quiero enviar notificaciones push masivas a los usuarios para comunicar alertas generales o información importante.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Envío masivo exitoso.</b><br>
      <b>Given</b> que el administrador redacta un mensaje,<br>
      <b>When</b> selecciona "Enviar a todos",<br>
      <b>Then</b> el sistema envía la notificación push a todos los usuarios registrados.<br><br>
      <b>Escenario 2: Confirmación de envío.</b><br>
      <b>Given</b> que el administrador envió una notificación masiva,<br>
      <b>When</b> el proceso finaliza,<br>
      <b>Then</b> el sistema muestra el número de usuarios notificados exitosamente.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US25</td>
    <td align="center">Ciudadano</td>
    <td align="center">Baja</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Visualizar historial de incidentes reportados</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero ver el historial de todos los incidentes que he reportado para darles seguimiento.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Listado de mis reportes.</b><br>
      <b>Given</b> que el ciudadano accede a "Mis reportes",<br>
      <b>When</b> la lista se carga,<br>
      <b>Then</b> el sistema muestra todos sus incidentes con estado, fecha y tipo.<br><br>
      <b>Escenario 2: Historial vacío.</b><br>
      <b>Given</b> que el ciudadano nunca ha reportado,<br>
      <b>When</b> accede a "Mis reportes",<br>
      <b>Then</b> el sistema muestra un mensaje indicando que no tiene reportes registrados.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US26</td>
    <td align="center">Ciudadano</td>
    <td align="center">Baja</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Recibir confirmación de reporte procesado</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero recibir una confirmación cuando mi reporte sea procesado por un administrador para saber su estado.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Reporte aprobado.</b><br>
      <b>Given</b> que el administrador aprueba el reporte,<br>
      <b>When</b> el estado cambia a "aprobado",<br>
      <b>Then</b> el sistema notifica al ciudadano que su reporte fue publicado.<br><br>
      <b>Escenario 2: Reporte rechazado.</b><br>
      <b>Given</b> que el administrador rechaza el reporte,<br>
      <b>When</b> el estado cambia a "rechazado",<br>
      <b>Then</b> el sistema notifica al ciudadano con el motivo del rechazo.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">US27</td>
    <td align="center">Ciudadano</td>
    <td align="center">Baja</td>
    <td align="center">EP02</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Valorar utilidad de reportes de otros usuarios</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como ciudadano, quiero valorar (like/dislike) los reportes de otros usuarios para destacar la información útil.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Votar reporte.</b><br>
      <b>Given</b> que el ciudadano ve el detalle de un incidente,<br>
      <b>When</b> presiona el botón "Útil",<br>
      <b>Then</b> el sistema registra el voto y actualiza el contador.<br><br>
      <b>Escenario 2: Cambiar voto.</b><br>
      <b>Given</b> que el ciudadano ya votó un reporte,<br>
      <b>When</b> presiona nuevamente,<br>
      <b>Then</b> el sistema revierte el voto anterior.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS01</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Configurar infraestructura cloud y pipeline CI/CD</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero configurar la infraestructura en la nube y el pipeline de integración continua para automatizar el despliegue del backend.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Pipeline de build exitoso.</b><br>
      <b>Given</b> que se realiza un push a la rama principal,<br>
      <b>When</b> el pipeline se ejecuta,<br>
      <b>Then</b> el sistema compila, ejecuta pruebas y despliega automáticamente.<br><br>
      <b>Escenario 2: Falla en pruebas.</b><br>
      <b>Given</b> que el pipeline encuentra pruebas fallidas,<br>
      <b>When</b> se ejecuta la etapa de tests,<br>
      <b>Then</b> el pipeline se detiene y notifica al equipo del error.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS02</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar autenticación JWT en el backend</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar autenticación basada en tokens JWT en el backend para asegurar los endpoints de la API.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Generación de token.</b><br>
      <b>Given</b> que el usuario inicia sesión correctamente,<br>
      <b>When</b> el servidor valida las credenciales,<br>
      <b>Then</b> el sistema retorna un token JWT con tiempo de expiración.<br><br>
      <b>Escenario 2: Token expirado.</b><br>
      <b>Given</b> que un request usa un token vencido,<br>
      <b>When</b> el middleware valida,<br>
      <b>Then</b> el sistema retorna código 401 (Unauthorized).
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS03</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar API REST de incidentes</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar los endpoints REST para el módulo de incidentes (CRUD y consultas geolocalizadas).</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Creación de incidente.</b><br>
      <b>Given</b> que el cliente envía un JSON con datos válidos,<br>
      <b>When</b> se realiza un POST a /api/incidents,<br>
      <b>Then</b> el sistema retorna código 201 con el ID del incidente creado.<br><br>
      <b>Escenario 2: Consulta por radio.</b><br>
      <b>Given</b> que el cliente envía coordenadas y radio,<br>
      <b>When</b> se realiza un GET a /api/incidents/nearby,<br>
      <b>Then</b> el sistema retorna los incidentes dentro del área especificada.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS04</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar API REST de alertas y geolocalización</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar los endpoints para el módulo de alertas, compartición de ubicación y notificaciones push.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Registro de suscripción a alertas.</b><br>
      <b>Given</b> que el cliente envía un token FCM válido,<br>
      <b>When</b> se realiza un POST a /api/alerts/subscribe,<br>
      <b>Then</b> el sistema registra el dispositivo para recibir notificaciones.<br><br>
      <b>Escenario 2: Compartición de ubicación.</b><br>
      <b>Given</b> que el ciudadano inicia el seguimiento,<br>
      <b>When</b> el cliente envía coordenadas periódicamente,<br>
      <b>Then</b> el sistema actualiza la ubicación y la pone disponible para el contacto.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS05</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Integrar Google Maps SDK en aplicaciones móviles</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero integrar el SDK de Google Maps en las apps Android y Flutter para mostrar el mapa de incidentes con marcadores y heatmap.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Mapa con marcadores.</b><br>
      <b>Given</b> que la app se inicializa,<br>
      <b>When</b> el mapa se carga con datos de la API,<br>
      <b>Then</b> los marcadores de incidentes se renderizan en las coordenadas correctas.<br><br>
      <b>Escenario 2: Heatmap funcional.</b><br>
      <b>Given</b> que se activa la capa de heatmap,<br>
      <b>When</b> los datos se procesan,<br>
      <b>Then</b> el mapa muestra el gradiente de densidad de incidentes.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS06</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP08</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar pruebas unitarias y de integración</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar pruebas unitarias y de integración para garantizar la calidad del backend y detectar regresiones.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Pruebas unitarias pasan.</b><br>
      <b>Given</b> que se ejecuta el suite de pruebas,<br>
      <b>When</b> todas las pruebas unitarias se completan,<br>
      <b>Then</b> el sistema reporta 100% de pruebas pasadas en los servicios core.<br><br>
      <b>Escenario 2: Cobertura mínima.</b><br>
      <b>Given</b> que se mide la cobertura de código,<br>
      <b>When</b> se ejecuta el reporte de cobertura,<br>
      <b>Then</b> el sistema verifica que la cobertura sea al menos del 70%.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS07</td>
    <td align="center">Developer</td>
    <td align="center">Media</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar WebSockets para actualizaciones en tiempo real</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar WebSockets en el backend para notificar cambios en tiempo real a los clientes conectados.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Conexión WebSocket exitosa.</b><br>
      <b>Given</b> que el cliente se suscribe al canal de incidentes,<br>
      <b>When</b> se establece la conexión WebSocket,<br>
      <b>Then</b> el cliente recibe eventos en tiempo real.<br><br>
      <b>Escenario 2: Reconexión automática.</b><br>
      <b>Given</b> que la conexión se pierde,<br>
      <b>When</b> el cliente detecta la desconexión,<br>
      <b>Then</b> el sistema intenta reconectarse automáticamente cada 3 segundos.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS08</td>
    <td align="center">Developer</td>
    <td align="center">Media</td>
    <td align="center">EP07</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Implementar sistema de caché y optimización de consultas</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero implementar un sistema de caché (Redis) para optimizar las consultas geolocalizadas y reducir la latencia.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Datos en caché.</b><br>
      <b>Given</b> que una consulta ya fue realizada antes,<br>
      <b>When</b> se repite la misma consulta,<br>
      <b>Then</b> el sistema retorna los datos desde caché en menos de 50 ms.<br><br>
      <b>Escenario 2: Invalidación de caché.</b><br>
      <b>Given</b> que se crea un nuevo incidente,<br>
      <b>When</b> el incidente se almacena,<br>
      <b>Then</b> el sistema invalida la caché de consultas cercanas.
    </td>
  </tr>
</table>

<br>

<table>
  <tr>
    <th style="text-align:center;">Story ID</th>
    <th style="text-align:center;">User</th>
    <th style="text-align:center;">Priority</th>
    <th style="text-align:center;">Epic</th>
  </tr>
  <tr>
    <td align="center">TS09</td>
    <td align="center">Developer</td>
    <td align="center">Alta</td>
    <td align="center">EP08</td>
  </tr>
  <tr>
    <td><b>Title</b></td>
    <td colspan="3">Realizar pruebas de seguridad y penetración</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Description</b></td>
  </tr>
  <tr>
    <td colspan="4">Como developer, quiero realizar pruebas de seguridad y penetración en la API para identificar y corregir vulnerabilidades antes del despliegue final.</td>
  </tr>
  <tr>
    <td colspan="4" align="center"><b>Acceptance Criteria</b></td>
  </tr>
  <tr>
    <td colspan="4">
      <b>Escenario 1: Prueba de inyección SQL.</b><br>
      <b>Given</b> que se envía un payload malicioso en los parámetros,<br>
      <b>When</b> el endpoint procesa la solicitud,<br>
      <b>Then</b> el sistema rechaza la entrada y retorna código 400.<br><br>
      <b>Escenario 2: Prueba de autenticación.</b><br>
      <b>Given</b> que se intenta acceder a un endpoint protegido sin token,<br>
      <b>When</b> se realiza la solicitud,<br>
      <b>Then</b> el sistema retorna código 401 y bloquea el acceso.
    </td>
  </tr>
</table>

### Spike Stories

#### **Spike 1: Investigación de Integración con Google Maps y Geolocalización**

**Contexto**
La plataforma UrbanVoice requiere una visualización fluida de "capas de calor" (Heatmaps) para representar la densidad delictiva en Lima Metropolitana basándose en los reportes ciudadanos. Se utiliza un frontend móvil desarrollado en Kotlin para Android y Swift para iOS, integrado con un backend Spring Boot 3.5.5. El equipo necesita evaluar la viabilidad técnica de Google Maps SDK para manejar grandes volúmenes de coordenadas GPS en tiempo real sin degradar el rendimiento de la aplicación móvil y determinar las cuotas de consumo de la API de Maps y Geolocation.

**Spike Story**
Como equipo de desarrollo (móvil y backend),
quiero investigar y prototipar la integración del SDK de Google Maps en nuestros componentes móviles y servicios de geolocalización,
para que podamos entender las implicaciones técnicas, el impacto en el rendimiento de renderizado y el esfuerzo requerido para la implementación de los mapas de riesgo dinámicos.

**Criterios de Aceptación (en formato Given-When-Then)**

1. **Revisa la Documentación de la API de Google Maps**
   - Dado que el equipo necesita entender las capacidades de la biblioteca de utilidades para mapas,
   - Cuando el desarrollador revisa la documentación técnica de Google (e.g., Maps SDK for Android/iOS, Maps Utils Heatmap Layer),
   - Entonces el desarrollador identifica y documenta el flujo de integración más eficiente para procesar puntos de calor en un informe técnico compartido.

2. **Evaluación de Precisión de Geolocalización**
   - Dado la necesidad de obtener la ubicación exacta del ciudadano para el reporte de incidentes,
   - Cuando el desarrollador evalúa el impacto del uso de Fused Location Provider vs GPS nativo en el consumo de batería y precisión,
   - Entonces el desarrollador documenta los hallazgos y la configuración recomendada en el informe.

3. **Prototipa la Integración de Mapas y Marcadores**
   - Dado la necesidad de validar la carga de incidentes sobre el mapa,
   - Cuando el desarrollador construye un PoC (Proof of Concept) funcional que consume un endpoint JSON de prueba y renderiza marcadores agrupados y capas de calor,
   - Entonces el PoC es funcional, se registra en una rama del repositorio y se referencia en el informe.

**Definition of Done (DoD)**
- El código del PoC de mapas está registrado en una rama del repositorio.
- El informe técnico incluye una estimación de costos basada en la cuota de la consola de Google Cloud.
- El Spike se completa dentro del límite de 16 horas establecido para el sprint.

---

#### **Spike 2: Validación para Alertas Geolocalizadas y Notificaciones**

**Contexto**
Una de las funcionalidades críticas de UrbanVoice es la prevención activa mediante alertas de proximidad (US05). El sistema debe notificar al usuario cuando se encuentre cerca de una zona de riesgo reportada recientemente. El equipo necesita investigar el uso de servicios de fondo (Background Services) y Geofencing para determinar la viabilidad de emitir alertas sin que la aplicación esté necesariamente en primer plano, utilizando Firebase Cloud Messaging (FCM).

**Spike Story**
Como equipo de desarrollo,
quiero investigar la implementación de notificaciones push geolocalizadas y la gestión de procesos en segundo plano,
para que podamos asegurar que los ciudadanos reciban advertencias de peligro oportunas y minimizar los riesgos de latencia en la entrega de alertas críticas.

**Criterios de Aceptación (en formato Given-When-Then)**

1. **Evaluación de Capacidades de Geofencing**
   - Dado el backend Spring Boot 3.5.5 y el cliente móvil,
   - Cuando el desarrollador investiga las APIs de Geofencing nativas de Android e iOS para detectar la entrada a perímetros de riesgo,
   - Entonces el desarrollador documenta los límites de regiones activas por dispositivo y los requisitos de permisos del sistema operativo.

2. **Validación de Notificaciones Push con FCM**
   - Dado la necesidad de enviar alertas desde el servidor hacia los dispositivos cercanos,
   - Cuando el desarrollador configura Firebase Cloud Messaging y realiza una prueba de envío de una notificación simulada de "Incidente Cercano",
   - Entonces el dispositivo móvil recibe la alerta con el contenido correcto y la muestra en la barra de notificaciones del sistema.

3. **Prototipa el Flujo de Alerta por Proximidad**
   - Dado un escenario donde el usuario se desplaza virtualmente hacia una coordenada de riesgo,
   - Cuando el sistema detecta la coincidencia de ubicación y dispara la notificación simulada,
   - Entonces el flujo es verificado exitosamente y se documenta el tiempo de respuesta entre la detección y la visualización de la alerta.

**Definition of Done (DoD)**
- El informe técnico incluye la recomendación sobre la frecuencia de actualización de ubicación para no agotar la batería.
- Los hallazgos se utilizan para refinar la User Story US05 en el Product Backlog.
- El informe se comparte y revisa en la sesión de equipo.

### 2.4.2. Impact Mapping
<td><img src="assets/impact-mapping.png"/></td>

### 2.4.3. Product Backlog

<table>
  <tr>
    <th style="text-align:center;">Sprint</th>
    <th style="text-align:center;">User Story ID</th>
    <th style="text-align:center;">Título</th>
    <th style="text-align:center;">Story Points</th>
    <th style="text-align:center;">Prioridad</th>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US01</td>
    <td>Registrarse en la plataforma</td>
    <td align="center">3</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US02</td>
    <td>Iniciar sesión en la plataforma</td>
    <td align="center">3</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US04</td>
    <td>Visualizar mapa de incidentes</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US05</td>
    <td>Registrar incidente en el mapa</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US06</td>
    <td>Adjuntar evidencia multimedia al reporte</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US08</td>
    <td>Explorar landing page informativa</td>
    <td align="center">1</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US09</td>
    <td>Registrar solicitud de alianza institucional</td>
    <td align="center">3</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">US10</td>
    <td>Consultar información de contacto y redes sociales</td>
    <td align="center">1</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">TS01</td>
    <td>Configurar infraestructura cloud y pipeline CI/CD</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">TS02</td>
    <td>Implementar autenticación JWT en el backend</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">1</td>
    <td align="center">TS03</td>
    <td>Implementar API REST de incidentes</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center" style="background-color: #e8f5e9;">1</td>
    <td align="center" style="background-color: #e8f5e9;" colspan="4"><b>Total Sprint 1: 44 SP</b></td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US03</td>
    <td>Recuperar contraseña olvidada</td>
    <td align="center">2</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US07</td>
    <td>Visualizar detalle de un incidente</td>
    <td align="center">2</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US11</td>
    <td>Realizar reporte anónimo</td>
    <td align="center">3</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US12</td>
    <td>Filtrar incidentes por tipo y fecha</td>
    <td align="center">3</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US13</td>
    <td>Moderar reportes ciudadanos</td>
    <td align="center">5</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US14</td>
    <td>Gestionar categorías de incidentes</td>
    <td align="center">3</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US15</td>
    <td>Recibir notificaciones de incidentes cercanos</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US16</td>
    <td>Compartir ubicación en tiempo real</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US17</td>
    <td>Monitorear ubicación de un contacto</td>
    <td align="center">5</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US19</td>
    <td>Editar perfil de usuario</td>
    <td align="center">2</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US20</td>
    <td>Cerrar sesión</td>
    <td align="center">1</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">US22</td>
    <td>Visualizar heatmap de zonas de riesgo</td>
    <td align="center">5</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">TS04</td>
    <td>Implementar API REST de alertas y geolocalización</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">TS05</td>
    <td>Integrar Google Maps SDK en aplicaciones móviles</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center" style="background-color: #e3f2fd;">2</td>
    <td align="center" style="background-color: #e3f2fd;" colspan="4"><b>Total Sprint 2: 63 SP</b></td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US18</td>
    <td>Activar o desactivar alertas por zona geográfica</td>
    <td align="center">3</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US21</td>
    <td>Gestionar contactos de confianza</td>
    <td align="center">3</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US23</td>
    <td>Generar reporte estadístico de incidentes</td>
    <td align="center">5</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US24</td>
    <td>Enviar notificaciones masivas desde administración</td>
    <td align="center">3</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US25</td>
    <td>Visualizar historial de incidentes reportados</td>
    <td align="center">3</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US26</td>
    <td>Recibir confirmación de reporte procesado</td>
    <td align="center">2</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">US27</td>
    <td>Valorar utilidad de reportes de otros usuarios</td>
    <td align="center">2</td>
    <td align="center">Baja</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">TS06</td>
    <td>Implementar pruebas unitarias y de integración</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">TS07</td>
    <td>Implementar WebSockets para actualizaciones en tiempo real</td>
    <td align="center">5</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">TS08</td>
    <td>Implementar sistema de caché y optimización de consultas</td>
    <td align="center">5</td>
    <td align="center">Media</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">TS09</td>
    <td>Realizar pruebas de seguridad y penetración</td>
    <td align="center">8</td>
    <td align="center">Alta</td>
  </tr>
  <tr>
    <td align="center" style="background-color: #fff3e0;">3</td>
    <td align="center" style="background-color: #fff3e0;" colspan="4"><b>Total Sprint 3: 47 SP</b></td>
  </tr>
  <tr>
    <td align="center" style="background-color: #f5f5f5;" colspan="2"><b>Total general</b></td>
    <td align="center" style="background-color: #f5f5f5;" colspan="3"><b>154 SP</b></td>
  </tr>
</table>

## 2.5. Strategic-Level Domain-Driven Design

Esta sección detalla la descomposición del sistema UrbanVoice en subdominios lógicos, permitiendo una arquitectura modular que responda a la complejidad de la seguridad urbana . Se emplean técnicas de diseño estratégico para asegurar que cada módulo tenga una responsabilidad clara y aislada.

### 2.5.1 EventStorming

El equipo realizó una sesión colaborativa para modelar los procesos de negocio de UrbanVoice, identificando eventos de dominio, comandos y reglas .

#### Paso 1: Collect Domain Events

En este primer paso, se identificaron todos los eventos relevantes para el dominio de nuestro sistema. Estos eventos representan hechos importantes que suceden en el proceso de negocio, como la creación de una cuenta, la publicación de un local o la confirmación de un pago, y los recopilamos utilizando post-its de color naranja.

<td><img src="assets/Step 1.jpg"/></td>


#### Paso 2: Timeline

En este paso organizamos los eventos identificados en una línea temporal, colocándolos en orden cronológico para visualizar mejor el flujo del proceso (por ejemplo, desde que el Propietario publica un local hasta que el Freelancer lo reserva y lo paga) y entender la secuencia natural de acciones en el sistema.

<td><img src="assets/Step 2.jpg"/></td>

#### Paso 3: Pain and Pivotal Points

En este paso se identificaron los pain points y los pivotal points del proceso. Esto significa que se encontraron las partes que necesitan mayor atención o que son cruciales para que el sistema funcione correctamente.

<td><img src="assets/Step 3.jpg"/></td>

#### Paso 4: Commands

En este paso se agregaron comandos (los post-its azules) para representar las acciones de los usuarios o sistemas que inician un cambio en el sistema.

<td><img src="assets/Step 4.jpg"/></td>

#### Paso 5: Policies

En este paso se definieron reglas de negocio (los post-its lila/morados) que responden a ciertos eventos y generan nuevos comandos o eventos. Básicamente, estas reglas automatizan decisiones basadas en lo que sucedió antes.

<td><img src="assets/Step 5.jpg"/></td>

#### Paso 6: Read Models

En este paso se identificaron las vistas o modelos de lectura que los usuarios necesitan (post-its verdes). Esto se refiere a la información específica que debe estar accesible en ciertos momentos.

<td><img src="assets/Step 6.jpg"/></td>

#### Paso 7: External System

En este paso se identificaron los sistemas externos (post-its rosados) que se conectan con nuestra solución. Estos son elementos que no controlamos directamente, pero que influyen en el proceso.

<td><img src="assets/Step 7.jpg"/></td>

#### Paso 8: Aggregates

En este paso se organizaron los comandos y eventos relacionados en grupos lógicos llamados agregados (los post-its amarillos claros). Cada grupo reúne un conjunto de funciones y entidades que trabajan juntas de manera coherente.

<td><img src="assets/Step 8.jpg"/></td>

#### Paso 9: Bounded Context

Al final, definimos las áreas de responsabilidad del sistema, agrupando los agregados y procesos afines, también conocidas como bounded contexts.

Bounded context: Identity and Access Management
<td><img src="assets/Identity and Access Managment.jpg"/></td>

Bounded context: Profile and Preferences Management
<td><img src="assets/Profile and Preferences Managment.jpg"/></td>

Bounded context: Location Managment
<td><img src="assets/Location Managment.jpg"/></td>

Bounded context: Report Managment
<td><img src="assets/Report Managment.jpg"/></td>

Bounded context: Notification Managment
<td><img src="assets/Notification Managment.jpg"/></td>


### 2.5.1.1 Candidate Context Discovery

Tras analizar los eventos clave y los límites naturales del lenguaje, se identificaron los siguientes Bounded Contexts candidatos para UrbanVoice :

- **Identity and Access Management**: Encargado de la seguridad, roles de usuario y sesiones.
- **Profile Management**: Provee la funcionalidad de perfiles personales y preferencias.
- **Report Management**: Maneja el ciclo de vida de los incidentes y la evidencia multimedia (Core Domain) .
- **Location & Geospatial Intelligence**: Provee la lógica de mapas de calor, coordenadas y cálculo de rutas seguras.
- **Notification Management:** Coordina el envío de alertas críticas y mensajes a contactos.

<td><img src="assets/Step 8.jpg"/></td>

### 2.5.1.2 Domain Message Flows Modeling

Se modelaron los flujos de comunicación entre contextos para los escenarios críticos de la aplicación .

**Escenario 1: Reporte de Incidente Ciudadano**

El Ciudadano registra un incidente mediante la app móvil. El contexto de Report almacena la data, el contexto de Location valida el punto crítico y el contexto de Notification dispara una alerta a los vecinos cercanos.

<td><img src="assets/Scenario 3 Process Payment.jpg"/></td>

**Escenario 2: Compartir Ubicación en Tiempo Real**

El Ciudadano inicia un trayecto. El contexto de Profile identifica a los contactos de confianza y el contexto de Location emite las coordenadas constantes al contexto de Notification para que los contactos reciban el seguimiento.


<td><img src="assets/Scenario 3 Process Payment.jpg"/></td>

### 2.5.1.3. Bounded Context Canvases

En esta sección, el equipo diseña sus candidate bounded contexts detallando los criterios de diseño estratégicos y tácticos. Para cada Bounded Context, se ha elaborado un Bounded Context Canvas utilizando la plantilla estándar, siguiendo un proceso iterativo que incluye la definición del propósito, la destilación del Lenguaje Ubicuo, las reglas de negocio, los mensajes consumidos/producidos y el análisis de dependencias.

1. Bounded Context Canvas: Identity and Access Management (IAM)
<td><img src="assets/IAM-canvas.jpg"/></td>

2. Bounded Context Canvas: Profile and Preferences Management
<td><img src="assets/Profile and Preferences Managemen-canvas.jpg"/></td>

3. Bounded Context Canvas: Location Managment
<td><img src="assets/Location-Managment.jpg"/></td>

4. Bounded Context Canvas: Report Managment
<td><img src="assets/Report-managment.png"/></td>

5. Bounded Context Canvas: Notification Managment
<td><img src="assets/Notification-Managment.jpg"/></td>

### 2.5.2. Context Mapping
Este diagrama define las relaciones y fronteras entre los diferentes dominios (Agregados) identificados en el Event Storming. Establece cómo interactúan los contextos de Access, User, Incident, Spacial y Alert, detallando la naturaleza de sus integraciones y el flujo de información entre ellos para garantizar la integridad del sistema.
<td><img src="assets//Mapping.jpeg"/></td>

### 2.5.3. Software Architecture
En esta sección se describe la estructura técnica de la solución. Se detalla la organización de los componentes, sus responsabilidades y cómo se articulan para satisfacer los requerimientos funcionales de participación ciudadana y seguridad urbana de UrbanVoice.

### 2.5.3.1. Software Architecture Context Level Diagrams
<td><img src="assets/structurizr-97259-SystemContext.png"/></td>


### 2.5.3.2. Software Architecture Container Level Diagrams
<td><img src="assets/structurizr-97259-Containers.png"/></td>


### 2.5.3.3. Software Architecture Deployment Diagrams
<td><img src="assets/structurizr-97259-ProductionDeployment.png"/></td>

## 2.6 Tactical-Level Domain-Driven Design

### 2.6.1 Bounded Context:Identity and Access Managment

El Bounded Context Identity and Access Management (IAM) es el pilar de seguridad de UrbanVoice. Su responsabilidad principal es gestionar el ciclo de vida de las identidades digitales, garantizando que solo los usuarios legítimos (ciudadanos y administradores) accedan a los recursos de la plataforma. Este contexto implementa la lógica de autenticación, autorización basada en roles (RBAC) y la gestión de sesiones mediante tokens de seguridad.

#### 2.6.1.1. Domain Layer

La Domain Layer concentra el modelo del dominio del contexto IAM. Aquí se ubican las clases que representan los conceptos del negocio, sus reglas y sus invariantes, sin dependencia alguna hacia frameworks, bases de datos ni servicios externos.

**Aggregate Root: `UserAccount`**

La entidad `UserAccount` es el aggregate root del contexto IAM. Esta entidad es la unidad de consistencia transaccional y concentra toda la lógica relacionada con el estado de un usuario registrado en el sistema: cuando un propietario o freelancer crea su cuenta, cuando se valida que su correo electrónico es único o cuando se restablece su contraseña, todas esas operaciones pasan necesariamente por este aggregate root.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `AccountId` (VO) | Identificador único de la cuenta de usuario |
| `name` | `UserProfileInfo` (VO) | Información del perfil del usuario (nombre y edad) |
| `credentials` | `AccountCredentials` (VO) | Credenciales de acceso (correo electrónico y hash de contraseña) |
| `status` | `AccountStatus` (Enum) | Estado actual de la cuenta (e.g., CREATED, VERIFIED, LOCKED) |
| `session` | `Session` (Entity) | Entidad interna que representa la sesión activa (opcional) |
| `createdAt` | `DateTime` | Fecha y hora de creación de la cuenta |
| `updatedAt` | `DateTime` | Fecha y hora de la última actualización |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `changeCredentials(credentials: AccountCredentials)` | public | Cambia las credenciales de acceso. Emite `PasswordChanged` |
| `isLoginAllowed()` | public | Invariante: Retorna `true` si el estado de la cuenta y los intentos fallidos permiten el inicio de sesión |
| `lock()` | public | Bloquea la cuenta por seguridad (e.g., tras múltiples fallos de login) |
| `validateProfileInfo()` | public | Valida que la información de nombre y edad cumpla con las reglas de negocio |
| `validatePasswordResetPolicy(policy: PasswordResetPolicy)` | public | Valida que un nuevo password cumpla con la política de seguridad |
| `updateProfileInfo(profileInfo: UserProfileInfo)` | public | Actualiza el nombre y la edad del usuario |

**Entidad interna: `Session`**

`Session` es una entidad interna del aggregate root `UserAccount`. Su ciclo de vida está ligado a la cuenta; representa una instancia de autenticación exitosa.

| Atributo | Tipo | Descripción |
|---|---|---|
| `token` | `SessionToken` (VO) | Token criptográfico que identifica la sesión |
| `startedAt` | `DateTime` | Fecha y hora de inicio de la sesión |
| `expiresAt` | `DateTime` | Fecha y hora de expiración del token |

**Value Objects**

| Value Object | Propósito |
|---|---|
| `AccountId` | Identificador único de la cuenta de usuario (e.g., UUID) |
| `Name` | Encapsula el nombre del usuario (e.g., longitud mínima 2) |
| `Age` | Encapsula la edad validada |
| `EmailAddress` | Encapsula el correo electrónico del usuario, validando su formato y asegurando que sea único en el sistema |
| `Password` | Encapsula la contraseña compleja, pero solo como una abstracción antes de ser hasheada |
| `AccountCredentials` | Encapsula el correo electrónico y el hash de la contraseña. Es inmutable y se modela por valor |
| `SessionToken` | Token único y seguro de sesión |

**Enumerations**

| Enum | Valores | Propósito |
|---|---|---|
| `AccountStatus` | CREATED, VERIFIED, LOCKED, DELETED | Representa el estado actual de la cuenta de usuario |

**Domain Services**

| Domain Service | Responsabilidad |
|---|---|
| `PasswordHashingService` | Provee una abstracción para el hasheo seguro de contraseñas. Su implementación vive en infraestructura |
| `PasswordResetService` | Coordina el proceso de validación y generación de tokens para la recuperación de contraseña |
| `EmailUniquenessChecker` | Servicio para verificar que un correo electrónico no esté ya registrado en el sistema |

**Repository Interfaces (abstracciones)**

| Interface | Operaciones principales |
|---|---|
| `UserAccountRepository` | `save(account: UserAccount)`, `findById(id: AccountId)`, `findByEmail(email: EmailAddress)` |

**Domain Events**

| Domain Event | Cuándo se emite | Consumidores |
|---|---|---|
| `UserAccountCreated` | Cuando se crea exitosamente un nuevo `UserAccount` | Interno y externo |
| `LoginSuccessful` | Cuando un usuario inicia sesión con credenciales válidas | Interno y externo |
| `LoginFailed` | Cuando un intento de inicio de sesión falla | Interno (e.g., para audit-log y bloqueo) |
| `PasswordResetInitiated` | Cuando se solicita un cambio de contraseña | Interno y externo |
| `PasswordChanged` | Cuando se completa exitosamente el cambio de contraseña | Interno y externo |
| `SessionEnded` | Cuando un usuario cierra sesión explícitamente | Interno y externo |

**Factories**

| Factory | Propósito |
|---|---|
| `UserAccountFactory` | Centraliza la creación de nuevos `UserAccount` válidos a partir de un command, asegurando que se cumplan todas las precondiciones |

#### 2.6.1.2. Interface Layer

La Interface Layer es la capa más externa del Bounded Context del lado entrante. Su responsabilidad es exponer las capabilities del contexto y traducir los requests entrantes al modelo de la Application Layer.

**Controllers REST**

| Controller | Endpoints | Capabilities soportadas |
|---|---|---|
| `AccountRegistrationController` | `POST /api/v1/accounts` | Creación de cuenta y completado de registro |
| `AccountLoginController` | `POST /api/v1/login`, `POST /api/v1/logout` | Inicio y cierre de sesión |
| `PasswordResetController` | `POST /api/v1/password-reset/initiate`, `POST /api/v1/password-reset/complete` | Solicitud y cambio de contraseña |

**Resources / DTOs**

| DTO | Tipo | Uso |
|---|---|---|
| `RegisterAccountRequest` | Input | Payload del request `POST` para crear una cuenta |
| `LoginRequest` | Input | Payload del request `POST` para iniciar sesión |
| `InitiatePasswordResetRequest` | Input | Payload para solicitar la recuperación de contraseña |
| `CompletePasswordResetRequest` | Input | Payload para establecer la nueva contraseña |
| `AccountSummaryResponse` | Output | Versión reducida de la cuenta para listados rápidos |
| `LoginResponse` | Output | Respuesta exitosa del login (e.g., con token de sesión) |
| `AccountStatusResponse` | Output | Respuesta detallada del estado de la cuenta |

**Assemblers**

| Assembler | Transformación |
|---|---|
| `FromRegisterAccountRequestAssembler` | `RegisterAccountRequest` a `RegisterAccountCommand` |
| `FromLoginRequestAssembler` | `LoginRequest` a `LoginUserCommand` |

#### 2.6.1.3. Application Layer

La Application Layer orquesta los flujos de proceso del negocio que involucran al Bounded Context. Aquí viven las clases responsables de recibir commands y queries, coordinar con el Domain Layer, gestionar la transaccionalidad y publicar los domain events. Se adopta el patrón CQRS ligero.

**Command Handlers**

| Command Handler | Command procesado | Flujo |
|---|---|---|
| `RegisterAccountCommandHandler` | `RegisterAccountCommand` | Valida el command, invoca al `UserAccountFactory` para crear el aggregate, persiste vía `UserAccountRepository` y publica `UserAccountCreated` |
| `LoginUserCommandHandler` | `LoginUserCommand` | Recupera el aggregate por correo, valida credenciales, invoca `account.startSession()`, persiste y publica `LoginSuccessful` |
| `InitiatePasswordResetCommandHandler` | `InitiatePasswordResetCommand` | Recupera el aggregate, invoca el `PasswordResetService` para generar token, persiste y publica `PasswordResetInitiated` |
| `CompletePasswordResetCommandHandler` | `CompletePasswordResetCommand` | Valida el token, recupera el aggregate, invoca `account.changeCredentials()`, persiste y publica `PasswordChanged` |
| `LogoutUserCommandHandler` | `LogoutUserCommand` | Recupera el aggregate, invoca `account.endSession()`, persiste y publica `SessionEnded` |

**Query Services**

| Query Service | Query soportada | Retorno |
|---|---|---|
| `GetRegistrationFormQueryService` | `GetRegistrationFormQuery` | `RegisterAccountRequest` (vacío) |
| `GetLoginFormQueryService` | `GetLoginFormQuery` | `LoginRequest` (vacío) |
| `GetAccountStatusQueryService` | `GetAccountStatusQuery(accountId)` | `AccountStatusResponse` |
| `GetAccountSummaryQueryService` | `GetAccountSummaryQuery(accountId)` | `AccountSummaryResponse` |

**Event Handlers**

| Event Handler | Evento | Acción |
|---|---|---|
| `UserAccountCreatedEventHandler` | `UserAccountCreated` | Publica el evento en el message broker para que otros contexts reaccionen |
| `LoginFailedEventHandler` | `LoginFailed` | Actualiza un read-model específico o genera una entrada de audit-log |

**Application Services**

| Application Service | Responsabilidad |
|---|---|
| `AccountApplicationService` | Fachada del contexto que coordina Command Handlers y Query Services |

#### 2.6.1.4 Infrastructure Layer

La Infrastructure Layer provee implementaciones concretas de las abstracciones definidas en el Domain Layer y gestiona la integración con tecnologías externas.

**Repository Implementations**

| Implementación | Interface que implementa | Tecnología |
|---|---|---|
| `JpaUserAccountRepository` | `UserAccountRepository` | Spring Data JPA sobre PostgreSQL |

**JPA Entities**

| JPA Entity | Mapeo |
|---|---|
| `UserAccountJpaEntity` | Tabla `accounts` |
| `UserProfileInfoJpaEntity` | Tabla `user_profiles` o descomposición en la tabla `accounts` |
| `SessionJpaEntity` | Tabla `sessions` |

**Mappers Domain a JPA**

| Mapper | Transformación |
|---|---|
| `UserAccountJpaMapper` | `UserAccount` a `UserAccountJpaEntity` y viceversa |
| `SessionJpaMapper` | `Session` a `SessionJpaEntity` y viceversa |

**External Service Adapters**

| Adapter | Servicio externo | Responsabilidad |
|---|---|---|
| `BCryptPasswordAdapter` | `PasswordHashingService` | Provee la implementación de hasheo seguro utilizando BCrypt |
| `JwtSessionServiceAdapter` | `SessionTokenGenerator` | Genera y valida tokens de sesión seguros utilizando JSON Web Tokens (JWT) |
| `MailgunServiceAdapter` | `EmailService` | Implementación externa para enviar correos electrónicos para la recuperación de contraseña |
| `EventPublisherAdapter` | RabbitMQ (vía Spring AMQP) | Publica los domain events en el exchange correspondiente |

**Configuration**

| Clase de configuración | Propósito |
|---|---|
| `IamContextConfig` | Registra los beans de Spring del contexto, configura transacciones y wiring de handlers |
| `SpringSecurityConfig` | Configura el framework de seguridad (e.g., filtros JWT, autenticación de endpoints) |
| `RabbitMqConfig` | Declara exchanges, queues y bindings del contexto |
| `DatabaseConfig` | Configura la conexión a la base de datos PostgreSQL específica para este contexto |

#### 2.6.1.5 Bounded Context Software Architecture Component Level Diagrams

En esta subsección se documenta de forma textual y visual la arquitectura a nivel de componentes del Bounded Context Identity and Access Management (IAM). La descomposición parte del contenedor `Identity Service`, que implementa este contexto, y lo organiza en componentes principales agrupados por capas. Cada componente representa una agrupación coherente de clases que colaboran para proveer el ciclo de vida de la cuenta de usuario.

La arquitectura evidencia una separación estricta entre las cuatro capas. La Interface Layer, compuesta por `AccountRegistrationController`, `AccountLoginController` y `PasswordResetController`, recibe las peticiones HTTP y delega en la Application Layer. Esta capa coordina el flujo mediante `AccountApplicationService`, Command Handlers específicos (como `RegisterAccountCommandHandler` y `LoginUserCommandHandler`) y Query Services.

Estos componentes interactúan con el Domain Layer, el núcleo del contexto, donde residen el aggregate root `UserAccount`, la factory `UserAccountFactory` y servicios de dominio puros como `PasswordResetService`. Siguiendo el Dependency Inversion Principle, la Infrastructure Layer provee las implementaciones técnicas a través de `JpaUserAccountRepository`, y delega la complejidad técnica externa a adapters como `JwtSessionServiceAdapter` (para tokens) y `BCryptPasswordAdapter` (para encriptación).

<td><img src="assets/IAMComponents.png"/></td>

#### 2.6.1.6 Bounded Context Software Architecture Code Level Diagrams

En esta subsección se describe la arquitectura a nivel de código del Bounded Context Identity and Access Management (IAM). Se documentan los dos artefactos principales del diseño detallado: el modelo de clases del Domain Layer, garantizando las reglas de negocio de autenticación y registro, y el diseño de persistencia relacional que soporta al contexto.

##### 2.6.1.6.1. Bounded Context Domain Layer Class Diagrams

El modelo de clases del Domain Layer gira alrededor del aggregate root UserAccount, que concentra la consistencia transaccional del contexto de identidad. Dentro de este aggregate se encuentra la entidad interna Session, cuya existencia depende de un inicio de sesión exitoso asociado a una cuenta activa.

Los value objects, como AccountId, AccountCredentials (que encapsula email y hash), UserProfileInfo y SessionToken, forman parte integral del modelo. Estos objetos inmutables refuerzan validaciones intrínsecas, por ejemplo, asegurando que un correo tenga el formato correcto antes de ser evaluado por el sistema. Las enumeraciones como AccountStatus dictan las invariantes del estado de la cuenta (CREATED, VERIFIED, LOCKED).

Sobre este núcleo actúan las interfaces abstractas UserAccountRepository y PasswordHashingService, manteniendo al dominio completamente ignorante de las librerías de persistencia o los algoritmos criptográficos específicos utilizados en producción.

<td><img src="assets/IAMDomainLayer.png"/></td>

##### 2.6.1.6.2.  Bounded Context Database Design Diagram   

El diseño de base de datos relacional que soporta el Bounded Context IAM sigue el principio de database-per-service. La tabla central es accounts, donde se materializa el aggregate root UserAccount. Esta tabla contiene los identificadores únicos, los datos del perfil del usuario (descompuestos en columnas) y las credenciales cifradas.

Para garantizar la integridad y la seguridad a nivel de base de datos, se utiliza un índice UNIQUE sobre la columna email, previniendo de forma estricta que dos usuarios se registren con el mismo correo. Asimismo, se implementan restricciones CHECK para asegurar que la columna status solo contenga valores válidos.

La tabla sessions representa la entidad interna del dominio y se relaciona con accounts mediante una foreign key. Esta tabla maneja la persistencia de los tokens de sesión activos y sus fechas de expiración, con un borrado en cascada (ON DELETE CASCADE) si la cuenta madre es eliminada. Finalmente, una columna version en la tabla accounts habilita el optimistic locking, evitando condiciones de carrera si el usuario intenta modificar su perfil desde dos dispositivos simultáneamente.

<td><img src="assets/IAMDatabase.png"/></td>

### 2.6.2 Bounded Context:Profile and Preferences Management
El Bounded Context Profile and Preferences Management es el encargado de gestionar la identidad social y la configuración de seguridad personalizada de cada ciudadano en UrbanVoice. Mientras que el contexto IAM se ocupa de la "cuenta" y el "acceso", este contexto se centra en el "sujeto": quién es el usuario, cómo desea ser notificado y, fundamentalmente, quiénes integran su red de apoyo inmediata.

Este contexto introduce el concepto crítico del Círculo de Confianza, una red de contactos que permite la reacción rápida ante situaciones de emergencia. La lógica de este contexto asegura que la información de contacto sea válida y que las preferencias de notificación respeten las invariantes de privacidad definidas por el usuario. El diseño táctico sigue los principios de segregación de responsabilidades para permitir que la gestión de perfiles escale independientemente del sistema de autenticación central.
#### 2.6.2.1. Domain Layer

La capa de dominio define la estructura y el comportamiento de la identidad del ciudadano y sus vínculos de seguridad. Es una capa pura que encapsula las reglas sobre cómo se construye una red de contactos confiable.

**Aggregate Root: `Profile`**

El aggregate root `Profile` es la entidad principal que orquesta la información del ciudadano y su círculo de confianza. Un perfil es el punto de consistencia para todas las configuraciones de seguridad personal; por ejemplo, no se puede activar una alerta de pánico si el perfil no tiene al menos un contacto de confianza validado.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `ProfileId` (VO) | Identificador único vinculado al `AccountId` del contexto IAM |
| `fullName` | `PersonName` (VO) | Nombre y apellido con validaciones de longitud y caracteres |
| `phoneNumber` | `Phone` (VO) | Número móvil validado para comunicaciones de emergencia |
| `circleOfTrust` | `List<TrustedContact>` | Colección de entidades internas (contactos de apoyo) |
| `preferences` | `UserPreferences` (VO) | Configuraciones de radio de alerta y categorías de interés |
| `avatarUrl` | `StorageUrl` (VO) | Enlace a la imagen de perfil almacenada en la nube |
| `createdAt` | `DateTime` | Fecha de creación del perfil |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `addTrustedContact(name, phone, relationship)` | public | Agrega un nuevo contacto al círculo. Invariante: Máximo 5 contactos por perfil. Emite `ContactAddedToCircle`. |
| `removeTrustedContact(contactId)` | public | Elimina un contacto de la red de apoyo. |
| `updateEmergencySettings(radius, autoAlert)` | public | Modifica los umbrales de geofencing para alertas automáticas. |
| `updateProfileInfo(name, phone)` | public | Actualiza datos básicos. Emite `ProfileUpdated`. |

**Entidad interna: `TrustedContact`**

`TrustedContact` es una entidad que solo existe dentro del ciclo de vida de un `Profile`. Representa a las personas externas (familiares, amigos) que recibirán notificaciones si el ciudadano se encuentra en peligro.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `ContactId` (VO) | Identificador único del contacto dentro del perfil |
| `name` | `string` | Nombre del contacto |
| `phoneNumber` | `Phone` (VO) | Número para recepción de SMS/Llamadas de alerta |
| `relationship` | `string` | Vínculo (Padre, Amigo, etc.) para contextualizar la alerta |

**Value Objects**

| Value Object | Propósito |
|---|---|
| `ProfileId` | UUID inmutable que actúa como llave foránea lógica hacia IAM. |
| `PersonName` | Valida que el nombre no contenga caracteres especiales y tenga una longitud mínima. |
| `Phone` | Valida el formato internacional de número telefónico (E.164). |
| `UserPreferences` | Encapsula el radio de acción (en metros) y los filtros de tipos de incidentes preferidos. |

**Domain Services**

| Domain Service | Responsabilidad |
|---|---|
| `CircleIntegrityService` | Valida que los números telefónicos en el Círculo de Confianza no estén duplicados y sean operables para servicios de SMS. |

**Domain Events**

| Domain Event | Cuándo se emite | Consumidores |
|---|---|---|
| `ProfileCreated` | Al instanciar un perfil nuevo tras el registro en IAM. | Notifications (para bienvenida). |
| `ContactAddedToCircle` | Al registrar un nuevo contacto de emergencia. | Notifications (para solicitar confirmación al contacto). |
| `EmergencyPreferencesChanged` | Al modificar radios de geofencing. | Location Management (para actualizar observadores). |

#### 2.6.2.2. Interface Layer
Expone las capacidades de gestión de identidad social y configuración a los clientes móviles y aplicaciones de administración.

**Controllers REST**

| Controller | Endpoints | Capabilities soportadas |
|---|---|---|
| `ProfileController` | `GET /api/v1/profiles/me` <br> `PATCH /api/v1/profiles/me` | Consulta y actualización del perfil del ciudadano autenticado. |
| `TrustCircleController` | `POST /api/v1/profiles/me/contacts` <br> `DELETE /api/v1/profiles/me/contacts/{id}` | Gestión dinámica del Círculo de Confianza. |

**Resources / DTOs**

| DTO | Uso |
|---|---|
| `UpdateProfileResource` | Payload para modificar datos personales y preferencias. |
| `TrustedContactResource` | Representación del contacto para ser mostrado en la App móvil. |
| `ProfileDetailResource` | Vista completa del perfil incluyendo estadísticas de reportes realizados. |

#### 2.6.2.3. Application Layer

Gestiona los flujos de orquestación, asegurando que las acciones del usuario se traduzcan en cambios válidos en el dominio y se notifiquen a otros contextos.

**Command Handlers**

| Command Handler | Flujo |
|---|---|
| `CreateProfileCommandHandler` | Reacciona al evento `UserRegistered` de IAM para inicializar un perfil vacío con valores por defecto. |
| `AddTrustedContactCommandHandler` | Recupera el perfil, invoca la lógica de negocio de `addTrustedContact` y persiste los cambios. |
| `UpdatePreferencesCommandHandler` | Traduce los nuevos parámetros de alerta y los aplica al aggregate root. |

**Query Services**

| Query Service | Responsabilidad |
|---|---|
| `GetProfileDetailsQueryService` | Retorna la información extendida del ciudadano, integrando datos del modelo de lectura optimizado. |

#### 2.6.2.4 Infrastructure Layer

Provee la persistencia y la integración con servicios multimedia externos.

**Persistence**

| Componente | Tecnología | Mapeo |
|---|---|---|
| `JpaProfileRepository` | Spring Data JPA | Tabla `profiles` y `trusted_contacts` (relación One-to-Many). |

**Adapters**

| Adapter | Servicio Externo | Responsabilidad |
|---|---|---|
| `CloudinaryImageAdapter` | Cloudinary API | Gestiona el upload de fotos de perfil y retorna las URLs optimizadas con transformación de tamaño. |
| `IamServiceClientAdapter` | IAM Context (REST/Internal) | Verifica la existencia de la cuenta antes de operaciones críticas de perfil. |

**Mappers**

| Mapper | Transformación |
|---|---|
| `ProfileMapper` | Convierte la entidad de persistencia `ProfileJpaEntity` al objeto de dominio `Profile` manteniendo la inmutabilidad de los Value Objects. |

#### 2.6.2.5 Bounded Context Software Architecture Component Level Diagrams

En esta subsección se documenta la arquitectura a nivel de componentes del Bounded Context **Profile and Preferences Management**. La descomposición parte del contenedor **Profile Service**, el cual implementa este contexto y se organiza en componentes agrupados por capas. Cada componente representa una agrupación coherente de clases que colaboran para gestionar la información personal del ciudadano, sus preferencias de seguridad y su círculo de confianza.

La **Interface Layer** expone las capacidades del contexto a través de `ProfileController` y `TrustCircleController`, los cuales reciben las solicitudes HTTP provenientes de la aplicación móvil y delegan su procesamiento a la **Application Layer**. Estos componentes permiten consultar y actualizar el perfil del usuario autenticado, así como registrar y eliminar contactos del círculo de confianza.

La **Application Layer** coordina los casos de uso mediante `ProfileApplicationService`, los command handlers `CreateProfileCommandHandler`, `UpdateProfileCommandHandler`, `AddTrustedContactCommandHandler`, `RemoveTrustedContactCommandHandler` y `UpdatePreferencesCommandHandler`, además del `GetProfileDetailsQueryService` para las operaciones de consulta. Esta capa se encarga de orquestar el flujo entre la capa de entrada y el modelo de dominio, manteniendo separada la lógica de negocio de los detalles de transporte y persistencia.

La **Domain Layer** concentra el núcleo del contexto. En ella residen el aggregate root `Profile`, la entidad interna `TrustedContact`, el value object `UserPreferences`, el servicio de dominio `CircleIntegrityService` y la abstracción `ProfileRepository`. Estas piezas encapsulan las reglas de negocio relacionadas con la actualización del perfil, la validación de contactos de confianza y la configuración de preferencias de seguridad. De esta manera, el dominio permanece independiente de frameworks y tecnologías externas.

Siguiendo el principio de inversión de dependencias, la **Infrastructure Layer** provee las implementaciones técnicas necesarias para ejecutar el contexto en producción. En esta capa se ubican `JpaProfileRepository`, encargado de la persistencia relacional; `ProfileMapper`, responsable de transformar entidades de persistencia en objetos de dominio y viceversa; `CloudinaryImageAdapter`, para la gestión de imágenes de perfil; e `IamServiceClientAdapter`, que permite validar la existencia de la cuenta del usuario en el contexto IAM cuando sea necesario. Opcionalmente, el contexto también puede incorporar un `EventPublisherAdapter` para publicar eventos de dominio hacia otros bounded contexts.

Esta organización por componentes evidencia una separación clara de responsabilidades, mejora la mantenibilidad del contexto y permite que la lógica del perfil evolucione de manera desacoplada de la infraestructura y del sistema de autenticación.

<td><img src="assets/Component Level Diagram — Profile and Preferences Management.png"/></td>

#### 2.6.2.6 Bounded Context Software Architecture Code Level Diagrams

En esta subsección se describe la arquitectura a nivel de código del Bounded Context **Profile and Preferences Management**. Se documentan los dos artefactos principales del diseño detallado del contexto: el modelo de clases del **Domain Layer**, que concentra las reglas de negocio del perfil del ciudadano y su círculo de confianza, y el diseño de persistencia relacional que soporta dichas capacidades.

El objetivo de esta vista es mostrar cómo los conceptos del dominio previamente identificados se traducen en estructuras de código concretas, preservando la separación entre la lógica de negocio, la persistencia y la integración con servicios externos. Para ello, se presenta primero el diagrama de clases del dominio y, posteriormente, el diagrama de diseño de base de datos asociado al contexto.


##### 2.6.2.6.1. Bounded Context Domain Layer Class Diagrams

El modelo de clases del **Domain Layer** gira alrededor del aggregate root `Profile`, que concentra la consistencia transaccional del contexto. Este aggregate representa la identidad funcional del ciudadano dentro de UrbanVoice y centraliza la gestión de su información personal, sus preferencias de seguridad y su círculo de confianza.

Dentro de este aggregate se encuentra la entidad interna `TrustedContact`, cuya existencia depende completamente del perfil al que pertenece. La relación entre ambas clases es de composición, ya que un contacto de confianza no tiene sentido fuera del ciclo de vida de un `Profile`. A través de esta estructura se modela la red de apoyo inmediata del ciudadano para escenarios de emergencia.

El aggregate utiliza distintos **Value Objects** para encapsular validaciones y reforzar la semántica del dominio. Entre ellos destacan `ProfileId`, `ContactId`, `PersonName`, `Phone`, `UserPreferences` y `StorageUrl`. Estos objetos son inmutables y contienen reglas intrínsecas, como el formato válido del número telefónico, la estructura correcta del nombre y las configuraciones permitidas de seguridad personalizada.

Sobre este núcleo actúa el servicio de dominio `CircleIntegrityService`, responsable de validar reglas que no pertenecen naturalmente a una sola entidad, como evitar la duplicidad de contactos dentro del círculo de confianza y verificar que los números registrados puedan ser utilizados para comunicaciones de emergencia. Asimismo, la abstracción `ProfileRepository` representa el puerto de persistencia del aggregate root, permitiendo almacenar y recuperar perfiles sin acoplar el dominio a una tecnología específica de base de datos.

Este diseño mantiene al dominio limpio y cohesionado, reforzando las invariantes del contexto y preservando su independencia respecto de la infraestructura.

<td><img src="assets/Domain Layer Class Diagram.png"/></td>

##### 2.6.2.6.2. Bounded Context Database Design Diagram

El diseño de base de datos relacional que soporta el Bounded Context **Profile and Preferences Management** sigue el principio de **database-per-service**, de modo que este contexto administra de forma independiente la persistencia de los perfiles y sus contactos de confianza.

La tabla central es `profiles`, donde se materializa el aggregate root `Profile`. En esta tabla se almacenan los atributos principales del perfil del ciudadano, tales como el identificador del perfil, la referencia lógica hacia la cuenta del contexto IAM (`account_id`), el nombre completo, el número telefónico, la URL del avatar y las preferencias de seguridad configuradas por el usuario, como el radio de alerta, la activación de alertas automáticas y las categorías preferidas de incidentes.

Para garantizar integridad a nivel de base de datos, la tabla `profiles` incorpora una restricción `UNIQUE` sobre `account_id`, evitando que una misma cuenta tenga más de un perfil asociado. Asimismo, la columna `version` permite implementar **optimistic locking**, previniendo conflictos cuando múltiples operaciones intentan modificar el mismo perfil de forma concurrente.

La tabla `trusted_contacts` representa la entidad interna `TrustedContact` y mantiene una relación de uno a muchos con `profiles`, ya que un perfil puede contener varios contactos de confianza. En esta tabla se almacenan el identificador del contacto, el identificador del perfil al que pertenece, el nombre del contacto, su número telefónico, el tipo de relación que mantiene con el usuario y la fecha de registro.

La relación entre `profiles` y `trusted_contacts` se implementa mediante una **foreign key** sobre `profile_id`, acompañada de borrado en cascada (`ON DELETE CASCADE`), ya que un contacto de confianza no debe existir sin el perfil al que pertenece. Adicionalmente, se recomienda definir índices sobre `account_id` y `profile_id` para optimizar las consultas más frecuentes del contexto.

Este diseño relacional permite representar adecuadamente las necesidades funcionales del bounded context y mantiene consistencia entre el modelo del dominio y la estructura de persistencia.

<td><img src="assets/Database Design Diagram.png"/></td>

### 2.6.3 Bounded Context:Location Managment

El Bounded Context Location Management representa el núcleo de inteligencia geoespacial de UrbanVoice. Su propósito es procesar, analizar y transformar los datos de ubicación crudos en información accionable sobre seguridad urbana. Mientras que otros contextos gestionan el "qué" (el incidente), este contexto se especializa en el "dónde": define las zonas de riesgo, calcula mapas de calor dinámicos y provee algoritmos para determinar la seguridad de los trayectos ciudadanos.

#### 2.6.3.1. Domain Layer

La capa de dominio de Location Management es responsable de la lógica espacial pura. No depende de proveedores de mapas específicos, sino que define cómo se modela el riesgo en el territorio.

**Aggregate Root: `GeospatialZone`**

La entidad `GeospatialZone` es el aggregate root. Representa un área geográfica delimitada (polígono o radio) que consolida múltiples reportes para determinar un nivel de riesgo específico. Es la unidad de consistencia para los mapas de calor.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `ZoneId` (VO) | Identificador único de la zona espacial |
| `boundary` | `GeoBoundary` (VO) | Polígono o radio que define la extensión de la zona |
| `riskLevel` | `RiskIndex` (VO) | Valor numérico (0.0 a 1.0) que cuantifica el peligro |
| `incidentCount` | `int` | Cantidad de reportes activos en la zona |
| `lastActivity` | `DateTime` | Última actualización basada en nuevos incidentes |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `recalculateRisk(incidents: List<IncidentData>)` | public | Actualiza el `RiskIndex` basándose en la densidad y gravedad de los sucesos. |
| `isPointInside(point: Coordinates)` | public | Determina si una coordenada específica pertenece a esta zona de riesgo. |
| `expireOldData(threshold: DateTime)` | public | Reduce el índice de riesgo si no se han reportado incidentes recientes (enfriamiento). |

**Value Objects**

| Value Object | Propósito |
|---|---|
| `Coordinates` | Encapsula Latitud y Longitud con validaciones de rango geográfico. |
| `RiskIndex` | Objeto inmutable que valida que el nivel de riesgo esté en el rango permitido y define su semántica (BAJO, MEDIO, ALTO). |
| `GeoBoundary` | Define la geometría de la zona (Círculo o Polígono). |

**Domain Services**

| Domain Service | Responsabilidad |
|---|---|
| `HeatmapCalculationService` | Ejecuta algoritmos de agrupación (clustering) para convertir puntos individuales en áreas de calor continuas. |
| `RouteSafetyEvaluator` | Recibe una serie de puntos (polilínea) y retorna un reporte de seguridad comparándolo con las `GeospatialZones` activas. |

**Repository Interfaces**

| Interface | Operaciones principales |
|---|---|
| `GeospatialRepository` | `save(zone: GeospatialZone)`, `findZonesNear(point: Coordinates, radius: double)`, `findAllActiveZones()` |

**Domain Events**

| Domain Event | Cuándo se emite | Consumidores |
|---|---|---|
| `RiskLevelEscalated` | Cuando una zona supera un umbral crítico de peligro. | **Notifications** (para alertas críticas de área). |
| `SafeRouteCalculated` | Al completar el análisis de un trayecto solicitado. | **Application Layer** (Auditoría). |

#### 2.6.3.2. Interface Layer


Se encarga de recibir las coordenadas de los usuarios y entregar los datos necesarios para el renderizado del mapa en la aplicación móvil.

**Controllers REST**

| Controller | Endpoints | Capabilities soportadas |
|---|---|---|
| `MapController` | `GET /api/v1/location/heatmap` | Provee la colección de puntos y pesos para el mapa de calor (US01). |
| `GeofencingController` | `POST /api/v1/location/check-point` | Valida si la ubicación actual del usuario representa un riesgo (US05). |
| `RouteController` | `POST /api/v1/location/safe-route` | Calcula el trayecto con menor exposición al riesgo (US06). |

**DTOs / Resources**

| DTO | Uso |
|---|---|
| `HeatmapPointResource` | Coordenada + Intensidad para el frontend de mapas. |
| `RouteRequestResource` | Punto de origen y destino para el cálculo de ruta. |
| `RiskAlertResource` | Información sobre la zona de riesgo detectada cerca del usuario. |


#### 2.6.3.3. Application Layer

Esta capa orquesta la interacción entre los reportes entrantes y la actualización de la inteligencia espacial.

**Command Handlers**

| Command Handler | Flujo |
|---|---|
| `UpdateHeatmapCommandHandler` | Reacciona a nuevos reportes de incidentes para disparar el recálculo de las zonas de riesgo afectadas. |
| `EvaluateRouteSafetyCommandHandler` | Coordina con el servicio de dominio para analizar una ruta y retornar la mejor opción al ciudadano. |

**Query Services**

| Query Service | Responsabilidad |
|---|---|
| `GetNearbyRiskZonesQueryService` | Retorna las zonas peligrosas en el radio de visión actual del usuario para optimizar el rendimiento del mapa móvil. |

#### 2.6.3.4 Infrastructure Layer

Provee el motor de base de datos espacial y la integración con proveedores de mapas externos.

**Persistence (Spatial DB)**

| Componente | Tecnología | Responsabilidad |
|---|---|---|
| `PostGisGeospatialRepository` | PostgreSQL + PostGIS | Utiliza tipos de datos `GEOMETRY` y `GEOGRAPHY` para realizar cálculos espaciales (`ST_DWithin`, `ST_Contains`) a nivel de base de datos. |

**Adapters**

| Adapter | Servicio Externo | Responsabilidad |
|---|---|---|
| `GoogleMapsApiAdapter` | Google Maps Platform | Provee servicios de Geocodificación (direcciones a coordenadas) y trazado inicial de rutas de tráfico. |
| `MatrixDistanceAdapter` | MapBox / Google | Calcula distancias y tiempos estimados para las rutas sugeridas. |

**Mappers Espaciales**

| Mapper | Transformación |
|---|---|
| `GeoJsonMapper` | Convierte los objetos de dominio `Coordinates` y `GeospatialZone` al estándar GeoJSON para facilitar la interoperabilidad con clientes móviles y web. |

#### 2.6.3.5 Bounded Context Software Architecture Component Level Diagrams


En esta subsección se documenta de forma textual la arquitectura a nivel de componentes del Bounded Context *Location Management*. La descomposición parte del container `Location Service`, responsable de la inteligencia geoespacial del sistema, y se organiza en componentes principales agrupados por capas siguiendo un enfoque de arquitectura limpia. Cada componente representa una unidad cohesionada de comportamiento encargada de procesar, transformar o exponer información espacial.

La arquitectura evidencia una separación estricta entre las cuatro capas del contexto. La **Interface Layer**, compuesta por `MapController`, `GeofencingController` y `RouteController`, actúa como punto de entrada para las solicitudes de los clientes. Estos controladores no contienen lógica de negocio; únicamente validan, transforman y delegan las peticiones hacia la Application Layer mediante DTOs como `HeatmapPointResource`, `RouteRequestResource` y `RiskAlertResource`.

La **Application Layer** orquesta los casos de uso del contexto a través de componentes como `UpdateHeatmapCommandHandler` y `EvaluateRouteSafetyCommandHandler`. Estos coordinan la ejecución de operaciones complejas, como la actualización de zonas de riesgo en respuesta a nuevos incidentes o el análisis de rutas seguras. Asimismo, servicios de consulta como `GetNearbyRiskZonesQueryService` optimizan la recuperación de datos geoespaciales según el contexto de visualización del usuario, evitando cargas innecesarias en dispositivos móviles.

En el núcleo del sistema se encuentra la **Domain Layer**, donde reside el aggregate `GeospatialZone`, encargado de encapsular la consistencia del modelo de riesgo espacial. Este aggregate trabaja en conjunto con value objects como `Coordinates`, `GeoBoundary` y `RiskIndex`, que representan conceptos fundamentales del dominio. La lógica compleja se delega a domain services como `HeatmapCalculationService`, responsable de ejecutar algoritmos de clustering sobre datos de incidentes, y `RouteSafetyEvaluator`, que analiza trayectorias para determinar niveles de exposición al riesgo.

Siguiendo el *Dependency Inversion Principle*, la capa de dominio define el puerto `GeospatialRepository` como una abstracción, mientras que la **Infrastructure Layer** provee su implementación concreta mediante `PostGisGeospatialRepository`. Esta implementación utiliza capacidades avanzadas de PostgreSQL con PostGIS para ejecutar operaciones espaciales eficientes como `ST_DWithin` y `ST_Contains`. Adicionalmente, la integración con servicios externos se encapsula a través de adapters como `GoogleMapsApiAdapter` y `MatrixDistanceAdapter`, los cuales permiten delegar tareas como geocodificación y cálculo de rutas sin acoplar el dominio a proveedores específicos.

Los eventos de dominio, como `RiskLevelEscalated` y `SafeRouteCalculated`, son generados por el aggregate o los servicios de dominio cuando se detectan cambios significativos en el estado del sistema. Estos eventos son capturados por la Application Layer y publicados hacia un broker de mensajería, permitiendo que otros bounded contexts, como Notifications, reaccionen de manera desacoplada. Esta arquitectura garantiza un modelo de dominio limpio, altamente cohesivo y preparado para escalar en escenarios de procesamiento geoespacial en tiempo real.

<td><img src="assets/structurizr-92879-LocationManagement-Components.png"/></td>

#### 2.6.3.6 Bounded Context Software Architecture Code Level Diagrams

En esta sección se detallan los diagramas a nivel de código del Bounded Context Location Management, proporcionando una representación más granular de las estructuras internas del sistema. Se incluyen tanto los diagramas de clases del dominio como el diseño de base de datos, permitiendo entender cómo se implementan los conceptos definidos en el modelo de dominio y cómo se persisten los datos geoespaciales.

##### 2.6.3.6.1. Bounded Context Domain Layer Class Diagrams

El modelo de clases del Domain Layer se centra en el aggregate root `GeospatialZone`, que representa la unidad de consistencia del modelo de riesgo espacial. Cada instancia de este aggregate define una región geográfica delimitada —ya sea mediante un polígono o un radio— y mantiene información agregada sobre la actividad delictiva en dicha zona, como el número de incidentes, el nivel de riesgo y la última actualización registrada.

Dentro de este aggregate, los value objects juegan un rol fundamental en la definición del dominio. `Coordinates` encapsula la latitud y longitud asegurando que los valores se mantengan dentro de rangos geográficos válidos. `GeoBoundary` define la geometría de la zona y provee operaciones como la verificación de pertenencia de un punto dentro de sus límites. Por su parte, `RiskIndex` modela el nivel de peligro como un valor numérico acotado, incorporando además su interpretación semántica en términos de riesgo bajo, medio o alto.

A diferencia de entidades tradicionales, estos value objects son inmutables y carecen de identidad propia, lo que refuerza la consistencia del modelo y evita efectos secundarios indeseados. La lógica de negocio compleja no se concentra exclusivamente en el aggregate, sino que se distribuye en domain services especializados. `HeatmapCalculationService` procesa colecciones de incidentes para generar agrupaciones espaciales coherentes, mientras que `RouteSafetyEvaluator` analiza trayectorias completas para producir reportes de seguridad basados en la intersección con zonas de riesgo.

El acceso a los datos se abstrae mediante la interface `GeospatialRepository`, que define operaciones como la persistencia de zonas, la búsqueda por proximidad y la recuperación de zonas activas. Esta abstracción permite desacoplar completamente el dominio de cualquier tecnología de almacenamiento específica. Finalmente, los domain events `RiskLevelEscalated` y `SafeRouteCalculated` permiten comunicar cambios relevantes del dominio hacia otras partes del sistema, facilitando la integración basada en eventos y promoviendo una arquitectura reactiva.

<td><img src="assets/Location Managment - UML.jpg"/></td>

##### 2.6.3.6.2.  Bounded Context Database Design Diagram

El diseño de persistencia del Bounded Context *Location Management* se fundamenta en el uso de una base de datos espacial basada en PostgreSQL con la extensión PostGIS, siguiendo el principio de *database-per-service*. Esto garantiza que el servicio de ubicación mantenga control total sobre sus datos geoespaciales, evitando acoplamientos indebidos con otros contextos.

La tabla principal, `geospatial_zones`, materializa el aggregate root `GeospatialZone`. En ella se almacenan tanto atributos descriptivos como el nivel de riesgo (`risk_level`), la cantidad de incidentes (`incident_count`) y la última actividad (`last_activity`), así como la geometría de la zona mediante el tipo `GEOMETRY`. Este enfoque permite delegar cálculos espaciales directamente a la base de datos, optimizando significativamente el rendimiento en operaciones de proximidad y contención.

Para reforzar la integridad del sistema, el diseño incorpora restricciones a nivel de base de datos. Por ejemplo, el campo `risk_level` se valida para asegurar que su valor se mantenga dentro del rango permitido, mientras que las estructuras geométricas deben cumplir con formatos válidos definidos por PostGIS. Adicionalmente, se emplean índices espaciales del tipo GIST sobre el campo `boundary`, lo que permite ejecutar consultas como `ST_DWithin` y `ST_Contains` de manera eficiente incluso con grandes volúmenes de datos.

La tabla `incidents_reference` actúa como una estructura de soporte para almacenar datos crudos de incidentes que alimentan los algoritmos de cálculo de mapas de calor. Esta separación entre datos agregados y datos base permite recalcular dinámicamente las zonas de riesgo sin comprometer la trazabilidad de la información original.

En términos de rendimiento, el diseño prioriza consultas geoespaciales en tiempo real, especialmente aquellas relacionadas con la detección de zonas cercanas al usuario y el análisis de rutas. Finalmente, el modelo está preparado para escenarios de alta concurrencia mediante estrategias como el uso de timestamps y potencial integración futura de mecanismos de versionado, permitiendo mantener consistencia en un entorno altamente dinámico y orientado a eventos.

<td><img src="assets/Location-database-uml.png"/></td>

### 2.6.4 Bounded Context:Report Managment

El Bounded Context **Report Management** es uno de los contextos core de UrbanVoice y concentra la mayor parte del valor diferencial de la plataforma. Este contexto es responsable de todo el ciclo de vida de un reporte de incidente de seguridad: su creación por parte de un ciudadano, la incorporación de evidencia multimedia, la consulta y filtrado de reportes existentes, la edición por parte del autor original y la exposición de los datos necesarios para que otros contextos, como Geospatial Intelligence y Notifications, puedan reaccionar ante la aparición de nuevos reportes.

#### 2.6.4.1. Domain Layer

La Domain Layer concentra el modelo del dominio del contexto Report Management. Aquí se ubican las clases que representan los conceptos del negocio, sus reglas y sus invariantes, sin dependencia alguna hacia frameworks, bases de datos, servicios externos ni tecnologías específicas. Esta capa es el corazón del Bounded Context y cualquier otra capa del contexto depende de ella, nunca al revés.

**Aggregate Root: `Report`**

La entidad `Report` es el aggregate root del contexto. Un reporte es la unidad de consistencia transaccional: cuando un ciudadano crea un reporte, adjunta evidencia o lo edita, todas esas operaciones atraviesan necesariamente al aggregate root para garantizar que las invariantes del reporte se mantengan en todo momento. Por ejemplo, un reporte no puede existir sin una ubicación válida, un reporte publicado anónimamente no puede exponer el id del autor, y solo el autor original puede editar un reporte.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `ReportId` (VO) | Identificador único del reporte |
| `authorId` | `UserId` (VO) | Identificador del ciudadano autor (referencia cruzada a User Profile) |
| `category` | `IncidentCategory` (VO) | Tipo de incidente reportado |
| `location` | `IncidentLocation` (VO) | Coordenadas geográficas del incidente |
| `content` | `ReportContent` (VO) | Título y descripción del reporte |
| `anonymity` | `AnonymityLevel` (Enum) | Nivel de anonimato: PUBLIC o ANONYMOUS |
| `status` | `ReportStatus` (Enum) | Estado del reporte: DRAFT, PUBLISHED, UNDER_REVIEW, APPROVED, REJECTED |
| `evidence` | `List<MediaEvidence>` | Colección de evidencias multimedia adjuntadas |
| `reportedAt` | `DateTime` | Fecha y hora en que ocurrió el incidente |
| `createdAt` | `DateTime` | Fecha y hora de creación del reporte en el sistema |
| `updatedAt` | `DateTime` | Fecha y hora de la última modificación |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `publish()` | public | Publica el reporte (pasa de DRAFT a PUBLISHED). Emite el evento `ReportPublished` |
| `attachEvidence(media: MediaEvidence)` | public | Adjunta una evidencia al reporte. Emite el evento `EvidenceAttached` |
| `removeEvidence(evidenceId: EvidenceId)` | public | Remueve una evidencia del reporte (solo permitido en DRAFT o si el autor es quien edita) |
| `editContent(content: ReportContent, editor: UserId)` | public | Edita el contenido. Invariante: solo el autor puede editarlo. Emite `ReportEdited` |
| `changeAnonymity(level: AnonymityLevel, editor: UserId)` | public | Cambia el nivel de anonimato. Invariante: solo el autor puede cambiarlo |
| `submitForReview()` | public | Cambia el estado a UNDER_REVIEW para moderación |
| `approve(moderator: UserId)` | public | Aprueba el reporte. Emite `ReportApproved` |
| `reject(moderator: UserId, reason: string)` | public | Rechaza el reporte. Emite `ReportRejected` |
| `isEditableBy(userId: UserId)` | public | Retorna `true` si el usuario puede editar el reporte |

**Entidad interna: `MediaEvidence`**

`MediaEvidence` es una entidad interna del aggregate `Report`. No es un aggregate root porque su ciclo de vida depende completamente del reporte al que pertenece; no tiene sentido que exista una evidencia sin un reporte asociado.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `EvidenceId` (VO) | Identificador único de la evidencia |
| `mediaType` | `MediaType` (Enum) | Tipo: IMAGE, AUDIO, VIDEO |
| `storageUrl` | `StorageUrl` (VO) | URL del archivo almacenado en Cloud Storage |
| `fileSize` | `FileSize` (VO) | Tamaño del archivo en bytes |
| `uploadedAt` | `DateTime` | Fecha y hora en que se subió la evidencia |

**Value Objects**

Los value objects encapsulan conceptos del dominio que se identifican por su valor y no por identidad. Son inmutables y contienen las validaciones intrínsecas del concepto que representan.

| Value Object | Propósito |
|---|---|
| `ReportId` | Identificador único del reporte (UUID v4). Inmutable |
| `EvidenceId` | Identificador único de una evidencia multimedia |
| `UserId` | Referencia al autor del reporte (compartido con otros contextos) |
| `IncidentLocation` | Encapsula latitud y longitud validadas. Miembro del Shared Kernel con Geospatial Intelligence |
| `IncidentCategory` | Categoría del incidente (robo, asalto, vandalismo, etc.). Miembro del Shared Kernel con Geospatial Intelligence |
| `ReportContent` | Encapsula título (3-100 caracteres) y descripción (10-1000 caracteres). Valida que no esté vacío |
| `StorageUrl` | URL válida hacia el archivo en Cloud Storage. Valida formato URL |
| `FileSize` | Tamaño del archivo en bytes. Invariante: máximo 10 MB por archivo |

**Enumerations**

| Enum | Valores | Propósito |
|---|---|---|
| `ReportStatus` | DRAFT, PUBLISHED, UNDER_REVIEW, APPROVED, REJECTED | Estado del reporte en su ciclo de vida |
| `AnonymityLevel` | PUBLIC, ANONYMOUS | Nivel de exposición de la identidad del autor |
| `MediaType` | IMAGE, AUDIO, VIDEO | Tipo de evidencia multimedia |

**Domain Services**

Los domain services encapsulan lógica de dominio que no pertenece naturalmente a una entidad o value object.

| Domain Service | Responsabilidad |
|---|---|
| `ReportFilterService` | Aplica criterios de filtrado complejos sobre una colección de reportes (por categoría, por radio geográfico, por rango de fechas, por nivel de riesgo asociado) |
| `ReportVisibilityPolicy` | Determina qué campos de un reporte son visibles para un usuario dado, considerando el nivel de anonimato y el rol del solicitante |

**Repository Interfaces (abstracciones)**

Las interfaces de repositorio se declaran en el Domain Layer. Su implementación vive en el Infrastructure Layer siguiendo el Dependency Inversion Principle.

| Interface | Operaciones principales |
|---|---|
| `ReportRepository` | `save(report: Report)`, `findById(id: ReportId)`, `findByAuthor(authorId: UserId)`, `findByFilters(criteria: ReportFilterCriteria)`, `delete(id: ReportId)` |

**Domain Events**

Los domain events representan hechos relevantes que ocurrieron en el dominio. Son inmutables y se publican cuando las invariantes del aggregate lo permiten.

| Domain Event | Cuándo se emite | Consumidores |
|---|---|---|
| `ReportPublished` | Cuando un reporte pasa de DRAFT a PUBLISHED | Geospatial Intelligence, Notifications |
| `EvidenceAttached` | Cuando se adjunta una evidencia a un reporte | Interno del contexto |
| `ReportEdited` | Cuando el autor edita el contenido del reporte | Notifications |
| `ReportApproved` | Cuando un moderador aprueba el reporte | Geospatial Intelligence, Notifications |
| `ReportRejected` | Cuando un moderador rechaza el reporte | Notifications |
| `IncidentReportedNearby` | Policy derivada de `ReportPublished` para ciudadanos cercanos | Notifications |

**Factories**

| Factory | Propósito |
|---|---|
| `ReportFactory` | Centraliza la creación de reportes válidos a partir de un `SubmitReportCommand`. Valida todas las precondiciones antes de instanciar el aggregate |

#### 2.6.4.2. Interface Layer

La Interface Layer es la capa más externa del Bounded Context del lado entrante. Su responsabilidad es exponer las capabilities del contexto al mundo exterior, como aplicaciones móviles, web admin y otros servicios, y traducir los requests entrantes al modelo de la Application Layer. En esta capa residen los controllers REST y los consumers de eventos asíncronos.

**Controllers REST**

Los controllers son la puerta de entrada HTTP al contexto. Siguen el patrón thin controller: reciben el request, lo traducen a un command o query, delegan en el Application Layer y retornan el DTO de respuesta. No contienen lógica de negocio.

| Controller | Endpoints | Capabilities soportadas |
|---|---|---|
| `ReportController` | `POST /api/v1/reports` (crear), `GET /api/v1/reports/{id}` (detalle), `PUT /api/v1/reports/{id}` (editar), `DELETE /api/v1/reports/{id}` (eliminar), `GET /api/v1/reports` (listar con filtros) | CRUD completo de reportes, alineado con US01, US02, US04, US09, US10 y US13 |
| `EvidenceController` | `POST /api/v1/reports/{id}/evidence` (adjuntar), `DELETE /api/v1/reports/{id}/evidence/{evidenceId}` (remover) | Gestión de evidencia multimedia, alineado con US03 |
| `ModerationController` | `POST /api/v1/reports/{id}/moderation/approve`, `POST /api/v1/reports/{id}/moderation/reject`, `GET /api/v1/reports/moderation/queue` | Panel de moderación, alineado con US11 |

**Resources / DTOs**

Cada endpoint trabaja con DTOs en lugar de exponer directamente las clases del Domain Layer. Esto evita acoplar la API pública a la estructura interna del dominio.

| DTO | Tipo | Uso |
|---|---|---|
| `SubmitReportResource` | Input | Payload del request `POST` para crear un reporte |
| `EditReportResource` | Input | Payload del request `PUT` para editar un reporte |
| `AttachEvidenceResource` | Input | Payload para adjuntar evidencia (contiene metadata y URL prefirmada) |
| `ReportSummaryResource` | Output | Versión reducida del reporte para listados |
| `ReportDetailResource` | Output | Versión completa del reporte para vista de detalle |
| `ReportFilterResource` | Input (query params) | Criterios de filtrado para listados |

**Assemblers**

Los assemblers convierten entre DTOs de la Interface Layer y objetos del Application Layer o Domain Layer.

| Assembler | Transformación |
|---|---|
| `FromSubmitReportResourceAssembler` | `SubmitReportResource` a `SubmitReportCommand` |
| `FromEditReportResourceAssembler` | `EditReportResource` a `EditReportCommand` |
| `ReportResourceFromEntityAssembler` | `Report` a `ReportDetailResource` |

**Event Consumers**

| Consumer | Evento escuchado | Acción |
|---|---|---|
| `UserRegisteredConsumer` | `UserRegistered` (publicado por IAM) | Preparar cache local de `UserId` válidos para validación rápida al recibir nuevos reportes |

#### 2.6.4.3. Application Layer

La Application Layer orquesta los flujos de proceso del negocio que involucran al Bounded Context. Aquí viven las clases responsables de recibir commands y queries, coordinar con el Domain Layer, gestionar la transaccionalidad y publicar los domain events hacia el resto del sistema. Esta capa no contiene reglas de negocio; solo coordinación.

Se adopta el patrón **CQRS** (Command Query Responsibility Segregation) ligero: los flujos de escritura pasan por Command Handlers y los flujos de lectura por Query Services. Esta separación permite optimizar cada ruta independientemente.

**Command Handlers**

Cada command representa una intención del usuario o del sistema de cambiar el estado del dominio.

| Command Handler | Command procesado | Flujo |
|---|---|---|
| `SubmitReportCommandHandler` | `SubmitReportCommand` | Valida el command, invoca al `ReportFactory` para crear el aggregate, persiste vía `ReportRepository` y publica `ReportPublished` |
| `AttachEvidenceCommandHandler` | `AttachEvidenceCommand` | Recupera el aggregate, invoca `report.attachEvidence()`, persiste y publica `EvidenceAttached` |
| `EditReportCommandHandler` | `EditReportCommand` | Recupera el aggregate, valida que el editor sea el autor, invoca `report.editContent()`, persiste y publica `ReportEdited` |
| `ApproveReportCommandHandler` | `ApproveReportCommand` | Recupera el aggregate, invoca `report.approve()`, persiste y publica `ReportApproved` |
| `RejectReportCommandHandler` | `RejectReportCommand` | Recupera el aggregate, invoca `report.reject()`, persiste y publica `ReportRejected` |

**Query Services**

Los query services manejan las operaciones de lectura. Retornan DTOs directamente sin pasar por aggregates completos cuando es posible, optimizando para el caso de uso de consulta.

| Query Service | Query soportada | Retorno |
|---|---|---|
| `GetReportByIdQueryService` | `GetReportByIdQuery(id)` | `ReportDetailResource` |
| `ListReportsByAuthorQueryService` | `ListReportsByAuthorQuery(authorId)` | `List<ReportSummaryResource>` |
| `SearchReportsQueryService` | `SearchReportsQuery(criteria)` | `Page<ReportSummaryResource>` filtrada y paginada |
| `GetModerationQueueQueryService` | `GetModerationQueueQuery()` | Cola de reportes en estado `UNDER_REVIEW` |

**Event Handlers**

Los event handlers reaccionan a domain events propios o externos al contexto.

| Event Handler | Evento | Acción |
|---|---|---|
| `ReportPublishedEventHandler` | `ReportPublished` | Publica el evento en el message broker para que Geospatial Intelligence y Notifications reaccionen |
| `EvidenceAttachedEventHandler` | `EvidenceAttached` | Actualiza el modelo de lectura del reporte |

**Application Services**

| Application Service | Responsabilidad |
|---|---|
| `ReportApplicationService` | Fachada del contexto que coordina Command Handlers y Query Services. Es el punto de entrada unificado desde la Interface Layer |
| `EvidenceUploadService` | Coordina el proceso de generación de URL prefirmada para que el cliente suba directamente a Cloud Storage y luego registre la evidencia en el reporte |

#### 2.6.4.4 Infrastructure Layer

La Infrastructure Layer provee implementaciones concretas de las abstracciones definidas en el Domain Layer y gestiona la integración con tecnologías externas al contexto: base de datos, message broker, servicios de almacenamiento en la nube, entre otros. Esta capa es la única que depende directamente de frameworks específicos como Spring Data JPA, Spring AMQP o los SDKs de cloud providers.

**Repository Implementations**

Implementan las interfaces declaradas en el Domain Layer.

| Implementación | Interface que implementa | Tecnología |
|---|---|---|
| `JpaReportRepository` | `ReportRepository` | Spring Data JPA sobre PostgreSQL |

**JPA Entities**

Las JPA entities son el equivalente técnico de las domain entities, decoradas con anotaciones de persistencia. Se mantienen separadas de las domain entities para no contaminar el modelo de dominio con preocupaciones de infraestructura.

| JPA Entity | Mapeo |
|---|---|
| `ReportJpaEntity` | Tabla `reports` |
| `MediaEvidenceJpaEntity` | Tabla `media_evidence` |
| `ReportCategoryJpaEntity` | Tabla de lookup `incident_categories` |

**Mappers Domain a JPA**

| Mapper | Transformación |
|---|---|
| `ReportJpaMapper` | `Report` (domain) a `ReportJpaEntity` (JPA) y viceversa |
| `MediaEvidenceJpaMapper` | `MediaEvidence` (domain) a `MediaEvidenceJpaEntity` (JPA) y viceversa |

**External Service Adapters**

Implementan puertos de salida hacia servicios externos.

| Adapter | Servicio externo | Responsabilidad |
|---|---|---|
| `CloudStorageAdapter` | AWS S3 o Firebase Storage | Genera URLs prefirmadas para upload directo y URLs de lectura con expiración |
| `EventPublisherAdapter` | RabbitMQ (vía Spring AMQP) | Publica los domain events en el exchange correspondiente |
| `UserProfileClientAdapter` | Profile Service (vía REST) | Consulta información pública del autor cuando se requiere mostrar un reporte no anónimo |

**Configuration**

| Clase de configuración | Propósito |
|---|---|
| `ReportingContextConfig` | Registra los beans de Spring del contexto, configura transacciones y wiring de handlers |
| `RabbitMqConfig` | Declara exchanges, queues y bindings del contexto |

#### 2.6.4.5 Bounded Context Software Architecture Component Level Diagrams

En esta subsección se documenta de forma textual la arquitectura a nivel de componentes del Bounded Context Report Management. La descomposición parte del container `Incident Service` o `Report Service`, que implementa este contexto, y lo organiza en componentes principales agrupados por capas. Cada componente representa una agrupación coherente de clases que colaboran para proveer una capability específica del negocio.

La arquitectura evidencia una separación estricta entre las cuatro capas del contexto. La Interface Layer, compuesta por `ReportController`, `EvidenceController`, `ModerationController` y `UserRegisteredConsumer`, solo conoce a la Application Layer. La Application Layer coordina el flujo mediante `ReportApplicationService`, `EvidenceUploadService`, los distintos Command Handlers y los Query Services. A su vez, estos componentes interactúan con el Domain Layer, donde residen el aggregate `Report`, la factory `ReportFactory`, los domain services `ReportFilterService` y `ReportVisibilityPolicy`, además de la abstracción `ReportRepository`.

Siguiendo el Dependency Inversion Principle, el Domain Layer declara el puerto `ReportRepository` como interface, mientras que en tiempo de ejecución la Infrastructure Layer provee la implementación concreta `JpaReportRepository`. Del mismo modo, la integración con servicios externos se encapsula mediante adapters como `CloudStorageAdapter`, `EventPublisherAdapter` y `UserProfileClientAdapter`, evitando que el dominio dependa directamente de detalles de infraestructura.

Los domain events emitidos por el aggregate son interceptados por event handlers de la Application Layer, que luego los publican al broker correspondiente para que otros bounded contexts, como Geospatial Intelligence y Notifications, reaccionen sin acoplamiento directo. Esta organización permite mantener un modelo de dominio limpio, cohesionando la lógica del reporte y dejando las preocupaciones técnicas en la capa de infraestructura.

<td><img src="assets/ReportManagementComponents.png"/></td>

#### 2.6.4.6 Bounded Context Software Architecture Code Level Diagrams

En esta subsección se describe, de manera textual, la arquitectura a nivel de código del Bounded Context Report Management. El objetivo es dejar documentados los dos artefactos principales del diseño detallado: el modelo de clases del Domain Layer y el diseño de persistencia relacional que soporta al contexto, sin insertar diagramas visuales en esta versión.

##### 2.6.4.6.1. Bounded Context Domain Layer Class Diagrams

El modelo de clases del Domain Layer gira alrededor del aggregate root `Report`, que concentra la consistencia transaccional del contexto. Dentro de este aggregate se encuentra la entidad interna `MediaEvidence`, cuya existencia depende completamente del reporte al que pertenece. La relación entre ambas clases es de composición, ya que una evidencia no puede existir fuera del ciclo de vida del reporte.

Los value objects, como `ReportId`, `EvidenceId`, `UserId`, `IncidentLocation`, `IncidentCategory`, `ReportContent`, `StorageUrl` y `FileSize`, forman parte integral del aggregate y encapsulan las validaciones propias del dominio. Estos objetos son inmutables y se modelan por valor, no por identidad, reforzando la semántica del dominio y reduciendo inconsistencias en las reglas de negocio.

Las enumeraciones `ReportStatus`, `AnonymityLevel` y `MediaType` permiten representar estados y categorías cerradas del dominio de forma explícita. Sobre este núcleo trabajan los domain services `ReportFilterService`, `ReportVisibilityPolicy` y `ReportFactory`, que operan sobre el aggregate sin formar parte estructural de él. Finalmente, la interface `ReportRepository` abstrae la persistencia del aggregate, cumpliendo con el principio de inversión de dependencias y manteniendo al dominio desacoplado de la infraestructura.

<td><img src="assets/Report Management Domain Layer.png"/></td>

##### 2.6.4.6.2. Bounded Context Database Design Diagram

El diseño de base de datos relacional que soporta el Bounded Context Report Management sigue el principio de database-per-service: el servicio responsable del contexto mantiene su propia instancia de PostgreSQL y ningún otro servicio accede directamente a estas tablas. La tabla central es `reports`, donde se materializa el aggregate root `Report`. Allí se descomponen en columnas planas los value objects del dominio, como el contenido del reporte, la ubicación del incidente, el nivel de anonimato y el estado del flujo de vida.

En `reports` se emplean restricciones `CHECK` para reforzar a nivel de base de datos las mismas invariantes ya protegidas en el Domain Layer. Por ejemplo, se valida que `status` solo acepte los cinco estados permitidos, que `anonymity_level` solo reciba valores válidos y que las coordenadas geográficas se mantengan dentro de los rangos correctos. Esta estrategia implementa defense-in-depth y reduce la posibilidad de que datos inválidos ingresen al sistema.

La tabla `media_evidence` representa la entidad interna `MediaEvidence` y se relaciona con `reports` en una cardinalidad uno a muchos. Esta tabla almacena únicamente metadatos de los archivos, como tipo, URL y tamaño, mientras que el contenido real vive en Cloud Storage. Debido a que las evidencias no tienen sentido fuera del reporte, esta relación se modela con borrado en cascada.

La tabla `incident_categories` funciona como lookup table para las categorías predefinidas del sistema, tales como robo, asalto o vandalismo. En lugar de eliminar físicamente una categoría, se usa el flag `is_active`, lo que permite mantener consistencia histórica sobre reportes ya emitidos que referencian categorías descontinuadas.

Por su parte, `moderation_log` mantiene la trazabilidad del proceso de moderación. Cada aprobación o rechazo genera una entrada asociada al reporte y al moderador que tomó la decisión, permitiendo auditoría completa y análisis posterior del desempeño del flujo de moderación.

La tabla `report_filter_presets` permite almacenar filtros frecuentes definidos por los usuarios. El uso de un campo `JSONB` para `criteria_json` facilita la evolución del modelo de búsqueda sin requerir migraciones constantes del esquema. Este enfoque da flexibilidad a la personalización de consultas y soporta mejor la ampliación futura de criterios.

En cuanto al desempeño, los índices priorizan tres patrones de acceso críticos: búsqueda por autor para la vista de "mis reportes", búsqueda por estado para la cola de moderación y búsqueda geográfica para escenarios de heatmap y alertas por proximidad. Finalmente, la columna `version` en `reports` habilita optimistic locking a nivel de JPA, evitando conflictos cuando dos actores intentan modificar simultáneamente el mismo reporte.

<td><img src="assets/Report Management Database.png"/></td>

### 2.6.5 Bounded Context: Notification Management

El Bounded Context **Notification Management** es un componente vital para la propuesta de valor proactiva de UrbanVoice. Este contexto es responsable de mantener al ciudadano informado y seguro en tiempo real. Se encarga de gestionar el ciclo de vida de las alertas emitidas por el sistema, notificar al usuario cuando ingresa a una zona de riesgo (geofencing), avisarle cuando se crea un nuevo reporte de incidente cerca de su ubicación, y gestionar las sesiones de "compartir ubicación" (Live Tracking) entre usuarios mediante códigos de acceso.

El modelo de dominio presentado en esta sección es consistente con lo identificado en el Design-Level EventStorming. Se establecieron commands principales como generar alerta de proximidad, marcar notificación como leída y unirse a una sesión de ubicación compartida; los domain events asociados como Alerta Emitida, Zona Peligrosa Detectada y Ubicación Compartida; y los read models necesarios como la bandeja de notificaciones, el detalle de la alerta y la vista en vivo del mapa compartido.

A continuación, se presenta el diseño del contexto organizado en las cuatro capas estándar de una arquitectura hexagonal o aplicada a DDD. Posteriormente se documenta, de forma textual, la arquitectura a nivel de componente y a nivel de código.

#### 2.6.5.1. Domain Layer

La Domain Layer concentra el modelo del dominio del contexto Notification Management. Aquí se ubican las clases que representan las alertas, las sesiones de ubicación compartida y sus reglas de negocio, manteniendo total independencia de frameworks, bases de datos o servicios de mensajería externos (como Firebase Cloud Messaging).

**Aggregate Root: `SecurityAlert` (Notificación)**

La entidad `SecurityAlert` es el aggregate root principal para el flujo de notificaciones. Representa una alerta individual despachada a un ciudadano específico. Toda transición de estado (por ejemplo, de "no leída" a "leída" o "descartada") debe pasar por este aggregate.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `AlertId` (VO) | Identificador único de la alerta |
| `recipientId` | `UserId` (VO) | Identificador del ciudadano receptor de la notificación |
| `type` | `AlertType` (Enum) | Tipo de alerta: PROXIMITY_WARNING, NEW_INCIDENT, SYSTEM_UPDATE |
| `content` | `AlertContent` (VO) | Título, mensaje detallado y severidad de la alerta |
| `referenceLocation` | `LocationCoordinates` (VO) | Coordenadas asociadas a la alerta (opcional) |
| `status` | `AlertStatus` (Enum) | Estado actual: UNREAD, READ, DISMISSED |
| `issuedAt` | `DateTime` | Fecha y hora en que el sistema generó la alerta |
| `readAt` | `DateTime` | Fecha y hora en que el usuario leyó la alerta (nullable) |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `markAsRead()` | public | Cambia el estado de UNREAD a READ y registra la fecha. Emite `AlertRead` |
| `dismiss()` | public | Cambia el estado a DISMISSED ocultándola de la bandeja activa |
| `isUrgent()` | public | Retorna `true` si el nivel de severidad en el contenido es HIGH o CRITICAL |

**Aggregate Root: `LocationShareSession`**

Este segundo aggregate root maneja el flujo de "compartir ubicación" evidenciado en el EventStorming. Gestiona el código de acceso temporal y los usuarios que tienen permiso para visualizar la ubicación del emisor.

| Atributo | Tipo | Descripción |
|---|---|---|
| `id` | `SessionId` (VO) | Identificador único de la sesión de rastreo |
| `ownerId` | `UserId` (VO) | Identificador del ciudadano que comparte su ubicación |
| `accessCode` | `ShareCode` (VO) | Código alfanumérico único para unirse a la sesión |
| `status` | `TrackingStatus` (Enum) | Estado: ACTIVE, PAUSED, EXPIRED |
| `viewers` | `List<UserId>` | Lista de usuarios que han ingresado el código exitosamente |
| `expiresAt` | `DateTime` | Fecha y hora de caducidad automática de la sesión |

**Métodos principales**

| Método | Visibilidad | Descripción |
|---|---|---|
| `addViewer(viewerId: UserId, code: ShareCode)` | public | Invariante: Verifica que el código coincida y la sesión esté activa. Emite `ViewerJoined` |
| `terminate()` | public | Cambia el estado a EXPIRED, cerrando el acceso. Emite `SessionTerminated` |

**Value Objects**

| Value Object | Propósito |
|---|---|
| `AlertId` | Identificador único de la notificación (UUID v4) |
| `UserId` | Identificador del usuario (Shared Kernel) |
| `AlertContent` | Encapsula el título (ej. "¡Peligro! Zona Insegura"), mensaje y el nivel de Severity |
| `ShareCode` | Código seguro de 6 dígitos autogenerado para compartir ubicación |
| `LocationCoordinates` | Encapsula latitud y longitud. Usado para mostrar la alerta en el mapa |

**Enumerations**

| Enum | Valores | Propósito |
|---|---|---|
| `AlertStatus` | UNREAD, READ, DISMISSED | Ciclo de vida de visualización de la alerta |
| `AlertType` | PROXIMITY_WARNING, NEW_INCIDENT, SYSTEM_UPDATE | Clasifica el motivo de la notificación |
| `TrackingStatus` | ACTIVE, PAUSED, EXPIRED | Controla si la ubicación sigue siendo visible |

**Domain Services**

| Domain Service | Responsabilidad |
|---|---|
| `ProximityAlertService` | Evalúa si las coordenadas actuales del usuario intersectan con un área de riesgo (Geofence) para emitir un PROXIMITY_WARNING |

**Repository Interfaces (abstracciones)**

| Interface | Operaciones principales |
|---|---|
| `SecurityAlertRepository` | `save(alert: SecurityAlert)`, `findUnreadByUserId(userId: UserId)`, `markAllAsRead(userId: UserId)` |
| `LocationShareRepository` | `save(session: LocationShareSession)`, `findByAccessCode(code: ShareCode)`, `findActiveByOwnerId(ownerId: UserId)` |

**Domain Events**

| Domain Event | Cuándo se emite | Consumidores |
|---|---|---|
| `AlertIssued` | Cuando se crea y despacha una nueva alerta | Interno (para enviar Push Notification) |
| `AlertRead` | Cuando el usuario visualiza la alerta | Interno |
| `LocationShareCreated` | Cuando se genera un nuevo código de ubicación | Externo (notificar a contactos sugeridos) |
| `ViewerJoined` | Cuando alguien ingresa el código correctamente | Interno (notifica al owner que alguien lo está viendo) |

#### 2.6.5.2. Interface Layer

La Interface Layer expone los endpoints para que la aplicación móvil consulte sus notificaciones y gestione las sesiones de mapa. También contiene los consumidores de eventos asíncronos provenientes de otros contextos (como Report Management).

**Controllers REST**

| Controller | Endpoints | Capabilities soportadas |
|---|---|---|
| `AlertsController` | `GET /api/v1/notifications`, `PATCH /api/v1/notifications/{id}/read` | Bandeja de entrada de alertas y actualización de estado |
| `LocationSharingController` | `POST /api/v1/location-share` (crear), `POST /api/v1/location-share/join` (ingresar código) | Flujo para compartir ubicación y visualizar a otros |

**Resources / DTOs**

| DTO | Tipo | Uso |
|---|---|---|
| `JoinSessionRequest` | Input | Contiene el `accessCode` ingresado por el usuario para ver un mapa |
| `AlertSummaryResponse` | Output | Lista de notificaciones para la bandeja de la app |
| `LocationSessionResponse` | Output | Devuelve el estado de la sesión y el código generado |

**Event Consumers**

| Consumer | Evento escuchado | Acción |
|---|---|---|
| `IncidentReportedConsumer` | `ReportPublished` (desde Report Management) | Desencadena el cálculo de usuarios cercanos para emitirles un `SecurityAlert` de tipo NEW_INCIDENT |

#### 2.6.5.3. Application Layer

Esta capa orquesta los casos de uso, suscribiéndose a eventos externos y despachando commands hacia el Domain Layer. Gestiona el patrón CQRS para separar la consulta de alertas de la generación de las mismas.

**Command Handlers**

| Command Handler | Command procesado | Flujo |
|---|---|---|
| `DispatchAlertCommandHandler` | `DispatchAlertCommand` | Instancia un `SecurityAlert`, persiste en base de datos y publica `AlertIssued` para que la infraestructura envíe la Push Notification |
| `MarkAlertReadCommandHandler` | `MarkAlertReadCommand` | Recupera el aggregate, invoca `markAsRead()`, y persiste |
| `CreateShareSessionCommandHandler` | `CreateShareSessionCommand` | Invoca factory para generar `LocationShareSession` con código único, persiste y publica evento |
| `JoinShareSessionCommandHandler` | `JoinShareSessionCommand` | Busca sesión por código, invoca `session.addViewer()`, autoriza acceso al socket de ubicación y persiste |

**Query Services**

| Query Service | Query soportada | Retorno |
|---|---|---|
| `GetUserAlertsQueryService` | `GetUserAlertsQuery(userId)` | `List<AlertSummaryResponse>` ordenado por fecha |
| `GetActiveSessionQueryService` | `GetActiveSessionQuery(code)` | `LocationSessionResponse` |

**Event Handlers**

| Event Handler | Evento | Acción |
|---|---|---|
| `AlertIssuedEventHandler` | `AlertIssued` | Delega al `PushNotificationAdapter` el envío a dispositivos iOS/Android |
| `NewIncidentEventHandler` | `ReportPublished` | Llama al `ProximityAlertService` para buscar usuarios en un radio de X km e invocar el `DispatchAlertCommand` |

#### 2.6.5.4. Infrastructure Layer

La Infrastructure Layer conecta el modelo del dominio con las tecnologías reales: bases de datos, WebSockets para el mapa en vivo y Firebase para notificaciones push.

**Repository Implementations**

| Implementación | Interface que implementa | Tecnología |
|---|---|---|
| `JpaSecurityAlertRepository` | `SecurityAlertRepository` | Spring Data JPA sobre PostgreSQL |
| `JpaLocationShareRepository` | `LocationShareRepository` | Spring Data JPA sobre PostgreSQL |

**JPA Entities y Mappers**

| JPA Entity / Mapper | Mapeo |
|---|---|
| `SecurityAlertJpaEntity` | Tabla `security_alerts`. Índices en `recipient_id` y `status` para consultas rápidas |
| `LocationShareJpaEntity` | Tabla `location_share_sessions`. Índice UNIQUE en `access_code` |
| `NotificationJpaMapper` | Transforma `SecurityAlert` (domain) a `SecurityAlertJpaEntity` y viceversa |

**External Service Adapters**

| Adapter | Servicio externo | Responsabilidad |
|---|---|---|
| `FcmPushNotificationAdapter` | Firebase Cloud Messaging (FCM) | Toma el evento `AlertIssued` y envía un Push Notification real al token del smartphone del usuario |
| `WebSocketLocationAdapter` | Spring WebSocket / STOMP | Mantiene el canal abierto y emite las coordenadas en tiempo real a los viewers autorizados en el `LocationShareSession` |

#### 2.6.5.5 Bounded Context Software Architecture Component Level Diagrams

En esta subsección se documenta la arquitectura a nivel de componentes del Bounded Context Notification Management. La descomposición parte del contenedor Notification Service, organizándolo por capas.

La Interface Layer expone los endpoints a través de `AlertsController` y `LocationSharingController`, mientras el `IncidentReportedConsumer` escucha activamente el Message Broker (RabbitMQ/Kafka). Estos componentes derivan el tráfico hacia la Application Layer, donde los Command Handlers (como `DispatchAlertCommandHandler` y `JoinShareSessionCommandHandler`) coordinan la lógica.

El Domain Layer encapsula el core con los aggregates `SecurityAlert` y `LocationShareSession`, protegiendo invariantes como la validación del código de acceso temporal. Finalmente, la Infrastructure Layer provee la persistencia mediante `JpaSecurityAlertRepository` y ejecuta las acciones externas mediante adaptadores especializados: `FcmPushNotificationAdapter` para emitir las alertas visuales en el dispositivo y `WebSocketLocationAdapter` para el streaming de coordenadas en vivo durante la compartición de ubicación.

<td><img src="assets/Component-Notification-Managment.svg"/></td>

#### 2.6.5.6 Bounded Context Software Architecture Code Level Diagrams

En esta subsección se describe la arquitectura a nivel de código del Bounded Context Notification Management, detallando su modelo de clases y diseño de persistencia relacional.

##### 2.6.5.6.1. Bounded Context Domain Layer Class Diagrams

El modelo de clases del Domain Layer presenta dos aggregates independientes. El primero es `SecurityAlert`, que centraliza el estado de las notificaciones (UNREAD, READ) y su contenido (encapsulado en el VO `AlertContent`). Incluye un VO `LocationCoordinates` para alertas vinculadas a eventos geográficos.

El segundo aggregate es `LocationShareSession`, diseñado para gestionar la característica de "compartir ubicación". Sus atributos incluyen el `ShareCode` autogenerado, el `ownerId` y la lista de viewers (espectadores). Este aggregate expone métodos como `addViewer(code)` que validan internamente si la sesión sigue activa y si el código ingresado coincide antes de permitir que un ciudadano monitoree a otro, asegurando la privacidad en todo momento.

<td><img src="assets/Class-Diagram-Notification-Managment.png"/></td>

##### 2.6.5.6.2. Bounded Context Database Design Diagram

El diseño relacional para el Bounded Context Notification Management consta de dos tablas principales bajo el esquema database-per-service. La tabla `security_alerts` persiste las notificaciones. Se optimiza el acceso de lectura masiva creando un índice compuesto en las columnas `recipient_id` y `status`, lo que garantiza que la consulta para contar "notificaciones no leídas" en la aplicación móvil responda en milisegundos.

Por otro lado, la tabla `location_share_sessions` persiste los datos de tracking. Posee una restricción UNIQUE en la columna `access_code` para garantizar que no existan colisiones cuando dos usuarios generen un código de vinculación. Una tabla intermedia `session_viewers` almacena la relación de qué usuarios (`viewer_id`) se han unido exitosamente a qué sesión (`session_id`), utilizando borrado en cascada para evitar registros huérfanos una vez que la sesión de emergencia expira.


<br>
<p align="center">
  <td><img src="assets/Data-Base-Notification-Managment.jpeg"/></td>
</p>
<br>

# Capítulo III: Solution UX/UI Design

## 3.1. Style Guidelines

UrbanVoice es una plataforma de seguridad ciudadana para Lima Metropolitana, por lo que la identidad visual prioriza **confianza institucional** y **claridad operativa**. La paleta se construye sobre un azul institucional (`#0062FF`) que comunica seriedad y respaldo, complementado por una escala funcional de alertas: rojo (`#DC2626`) para riesgo alto, ámbar (`#F59E0B`) para advertencias y verde (`#10B981`) para zonas seguras y confirmaciones positivas. La tipografía combina Geist (headings, geométrica y técnica), Inter (body, alta legibilidad) y Geist Mono (datos y metadatos), todas sans-serif modernas. Los componentes usan radios suaves (8–20 px) para tarjetas y forma píldora para acciones primarias, con elevación sutil mediante sombras de baja intensidad.

A continuación se muestra el design system base con los tokens de color y los nueve componentes reutilizables (StatusBar, TabBar, BtnPrimary, BtnSecondary, Input, IncidentCard, AlertBanner, FAB, Chip) que se aplican a todas las pantallas de la app móvil:

<p align="center">
  <img src="assets/ui/overview/00-design-system.png" alt="UrbanVoice — Design System" width="900"/>
</p>

### 3.1.1.1. General Style Guidelines 

* **Branding:** Nuestro logo refleja de manera sencilla y memorable el espíritu de UrbanVoice. Buscamos que sea un distintivo fácil de recordar, que transmita la misma seguridad que ofrecemos en cada trayecto.
* **Typography:** La jerarquía tipográfica está dividida funcionalmente:
    * **Lora:** Utilizada para nuestro logotipo y encabezados principales (Headings). Es una fuente serif que refleja un estilo elegante, simple y moderno, promoviendo una atmósfera de innovación y seriedad.
    * **Poppins:** Utilizada para el cuerpo de texto (Body), botones y el resto de la interfaz (UI). Es una fuente sans-serif geométrica que garantiza una alta legibilidad en pantallas móviles y web, facilitando la interacción rápida en momentos de estrés o urgencia.
* **Colors:** Continuando con el objetivo de brindar una imagen que influya principalmente confianza y seguridad, hemos optado por una paleta de colores que transmite calma, estabilidad y profesionalismo.
    * **Primary (Azules Institucionales):** Tonos de azul profundo hasta llegar a variantes más claras o blanco. Esta combinación manifiesta el objetivo de nuestro proyecto y crea una atmósfera de serenidad y sofisticación.
    * **Semantic / Alerts:** Para el mapa y los incidentes, se integran colores funcionales universales: Rojo (Riesgo alto/Denuncias graves), Ámbar (Precaución/Zonas medias) y Verde (Zonas seguras/Acciones exitosas).

---

## 3.1.2. Information Architecture

En nuestra aplicación UrbanVoice, buscamos ofrecer una interfaz interactiva que inspire confianza y seguridad a nuestros usuarios. Teniendo como enfoque principal la seguridad ciudadana del Perú, esta prioridad debe estar presente en cada paso de la experiencia de usuario. Una parte esencial es la correcta administración de la arquitectura de la información, estructurada de la siguiente manera:

> **Página de Inicio (Home / Landing):**
* **Mapa Interactivo:** Sección central que muestra un mapa con los niveles de seguridad en diferentes zonas, permitiendo a los usuarios identificar áreas seguras e inseguras a un solo vistazo.
* **Opciones de Denuncia (CTA):** Enlace y acceso rápido a la funcionalidad de reporte, donde los usuarios pueden registrar crímenes o incidentes de manera pública o anónima.
* **Información sobre la Plataforma:** Detalles institucionales sobre UrbanVoice (misión, visión, impacto esperado), además de enlaces de contacto para consultas y asistencia técnica.

> **Mapa de Seguridad (Core Feature):**
* **Categorías de Riesgo:** División del mapa mediante capas térmicas categorizadas por niveles de seguridad para una rápida identificación de áreas críticas.
* **Filtros de Búsqueda:** Herramientas dinámicas para segmentar el mapa por tipos de incidentes reportados, rangos de fecha/hora y nivel de gravedad.
* **Vista Detallada de Incidentes:** Páginas (o modales emergentes) individuales para cada incidente con descripciones completas, ubicación precisa, hora exacta y opciones para visualizar evidencias adjuntas.

> **Denuncia de Crímenes (Reporting Flow):**
* **Herramienta de Denuncia:** Interfaz intuitiva y guiada paso a paso para reportar incidentes. Permite seleccionar la categoría, adjuntar evidencia multimedia (fotos, videos, audios) y elegir la visibilidad.
* **Vista Previa en Tiempo Real:** Pantalla de confirmación para previsualizar el reporte y validar que los datos y ubicación sean correctos antes de la publicación final.
* **Geolocalización Automática:** Selección asistida de la ubicación del incidente mediante el GPS del dispositivo o marcación manual en el mapa interactivo.

> **Registro y Perfil (User Onboarding):**
* **Registro de Usuarios:** Formulario de fricción mínima para la creación de cuentas (nombre, correo electrónico, número de teléfono y contraseña).
* **Registro de Contactos de Confianza:** Opción vital para que los usuarios vinculen a familiares o amigos con quienes compartirán su ubicación en tiempo real ante situaciones de riesgo.

---

### 3.1.2.1. Organization Systems 

El sistema de organización se centrará en proporcionar la mejor experiencia al usuario en cuanto a la navegación y uso de las funcionalidades en momentos críticos. Nuestra plataforma está diseñada estructuralmente para evitar la sobrecarga cognitiva.

> **Categorización de la Información:**
* **Mapa de Seguridad:** Categorizado visualmente por niveles de riesgo (alto, medio, bajo) y agrupado por clústeres de incidentes.
* **Denuncias y Reportes:** Categorizado por tipología del crimen y nivel de urgencia, facilitando el triage visual y la respuesta rápida de la comunidad.

> **Filtros y Búsqueda:**
* **Filtros en el Mapa:** Permiten a los usuarios refinar la vista temporal y espacialmente.
* **Búsqueda Avanzada:** Barra de búsqueda global para encontrar direcciones específicas, zonas críticas o cruzar variables de información.

> **Interfaz de Usuario Intuitiva:**
* **Menú Principal:** Navegación clara y persistente con acceso a las rutas principales.
* **Submenús Contextuales:** Opciones secundarias que solo aparecen cuando son necesarias.

> **Funcionalidades Específicas:**
* **Información Detallada de Incidentes:** Tarjetas de contenido expansibles que muestran la anatomía completa de un reporte (descripción, validación de la comunidad, ubicación).

---

### 3.1.2.2. Labelling Systems 

Consideramos que la mejor opción para reducir la curva de aprendizaje es a través de un sistema de etiquetado claro, universal y libre de ambigüedades. Utilizaremos etiquetas concisas para describir cada funcionalidad.

Ejemplos de etiquetas clave incluirán:
* **Mapa de zonas de riesgo** 
* **Reportar Incidente** 
* **Detalle del Reporte** 
* **Mi Red de Confianza** 
* **Compartir mi ubicación** 

---

### 3.1.2.3. SEO Tags and Meta Tags 

Nuestros SEO Tags y Meta Tags están optimizados para el posicionamiento orgánico, asegurando que los ciudadanos encuentren la plataforma cuando busquen herramientas de seguridad en el Perú.

> **Landing Page:**
* **Title:** UrbanVoice — Tu ciudad más segura en tiempo real
* **Description:** Descubre UrbanVoice, la red ciudadana que te permite visualizar mapas de riesgo, reportar incidentes y proteger a los tuyos con tu red de confianza.
* **Keywords:** Seguridad ciudadana, Mapa de calor, Incidentes, Policía, Prevención, App de seguridad, Perú.
* **Authors:** UrbanVoice Team

> **Web Application:**
* **Title:** UrbanVoice | Mapa de Seguridad
* **Description:** Plataforma oficial de UrbanVoice. Monitorea alertas geolocalizadas y reportes ciudadanos en tiempo real para planificar rutas seguras.
* **Keywords:** Mapa interactivo, Zonas seguras, Accidentes, Denuncias anónimas, Lima, Seguridad.
* **Authors:** UrbanVoice Team

---

### 3.1.2.4. Searching Systems 

El sistema de búsqueda (Search Engine interno) permitirá a los usuarios encontrar y filtrar información relevante de manera granular, adaptándose a diferentes escenarios de uso:

> **Búsqueda por Incidente:**
* Los usuarios pueden realizar consultas de texto libre como "robos en Miraflores" o "agresiones en San Isidro".
* Se proporcionan operadores de búsqueda avanzada para filtrar de inmediato por fecha, hora, tipo de crimen y nivel de riesgo asociado.

> **Búsqueda por Ubicación :**
* Consultas basadas en puntos de interés  o direcciones exactas, como "incidentes en el centro de Lima".
* Integración de geocodificación para centrar el mapa automáticamente en el distrito o calle buscada.

> **Búsqueda por Nivel de Seguridad:**
* Los usuarios pueden buscar clústeres según su nivel de seguridad, filtrando directamente por "zonas de alto riesgo" o "áreas seguras".
* La plataforma incluye un sistema de sugerencias que recomienda las rutas o zonas más seguras cercanas al usuario.

> **Búsqueda Avanzada :**
* Permite combinar múltiples criterios lógicos; por ejemplo: "Robos" + "Miraflores" + "Durante la noche (20:00 - 06:00)".
* Los resultados se presentan tanto en los pines del mapa como en una vista de lista organizada por relevancia o proximidad.

> **Búsqueda por Fecha y Hora :**
* Deslizadores (Sliders) temporales para buscar incidentes dentro de un rango específico de horas o días.
* Permite identificar patrones, mostrando información sobre la frecuencia y "horas pico" de incidentes en determinadas zonas.

---

### 3.1.2.5. Navigation Systems

El sistema de navegación de PeaceApp está diseñado para proporcionar una experiencia fluida, permitiendo a los usuarios, incluso en situaciones de pánico, encontrar rápidamente lo que necesitan.

> **Menú Principal:**
* Ubicado estratégicamente (barra lateral en web, Tab Bar inferior en móvil) e incluye el imagotipo de la marca. Agrupa los enlaces a las secciones críticas: Mapa, Denuncias, Alertas y Perfil.
* Cada ítem está acompañado de iconografía universal (Material Design/iOS Icons) y etiquetas claras para facilitar el reconocimiento visual sobre la lectura.

> **Navegación Contextual:**
* Dentro de cada módulo, se proporcionan controles contextuales. Por ejemplo, al tocar un incidente en el mapa, se despliega un *Bottom Sheet* (panel inferior) con opciones relacionadas exclusivamente a ese reporte (ver fotos, validar, compartir).

> **Botones de Acción Destacados:**
* En las vistas de Inicio y Mapa, se emplea un Floating Action Button (FAB) prominente, con el color de acento primario o rojo de alerta, destinado a la acción más importante: **Reportar Incidente**.
* Están estratégicamente anclados en la zona de fácil alcance del pulgar para asegurar una interacción rápida.

> **Búsqueda y Filtros Visibles:**
* La barra de búsqueda superior (Search Bar) es persistente y visible en la pantalla del mapa en todo momento.
* Los chips de filtros rápidos se ubican de forma horizontal debajo del buscador, permitiendo activar o desactivar capas de información con un solo toque.

> **Flujo de Navegación Intuitivo :**
* Se sigue una progresión lógica (Lineal y No-Lineal). Desde abrir la app y ver el entorno inmediato, hasta el flujo de denuncia guiado por pasos.
* Se utilizan microinteracciones, *snackbars* (mensajes breves) y confirmaciones visuales ("Reporte enviado con éxito") para mantener al usuario informado sobre el estado del sistema en cada transición.


El Landing Page de UrbanVoice cubre las historias **US13 (Sección informativa)** y **US14 (Formulario de Alianzas)** del Product Backlog. Su objetivo es comunicar el valor de la plataforma a dos audiencias: ciudadanos visitantes que buscan descargar la app y visitantes institucionales (municipios, ONGs, medios) interesados en alianzas. La narrativa se construye en cinco zonas — Hero con CTA de descarga, Trust strip institucional, Features (cuatro pilares), Cómo funciona (tres pasos), Testimonios y CTA final con Footer — siguiendo un arco "promesa → prueba → acción" propio de un landing de conversión.

#### 3.1.3.1. Landing Page Wireframe

El wireframe en baja fidelidad (lo-fi) define la jerarquía estructural del landing antes de aplicar la identidad visual. Se decidieron las proporciones del hero (texto a la izquierda, mockup de app a la derecha), la grilla de features 2×2 para mostrar las cuatro funcionalidades clave (Mapa de riesgo, Reporte ciudadano, Alertas geolocalizadas, Red de confianza), la disposición horizontal de los tres pasos del flujo de uso, y el patrón de tres testimonios en línea. El footer agrupa enlaces en columnas estándar y termina con el CTA dual de descarga (App Store + Google Play).

<p align="center">
  <img src="assets/ui/landing/landing-lofi.png" alt="UrbanVoice Landing Page — Wireframe (Lo-fi)" width="900"/>
</p>

#### 3.1.3.2. Landing Page Mock-up

El mockup en alta fidelidad (hi-fi) materializa el wireframe con la identidad visual completa de UrbanVoice. El hero usa un gradiente azul institucional profundo (`#0A1430` → `#1E40AF`) que evoca seriedad y respaldo cívico, contraste contra el cual la pill "En vivo · 1,247 reportes hoy" con punto rojo pulsante refuerza la sensación de plataforma activa en tiempo real. El mockup de la app a la derecha muestra el heatmap real con pins de incidente y un alert banner, comunicando inmediatamente qué hace el producto. Las cuatro tarjetas bento alternan superficies oscuras institucionales y claras tonales para crear ritmo visual; cada una incorpora un mini-componente de UI extraído de la app (banner de alerta, toggle de anonimato, avatares de la red) como prueba de funcionalidad. Los testimonios incluyen una tarjeta destacada en azul institucional, y el bloque CTA final cierra con descarga + tres tags de confianza (datos cifrados, modo anónimo, sin venta de datos).

<p align="center">
  <img src="assets/ui/landing/landing-hifi.jpeg" alt="UrbanVoice Landing Page — Mock-up (Hi-fi)" width="900"/>
</p>

### 3.1.4. Mobile Applications UX/UI Design

La aplicación móvil cubre el flujo completo del ciudadano y del contacto de confianza para las historias **US01–US10**. Se diseñaron 15 pantallas organizadas en cuatro agrupaciones funcionales: **Onboarding y Autenticación** (Splash, 3 slides de walkthrough, Login, Registro, Recuperación de contraseña), **Núcleo Operativo** (Home con mapa de zonas de riesgo, Crear Reporte con evidencia multimedia, Detalle de Incidente con votación comunitaria), y **Configuración Personal** (Perfil, Edición de Perfil, Configuración de Alertas de Proximidad, Red de Confianza, Notificaciones). Todas las pantallas siguen las pautas de Material/iOS — status bar de 62 px, contenido en wrapper único con padding consistente y, donde aplique, una pill-style Tab Bar de 4 destinos como barra inferior persistente.

#### 3.1.4.1. Mobile Applications Wireframes

Los wireframes en baja fidelidad establecen estructura, jerarquía y zonas táctiles antes de aplicar la identidad visual. Cada pantalla se diseñó con un device frame de 320 × 680 px usando placeholders grises para áreas dinámicas y etiquetas monoespaciadas describiendo cada bloque. Los siguientes son los 15 wireframes agrupados por flujo:

**Onboarding y Autenticación**

<table>
  <tr>
    <td align="center"><img src="assets/ui/mobile-wireframes/01-splash.png" width="180"/><br/><sub>01 · Splash</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/02-onboarding-1.png" width="180"/><br/><sub>02 · Onboarding 1/3</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/03-onboarding-2.png" width="180"/><br/><sub>03 · Onboarding 2/3</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/04-onboarding-3.png" width="180"/><br/><sub>04 · Onboarding 3/3</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/ui/mobile-wireframes/05-login.png" width="180"/><br/><sub>05 · Login</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/06-register.png" width="180"/><br/><sub>06 · Registro</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/07-recover.png" width="180"/><br/><sub>07 · Recuperar contraseña</sub></td>
    <td align="center"></td>
  </tr>
</table>

**Núcleo Operativo**

<table>
  <tr>
    <td align="center"><img src="assets/ui/mobile-wireframes/08-home-map.png" width="180"/><br/><sub>08 · Home (Mapa de riesgo)</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/09-create-report.png" width="180"/><br/><sub>09 · Crear Reporte</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/10-incident-detail.png" width="180"/><br/><sub>10 · Detalle de Incidente</sub></td>
  </tr>
</table>

**Configuración Personal**

<table>
  <tr>
    <td align="center"><img src="assets/ui/mobile-wireframes/11-profile.png" width="180"/><br/><sub>11 · Perfil</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/12-edit-profile.png" width="180"/><br/><sub>12 · Editar Perfil</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/13-alerts-config.png" width="180"/><br/><sub>13 · Configurar Alertas</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/14-trust-network.png" width="180"/><br/><sub>14 · Red de Confianza</sub></td>
    <td align="center"><img src="assets/ui/mobile-wireframes/15-notifications.png" width="180"/><br/><sub>15 · Notificaciones</sub></td>
  </tr>
</table>

**Mock-ups en alta fidelidad**

A continuación se presentan las mismas 15 pantallas con la identidad visual completa aplicada (azul institucional, escala de alertas, tipografía Geist/Inter y componentes finales). Los mock-ups muestran detalles que en lo-fi quedan abstractos: el heatmap simulado en el Home con capas radiales de gradiente rojo/ámbar superpuestas a la cuadrícula vial, los pins diferenciados por color según tipo de incidente, el alert banner rojo de proximidad con micro-tipografía y la barra de votos comunitarios en el detalle de incidente.

<table>
  <tr>
    <td align="center"><img src="assets/ui/mobile-mockups/01-splash.png" width="180"/><br/><sub>01 · Splash</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/02-onboarding-1.png" width="180"/><br/><sub>02 · Onboarding 1/3</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/03-onboarding-2.png" width="180"/><br/><sub>03 · Onboarding 2/3</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/04-onboarding-3.png" width="180"/><br/><sub>04 · Onboarding 3/3</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/ui/mobile-mockups/05-login.png" width="180"/><br/><sub>05 · Login</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/06-register.png" width="180"/><br/><sub>06 · Registro</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/07-recover.png" width="180"/><br/><sub>07 · Recuperar contraseña</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/08-home-map.png" width="180"/><br/><sub>08 · Home (Mapa)</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/ui/mobile-mockups/09-create-report.png" width="180"/><br/><sub>09 · Crear Reporte</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/10-incident-detail.png" width="180"/><br/><sub>10 · Detalle Incidente</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/11-profile.png" width="180"/><br/><sub>11 · Perfil</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/12-edit-profile.png" width="180"/><br/><sub>12 · Editar Perfil</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/ui/mobile-mockups/13-alerts-config.png" width="180"/><br/><sub>13 · Config. Alertas</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/14-trust-network.png" width="180"/><br/><sub>14 · Red de Confianza</sub></td>
    <td align="center"><img src="assets/ui/mobile-mockups/15-notifications.png" width="180"/><br/><sub>15 · Notificaciones</sub></td>
    <td align="center"></td>
  </tr>
</table>

#### 3.1.4.2. Mobile Applications Wireflow Diagrams

Los Wireflow Diagrams documentan los cuatro flujos críticos de UrbanVoice mostrando la secuencia de pantallas que el usuario recorre, con anotaciones sobre los gestos o eventos que disparan cada transición (tap en FAB, submit de formulario, push notification, etc.). Cada nodo es una mini-representación de la pantalla involucrada y las flechas se codifican por color según el tipo de flujo: azul institucional para alta neutral, rojo para reporte de incidente, ámbar para alertas y verde para confirmaciones de configuración.

**Flow 1 — Registro → Onboarding → Home**

El nuevo ciudadano descarga la app, completa su registro, recorre el walkthrough de tres slides, otorga el permiso de ubicación y aterriza en el mapa de su zona. El flujo prioriza fricción mínima (registro de tres campos) y educación visual antes de pedir permisos sensibles.

<p align="center">
  <img src="assets/ui/wireflows/flow-1-registro-onboarding-home.png" alt="Flow 1 · Registro → Onboarding → Home" width="900"/>
</p>

**Flow 2 — Home → Reportar incidente → Confirmación**

Cubre la historia US02 (Registro de incidente) y US03 (Evidencia multimedia). El ciudadano detecta un incidente, abre el formulario desde el FAB rojo del mapa, selecciona tipo, adjunta evidencia (foto/audio/video), confirma el modo anónimo (US04) y publica. El sistema valida la evidencia, encripta y muestra confirmación con CTA de "ver en mapa".

<p align="center">
  <img src="assets/ui/wireflows/flow-2-home-reportar-confirmacion.png" alt="Flow 2 · Home → Reportar → Confirmación" width="900"/>
</p>

**Flow 3 — Notificación de alerta → Detalle → Compartir con red**

Cubre la historia US05 (Alertas geolocalizadas) y US07 (Compartir ubicación). El sistema detecta proximidad a un incidente reportado y emite push notification visible incluso desde lockscreen. Al abrirla, el ciudadano accede al detalle completo (mini-mapa, evidencia, votos comunitarios) y puede compartir la información y su ubicación con uno o varios contactos de su red de confianza.

<p align="center">
  <img src="assets/ui/wireflows/flow-3-alerta-detalle-compartir.png" alt="Flow 3 · Alerta → Detalle → Compartir" width="900"/>
</p>

**Flow 4 — Perfil → Configurar alertas → Guardar**

Cubre la configuración granular de US05. Desde su perfil el usuario accede a la configuración de alertas, ajusta el radio de proximidad mediante slider visual (100m–2km), activa/desactiva tipos de incidente que le interesan (robos, acoso, vehículos sospechosos, emergencias) y guarda. La pantalla de éxito confirma la configuración aplicada y devuelve al perfil.

<p align="center">
  <img src="assets/ui/wireflows/flow-4-perfil-alertas-guardar.png" alt="Flow 4 · Perfil → Alertas → Guardar" width="900"/>
</p>

<br>

#### 3.1.4.3. Mobile Applications Mock-ups

<table>
  <tr>
    <td align="center"><img src="assets/mockups/01._splash_screen.png" width="180"/><br/><sub>01 · Splash</sub></td>
    <td align="center"><img src="assets/mockups/02._onboarding_1_3.png" width="180"/><br/><sub>02 · Onboarding 1/3</sub></td>
    <td align="center"><img src="assets/mockups/03._onboarding_2_3.png" width="180"/><br/><sub>03 · Onboarding 2/3</sub></td>
    <td align="center"><img src="assets/mockups/04._onboarding_3_3.png" width="180"/><br/><sub>04 · Onboarding 3/3</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/mockups/05._login.png" width="180"/><br/><sub>05 · Login</sub></td>
    <td align="center"><img src="assets/mockups/06._registro.png" width="180"/><br/><sub>06 · Registro</sub></td>
    <td align="center"><img src="assets/mockups/07._recuperar_contrase_a.png" width="180"/><br/><sub>07 · Recuperar contraseña</sub></td>
    <td align="center"><img src="assets/mockups/08._home_mapa_de_riesgo.png" width="180"/><br/><sub>08 · Home (Mapa de riesgo)</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/mockups/09._crear_reporte_de_incidente.png" width="180"/><br/><sub>09 · Crear Reporte</sub></td>
    <td align="center"><img src="assets/mockups/10._detalle_de_incidente.png" width="180"/><br/><sub>10 · Detalle de Incidente</sub></td>
    <td align="center"><img src="assets/mockups/11._perfil.png" width="180"/><br/><sub>11 · Perfil</sub></td>
    <td align="center"><img src="assets/mockups/12._editar_perfil.png" width="180"/><br/><sub>12 · Editar Perfil</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="assets/mockups/13._configurar_alertas.png" width="180"/><br/><sub>13 · Config. Alertas</sub></td>
    <td align="center"><img src="assets/mockups/14._red_de_confianza.png" width="180"/><br/><sub>14 · Red de Confianza</sub></td>
    <td align="center"><img src="assets/mockups/15._notificaciones.png" width="180"/><br/><sub>15 · Notificaciones</sub></td>
    <td align="center"></td>
  </tr>
</table>

#### 3.1.4.4. Mobile Applications User Flow Diagrams 

Los siguientes User Flow Diagrams representan la secuencia lógica de acciones y decisiones que realizan los usuarios dentro de UrbanVoice. A diferencia de los wireflows, estos diagramas modelan el comportamiento funcional del sistema y su trazabilidad con las User Stories definidas en el Product Backlog. Cada flujo cubre funcionalidades críticas del producto y permite validar la coherencia entre requisitos, backlog y desarrollo iterativo.

##### Flow 1 — Registro y acceso inicial

<img src="assets/flows/Flow-1.png"/><br/>

##### Flow 2 — Consultar mapa y rutas seguras
<img src="assets/flows/Flow-2.png"/><br/>


##### Flow 3 — Registrar incidente
<img src="assets/flows/Flow-3.png"/><br/>


##### Flow 4 — Recibir alertas
<img src="assets/flows/Flow-4.png"/><br/>


##### Flow 5 — Compartir ubicación
<img src="assets/flows/Flow-5.png"/><br/>


##### Flow 6 — Moderación de incidentes
<img src="assets/flows/Flow-6.png"/><br/>



#### 3.1.4.5. Mobile Applications Prototyping 

El prototipo de la aplicación móvil de UrbanVoice fue desarrollado a partir de las pantallas diseñadas previamente. Su propósito es mostrar cómo sería la navegación principal de la aplicación antes de iniciar la implementación.

<img src="assets/Prototipo.png"/><br/>

Enlace del prototipo: [[UrbanVoice](https://stitch.withgoogle.com/preview/14344472304506913570?node-id=41b9a44fbe08432b91e33a1f16d047ba)]

# Capítulo IV: Product Implementation & Validation

## 4. Product Implementation & Validation

### 4.1. Software Configuration Management

A continuación, presentaremos el proceso por el cual organizamos, gestionamos y controlamos los cambios en el desarrollo de este proyecto.

#### 4.1.1. Software Development Environment Configuration

**Requirements Management**

1. **Trello:** Es una herramienta utilizada para gestionar el flujo de trabajo de proyectos principalmente basados en marcos de trabajo ágiles. Será empleado para visualizar y actualizar el estado actual de las tareas e historias de usuario pertenecientes al sprint a desarrollar.  
   Ruta de referencia: https://trello.com/es

**Product UX/UI Design**

1. **Figma:** Plataforma de elaboración de prototipos y edición gráfica, principalmente utilizada para el diseño digital. En el caso del proyecto, será utilizada para el prototipado de la aplicación móvil UrbanVoice y sus versiones de wireframes y mockups.  
   Ruta de referencia: https://www.figma.com/login

2. **Miro:** Herramienta colaborativa de pizarra digital empleada para el modelado del EventStorming, Domain Message Flows y Bounded Context Canvases del diseño estratégico del sistema.  
   Ruta de referencia: https://miro.com/

**Software Development**

1. **Android Studio:** Entorno de desarrollo integrado oficial para el desarrollo de aplicaciones Android nativas. Será empleado para la construcción de la aplicación móvil de UrbanVoice en Kotlin.  
   Ruta de referencia: https://developer.android.com/studio

2. **IntelliJ IDEA / Spring Boot:** Framework de desarrollo backend basado en Java. Se utilizará para construir los servicios RESTful que soportan la lógica de negocio de los bounded contexts definidos en el diseño táctico.  
   Ruta de referencia: https://spring.io/projects/spring-boot

3. **Kotlin:** Lenguaje de programación moderno para Android, utilizado para el desarrollo de la aplicación móvil nativa.  
   Ruta de referencia: https://kotlinlang.org/

4. **Java:** Lenguaje de programación principal para el desarrollo del backend con Spring Boot.  
   Ruta de referencia: https://www.java.com/

5. **PostgreSQL:** Sistema de gestión de bases de datos relacional utilizado para la persistencia de los datos de cada bounded context bajo el principio de database-per-service.  
   Ruta de referencia: https://www.postgresql.org/

6. **Git:** Herramienta de control de versiones que facilita el registro y la gestión de las distintas versiones del programa. Su propósito es mantener un historial de cambios y simplificar la corrección de errores.  
   Ruta de referencia: https://git-scm.com/

**Software Documentation and Project Management**

7. **GitHub:** Plataforma en la nube que hospedará los repositorios de código del proyecto. Permitirá la colaboración en tiempo real y la revisión de contribuciones de cada miembro del equipo.  
   Ruta de referencia: https://github.com/

**Software Deployment**

1. **GitHub Pages:** Servicio de alojamiento web estático utilizado para publicar el Landing Page de UrbanVoice directamente desde el repositorio de GitHub.  
   Ruta de referencia: https://pages.github.com/

2. **Firebase App Distribution:** Plataforma de distribución de aplicaciones móviles de Google, utilizada para compartir builds de la app UrbanVoice en formato `.apk` con testers y usuarios de validación.  
   Ruta de referencia: https://firebase.google.com/products/app-distribution

---

#### 4.1.2. Source Code Management

El proyecto seguirá las convenciones del flujo de trabajo establecido por el modelo **GitFlow** para el control de versiones, empleando GitHub como plataforma y sistema de control de versiones.

**Repositorios de GitHub:**

- **Organización:** https://github.com/urbanvoice-3248-dispo-moviles
- **Repositorio del Reporte:** https://github.com/urbanvoice-3248-dispo-moviles/UrbanVoice
- **Repositorio del Landing Page:** https://github.com/urbanvoice-3248-dispo-moviles/Landing-Page
- **Repositorio del Backend:** https://github.com/urbanvoice-3248-dispo-moviles/Backend-UrbanVoice
<!-- - **Repositorio de la App Móvil:** -->

**Flujo de trabajo GitFlow**

El flujo de trabajo implementado para el desarrollo del proyecto se basará en el modelo propuesto por Vincent Driessen en *"A successful Git branching model"*.

**Estructura de branches (Ramas):**

1. **Main branch (Rama principal):** Esta rama servirá como la principal para la aplicación, alojando versiones estables y finales del desarrollo. Únicamente se aceptarán cambios que hayan sido previamente probados y verificados en las ramas de feature y develop.

2. **Develop branch (Rama de desarrollo):** El propósito de esta rama es facilitar los avances del proyecto en equipo y mantener los archivos centrales del desarrollo continuo.

3. **Feature branch (Ramas de funcionalidad):** Cada funcionalidad o bounded context desarrollado por el equipo tendrá su propia rama. Una vez que una funcionalidad esté completamente trabajada, se fusionará con la rama de desarrollo del proyecto. Las convenciones para nombrar las ramas de funcionalidad seguirán un patrón descriptivo y único, por ejemplo, `feature/notification-management` o `feature/report-module`.

4. **Convenciones de Ramas (GitFlow):**
  * **Main:** Versiones estables para producción (v1.0.0).
  * **Develop:** Integración de nuevas funcionalidades.
  * **Feature:** `feature/US-ID-descripcion` (Ej. `feature/US02-registro-incidente`).
  * **Fix:** `hotfix/descripcion-error` para correcciones críticas en Main.

#### 4.1.3. Source Code Style Guide & Conventions

**Kotlin (Android)**

Algunas de las prácticas que deben seguirse para alcanzar un código coherente, sostenible y ordenado son las siguientes:

1. Utilizar nombres de variables y funciones en **camelCase** y clases en **PascalCase**.
2. Declarar las propiedades inmutables con `val` y solo usar `var` cuando sea estrictamente necesario.
3. Preferir funciones de extensión para mejorar la legibilidad del código.
4. Seguir las convenciones de paquetes por capas: `data`, `domain`, `presentation`, `ui`.
5. Utilizar comentarios descriptivos en funciones complejas y documentar con KDoc las interfaces públicas.
6. Mantener las funciones cortas y con una única responsabilidad.

Referencia: [Kotlin Coding Conventions](https://kotlinlang.org/docs/coding-conventions.html)

**Java / Spring Boot (Backend)**

Entre las prácticas empleadas se mencionan:

1. Seguir la convención de nombres estándar de Java: clases en **PascalCase**, métodos y variables en **camelCase**, constantes en **UPPER_SNAKE_CASE**.
2. Organizar el código por bounded contexts con paquetes que reflejen las cuatro capas del DDD: `domain`, `application`, `infrastructure`, `interfaces`.
3. Documentar las interfaces y clases públicas con Javadoc.
4. Usar anotaciones de Spring de forma explícita: `@Service`, `@Repository`, `@Component`, `@RestController`.
5. Mantener los controllers delgados (thin controllers): solo reciben el request y delegan en el Application Layer.
6. Escribir pruebas unitarias para los Command Handlers y Domain Services.

Referencia: [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)

**SQL / PostgreSQL**

1. Nombrar las tablas en **snake_case** y en plural (ej. `security_alerts`, `reports`).
2. Usar `UUID` como tipo de dato para las claves primarias.
3. Definir restricciones `CHECK` para columnas con valores acotados.
4. Crear índices sobre columnas de búsqueda frecuente (`author_id`, `status`, `recipient_id`).
5. Documentar cada tabla con comentarios en el script de creación.

**HTML / CSS (Landing Page)**

1. Cerrar todos los elementos HTML correctamente.
2. Declarar el tipo de documento `<!DOCTYPE html>` en la primera línea.
3. Utilizar clases semánticas y significativas en CSS.
4. Mantener el código en minúsculas y con sangría de 2 espacios.
5. Eliminar espacios en blanco innecesarios y mantener comentarios explicativos.

Referencia: [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)

---

#### 4.1.4. Software Deployment Configuration

**Landing Page Deployment**

El Landing Page del proyecto será desplegado utilizando **GitHub Pages**, lo que permite alojar el sitio web de manera gratuita directamente desde el repositorio de GitHub, configurando la rama `main` como fuente de publicación.

**Backend Deployment**

El backend desarrollado en Spring Boot será desplegado en un entorno cloud. Se utilizará **Railway** o **Render** como plataforma de hosting, conectado a una instancia de **PostgreSQL** como base de datos principal. Cada bounded context mantendrá su propia base de datos bajo el principio de database-per-service.

**Mobile Application Deployment**

La aplicación móvil Android será distribuida durante las fases de validación a través de **Firebase App Distribution**, permitiendo a los testers descargar el `.apk` directamente. Para producción, se publicará en **Google Play Store**.

---

### 4.2. Landing Page & Mobile Application Implementation

#### 4.2.1. Sprint 1

##### 4.2.1.1. Sprint Planning 1

Para este primer sprint el equipo se enfocará en la construcción de la base del proyecto UrbanVoice: el Landing Page informativo completo, la arquitectura inicial del backend y los módulos de autenticación e incidentes. Se implementarán los endpoints REST de incidentes, la autenticación JWT y la infraestructura CI/CD como base para soportar las funcionalidades principales que serán completadas en los siguientes sprints.

| Sprint # | Sprint 1 |
|---|---|
| **Sprint Planning Background** | |
| **Date** | 22/04/2026 |
| **Time** | 07:00 PM |
| **Location** | Servidor de Discord del Equipo |
| **Prepared By** | Billy Jake Ruiz Madrid |
| **Attendees (to planning meeting)** | Ivan La Madrid / Jeremy Quijada / Billy Ruiz / Santiago Gordillo / Giorgio Awad |
| **Sprint 1 Review Summary** | En esta primera sesión se definió la base estructural del proyecto UrbanVoice, incluyendo el Landing Page completo, registro e inicio de sesión de usuarios, el módulo de visualización y registro de incidentes en el mapa, y la arquitectura base del backend con autenticación JWT. |
| **Sprint 1 Retrospective Summary** | El equipo acordó priorizar la estabilidad de la arquitectura DDD, completar la Landing Page al 100% y alcanzar un 70% del backend con los endpoints críticos de incidentes y autenticación para permitir la escalabilidad funcional en los siguientes sprints. |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | Desarrollar y desplegar el Landing Page de UrbanVoice al 100%, implementar el flujo completo de registro e inicio de sesión, construir el módulo de incidentes (visualización en mapa, registro y adjunto de evidencia), e iniciar la infraestructura backend con autenticación JWT, API REST de incidentes y pipeline CI/CD. El éxito se logrará cuando un ciudadano pueda registrarse, iniciar sesión, visualizar el mapa de incidentes y reportar un nuevo incidente con evidencia multimedia. |
| **Sprint 1 Velocity** | 44 Velocity |
| **Sum of Story Points** | 44 Story Points |

---

##### 4.2.1.2. Sprint Backlog 1

| # Orden | User Story ID | Título | Descripción | Story Points | Estimation (hours) | Assigned To | Status |
|:---:|:---:|---|---|:---:|:---:|---|:---:|
| 1 | US01 | Registrarse en la plataforma | Como visitante, quiero registrarme en UrbanVoice proporcionando mis datos básicos para acceder a las funcionalidades de la plataforma. | 3 | 5 | Billy Ruiz | Done |
| 2 | US02 | Iniciar sesión en la plataforma | Como ciudadano registrado, quiero iniciar sesión con mis credenciales para acceder a las funcionalidades de UrbanVoice. | 3 | 5 | Billy Ruiz | Done |
| 3 | US04 | Visualizar mapa de incidentes | Como ciudadano, quiero visualizar un mapa con los incidentes reportados cerca de mi ubicación para estar informado sobre la situación de seguridad en mi zona. | 5 | 8 | Ivan La Madrid | In Progress |
| 4 | US05 | Registrar incidente en el mapa | Como ciudadano, quiero registrar un incidente de inseguridad seleccionando su ubicación en el mapa para alertar a otros usuarios. | 5 | 8 | Ivan La Madrid | In Progress |
| 5 | US06 | Adjuntar evidencia multimedia al reporte | Como ciudadano, quiero adjuntar fotos o videos al reporte de incidente para proporcionar evidencia visual del suceso. | 5 | 8 | Giorgio Awad | In Progress |
| 6 | US08 | Explorar landing page informativa | Como visitante, quiero explorar la landing page de UrbanVoice para conocer las funcionalidades y beneficios de la plataforma. | 1 | 2 | Santiago Gordillo | Done |
| 7 | US09 | Registrar solicitud de alianza institucional | Como visitante institucional, quiero enviar una solicitud de contacto desde la landing page para proponer alianzas con UrbanVoice. | 3 | 4 | Jeremy Quijada | Done |
| 8 | US10 | Consultar información de contacto y redes sociales | Como visitante, quiero consultar la información de contacto y redes sociales de UrbanVoice para seguir la plataforma. | 1 | 2 | Santiago Gordillo | Done |
| 9 | TS01 | Configurar infraestructura cloud y pipeline CI/CD | Como developer, quiero configurar la infraestructura en la nube y el pipeline de integración continua para automatizar el despliegue del backend. | 5 | 8 | Ivan La Madrid | In Progress |
| 10 | TS02 | Implementar autenticación JWT en el backend | Como developer, quiero implementar autenticación basada en tokens JWT en el backend para asegurar los endpoints de la API. | 5 | 8 | Giorgio Awad | In Progress |
| 11 | TS03 | Implementar API REST de incidentes | Como developer, quiero implementar los endpoints REST para el módulo de incidentes (CRUD y consultas geolocalizadas). | 8 | 12 | Ivan La Madrid | In Progress |

##### 4.2.1.3. Development Evidence for Sprint Review 

Durante este Sprint, se lograron avances significativos en la implementación de la landing page UrbanVoice, destacando la creación del frontend usando HTML, un diseño responsivo y estilizado con CSS, y la incorporación de funcionalidades dinámicas mediante JavaScript. Realizado en el periado de 11 de Abril al 11 de Mayo.

| Repository | Branch | CommitID | Commit Message | Commit On |
|------------|--------|----------|----------------|-----------|
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 9b667eb | Add mobile applications prototyping | 09/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | b6478a2 | Add files via upload | 09/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | f19c5d6 | Add mobile applications user flow diagrams | 09/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | f5e2f49 | Update mockup image filenames | 09/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 54be945 | Add mobile applications mock-ups section | 09/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 81ebbfa | Add files via upload | 09/05/2026 |
| BillyJakeRuizMadrid/urbanvoice-3248-dispo-moviles | main | 1ec89c8 | docs(chapter4): add sprint 1. | 08/05/2026 |
| SantiagoGR14/urbanvoice-3248-dispo-moviles | main | f324044 | Refine descriptions in README for clarity | 07/05/2026 |
| SantiagoGR14/urbanvoice-3248-dispo-moviles | main | 7a04155 | Update README with style guidelines and architecture | 07/05/2026 |
| GiorgioAwad/urbanvoice-3248-dispo-moviles | main | 696a122 | Capitulo III: Landing Page UI Design, Wirefram, mock-up, UX/UI design, wireframes, wireflow diagrams | 06/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | e0a6a7a | Merge pull request #6 feat/-correcciones-avance-1 | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | 1b72c54 | fix: 5w 2 h | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | a933bc5 | Merge pull request #5 feat/-correcciones-avance-1 | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | 576fa1f | fix: Corrigiendo user stories / product backlog | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | c86cc51 | On Avance-1: !!GitHub_Desktop<Avance-1> | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | 0dad32e | index on Avance-1: 731120d feat/ Location-managment | 05/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 23cd78e | Revise spike stories for clarity and focus | 04/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 800c489 | Remove prioritization section for Spike Stories | 04/05/2026 |
| IvanLaMadrid/urbanvoice-3248-dispo-moviles | main | 0cce7b6 | Add Spike Stories for UrbanVoice development | 04/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | 0671e4c | Merge pull request #4 Avance-1 | 20/04/2026 |

##### 4.2.1.4. Testing Suite Evidence for Sprint Review 
En este Sprint se implementaron pruebas automatizadas bajo el enfoque BDD (Behavior Driven Development), elaborando archivos .feature en lenguaje Gherkin y sus correspondientes archivos Steps en el lenguaje de programación del proyecto.

**Feature:**
<img src="assets/Features.png"/><br/>

**Steps:**
<img src="assets/Steps.png"/><br/>

| Repository | Branch | CommitID | Commit Message | Commit On |
|------------|--------|----------|----------------|-----------|
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | a933bc5 | feat: Version Final | 11/05/2026 | 05/05/2026 |
| JeremyQuijadaMagro/urbanvoice-3248-dispo-moviles | main | 576fa1f | feat: Steps and Feature | 11/05/2026 |

##### 4.2.1.5. Execution Evidence for Sprint Review 

En este sprint, la Landing Page logró cubrir de manera completa las funcionalidades básicas de navegación, búsqueda y presentación de información, cumpliendo con los criterios definidos en el backlog. Además, se avanzo con el backend a un 70% de la funcionalidad requerida, lo que permitió obtener un gran avance en la implementación de los endpoints.

###### Capturas de la Landing Page:

**Presentacion:**
<img src="assets/LandingPage-1.png"/><br/>

**Funcionalidades:**
<img src="assets/LandingPage-2.png"/><br/>

**Footer:**
<img src="assets/LandingPage-3.png"/><br/>

###### Capturas del backend:

<img src="assets/BackEnd.png"/><br/>

##### 4.2.1.6. Services Documentation Evidence for Sprint Review 

En este Sprint se consolidó la documentación de Web Services mediante OpenAPI/Swagger UI, asegurando que cada módulo tenga sus endpoints descritos con acciones, parámetros y ejemplos de respuesta. Esto facilita la validación de servicios RESTful y la trazabilidad de cambios en el repositorio. 

##  Locations  
API para gestionar ubicaciones y zonas de riesgo.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener todas las ubicaciones | GET | `/api/v1/locations` | Ninguno | `[{"id":1,"name":"Parque Central","district":"Surco"}]` |
| Crear nueva ubicación | POST | `/api/v1/locations` | Body: `{ "name":"Plaza Norte","district":"Independencia" }` | `{ "id":2,"name":"Plaza Norte","district":"Independencia" }` |
| Obtener ubicación por ID | GET | `/api/v1/locations/{id}` | Path: `id` | `{ "id":1,"name":"Parque Central","district":"Surco" }` |
| Eliminar ubicación | DELETE | `/api/v1/locations/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Obtener ubicaciones cercanas | GET | `/api/v1/locations/nearby` | Query: `lat,long` | `[{"id":3,"name":"Plaza Mayor"}]` |
| Obtener ubicaciones por distrito | GET | `/api/v1/locations/district/{district}` | Path: `district` | `[{"id":4,"name":"Plaza Norte"}]` |
| Obtener ubicaciones peligrosas | GET | `/api/v1/locations/dangerous` | Ninguno | `[{"id":5,"name":"Zona Roja"}]` |

---

##  User Profiles  
API para gestionar perfiles de usuario.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener perfil por ID | GET | `/api/v1/profiles/{id}` | Path: `id` | `{ "id":5,"email":"user@mail.com" }` |
| Actualizar perfil | PUT | `/api/v1/profiles/{id}` | Path: `id`, Body: `{ "email":"new@mail.com" }` | `{ "id":5,"email":"new@mail.com","status":"updated" }` |
| Eliminar perfil | DELETE | `/api/v1/profiles/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Crear nuevo perfil | POST | `/api/v1/profiles` | Body: `{ "email":"user@mail.com","name":"Juan" }` | `{ "id":6,"status":"created" }` |
| Obtener perfil por email | GET | `/api/v1/profiles/email/{email}` | Path: `email` | `{ "id":6,"email":"user@mail.com" }` |

---

##  Incident Reports  
API para gestionar reportes de incidentes.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener reporte por ID | GET | `/api/v1/reports/{id}` | Path: `id` | `{ "id":10,"description":"Accidente en Av. Primavera" }` |
| Actualizar reporte | PUT | `/api/v1/reports/{id}` | Path: `id`, Body: `{ "description":"Actualización del reporte" }` | `{ "id":10,"status":"updated" }` |
| Eliminar reporte | DELETE | `/api/v1/reports/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Crear nuevo reporte | POST | `/api/v1/reports` | Body: `{ "userId":5,"description":"Accidente en Av. Primavera" }` | `{ "id":10,"status":"created" }` |
| Obtener reportes de un usuario | GET | `/api/v1/reports/user/{userId}` | Path: `userId` | `[{"id":11,"description":"Caída en Av. Benavides"}]` |
| Obtener reportes cercanos | GET | `/api/v1/reports/nearby` | Query: `lat,long` | `[{"id":12,"description":"Incidente en Parque Kennedy"}]` |

---

##  Alerts  
API para gestionar alertas y notificaciones.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener todas las alertas | GET | `/api/v1/alerts` | Ninguno | `[{"id":1,"message":"Zona peligrosa detectada"}]` |
| Crear nueva alerta | POST | `/api/v1/alerts` | Body: `{ "message":"Nueva alerta" }` | `{ "id":2,"status":"created" }` |
| Eliminar todas las alertas | DELETE | `/api/v1/alerts` | Ninguno | `{ "status":"deleted_all" }` |
| Obtener alerta por ID | GET | `/api/v1/alerts/{id}` | Path: `id` | `{ "id":2,"message":"Nueva alerta" }` |
| Eliminar alerta por ID | DELETE | `/api/v1/alerts/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Obtener alertas por usuario | GET | `/api/v1/alerts/user/{userId}` | Path: `userId` | `[{"id":3,"message":"Alerta personalizada"}]` |


##### 4.2.1.7. Software Deployment Evidence for Sprint Review 
En este Sprint se realizó el despliegue inicial de un producto digital: una Landing Page. El despliegue se efectuó mediante GitHub Pages, aprovechando la infraestructura gratuita de GitHub para alojar sitios estáticos.
Este proceso la activación de GitHub Pages y la verificación del resultado.

**Paso 1:** Estar en el repositorio de la Landing Page e ir a Settings 

<img src="assets/Paso1.png"/><br/>

**Paso 2:** Ir a Pages

<img src="assets/Paso2.png"/><br/>

**Paso 3:** Seleccionar rama main y carpeta /root
y guardar informacion

<img src="assets/Paso3.png"/><br/>

**Paso 4:** Verificar despliegue público

<img src="assets/despliegue landing.png"/><br/>

Acceder al enlace https://urbanvoice-3248-dispo-moviles.github.io/Landing-Page/

##### 4.2.1.8. Team Collaboration Insights during Sprint 
Para este Sprint, las tareas de diseño, implementación y documentación de la landing page se distribuyeron entre los integrantes del equipo. La implementación y despliegue de la landing page fue llevado a cabo por todo el equipo, siguiendo un enfoque colaborativo que involucró diversas etapas bien definidas. Además del desarrollo del backend.

<img src="assets/Evidence Sprint Review.png"/><br/>

<img src="assets/Network.png"/><br/>

Las actividades de implementación se desarrollaron mediante un flujo de trabajo ágil. El proceso comenzó con la planificación inicial, donde se asignaron roles específicos para cada fase. Esto incluyó el diseño de la estructura HTML y los estilos CSS, que se iniciaron con commits iniciales para establecer la base del proyecto.

#### 4.2.2. Sprint 2

##### 4.2.2.1. Sprint Planning 2

Para este segundo sprint el equipo se enfocará en completar el núcleo funcional de UrbanVoice. Se finalizarán los módulos de autenticación, incidentes y geolocalización iniciados en el sprint anterior, además de implementar las funcionalidades de alertas, compartición de ubicación en tiempo real, monitoreo entre contactos, panel de administración (moderación y categorías), heatmap de zonas de riesgo e integración de Google Maps SDK en las apps móviles.

| Sprint # | Sprint 2 |
|---|---|
| **Sprint Planning Background** | |
| **Date** | 06/05/2026 |
| **Time** | 07:00 PM |
| **Location** | Servidor de Discord del Equipo |
| **Prepared By** | Billy Jake Ruiz Madrid |
| **Attendees (to planning meeting)** | Ivan La Madrid / Jeremy Quijada / Billy Ruiz / Santiago Gordillo / Giorgio Awad |
| **Sprint 2 Review Summary** | En esta sesión se priorizó la implementación de las funcionalidades core del sistema, centradas en geolocalización, reportes ciudadanos, visualización del mapa de riesgo, alertas de proximidad, compartición de ubicación y el panel de administración para moderación de reportes. |
| **Sprint 2 Retrospective Summary** | El equipo decidió completar el backend al 100% y habilitar las apps Android y Flutter con funcionalidades de mapa, reportes, alertas y geolocalización para asegurar la disponibilidad de la plataforma en los principales frentes móviles. |
| **Sprint Goal & User Stories** | |
| **Sprint 2 Goal** | Completar el backend de UrbanVoice al 100%, implementar las funcionalidades de alertas geolocalizadas, compartición de ubicación en tiempo real, monitoreo entre contactos, panel de administración (moderación y categorías), heatmap de zonas de riesgo y la integración con Google Maps SDK en Android y Flutter. El éxito se logrará cuando un ciudadano pueda recibir notificaciones de incidentes cercanos, compartir su ubicación en tiempo real, y un administrador pueda moderar reportes y gestionar categorías. |
| **Sprint 2 Velocity** | 63 Velocity |
| **Sum of Story Points** | 63 Story Points |

---

##### 4.2.2.2. Sprint Backlog 2

| # Orden | User Story ID | Título | Descripción | Story Points | Estimation (hours) | Assigned To | Status |
|:---:|:---:|---|---|:---:|:---:|---|:---:|
| 1 | US03 | Recuperar contraseña olvidada | Como ciudadano, quiero recuperar mi contraseña mediante mi correo electrónico para restablecer el acceso a mi cuenta. | 2 | 3 | Billy Ruiz | Done |
| 2 | US07 | Visualizar detalle de un incidente | Como ciudadano, quiero ver el detalle de un incidente específico para conocer tipo, fecha, descripción y evidencia disponible. | 2 | 3 | Santiago Gordillo | Done |
| 3 | US11 | Realizar reporte anónimo | Como ciudadano, quiero realizar un reporte de incidente de forma anónima para proteger mi identidad mientras contribuyo a la seguridad ciudadana. | 3 | 4 | Giorgio Awad | Done |
| 4 | US12 | Filtrar incidentes por tipo y fecha | Como ciudadano, quiero filtrar los incidentes en el mapa por tipo y rango de fechas para enfocarme en la información relevante. | 3 | 4 | Santiago Gordillo | Done |
| 5 | US13 | Moderar reportes ciudadanos | Como administrador, quiero moderar los reportes de incidentes para aprobar o rechazar contenido inapropiado o falso. | 5 | 8 | Jeremy Quijada | Done |
| 6 | US14 | Gestionar categorías de incidentes | Como administrador, quiero gestionar las categorías de incidentes (crear, editar, desactivar) para mantener actualizada la taxonomía de reportes. | 3 | 4 | Jeremy Quijada | Done |
| 7 | US15 | Recibir notificaciones de incidentes cercanos | Como ciudadano, quiero recibir notificaciones push cuando ocurra un incidente cerca de mi ubicación para tomar precauciones inmediatas. | 8 | 12 | Billy Ruiz | In Progress |
| 8 | US16 | Compartir ubicación en tiempo real | Como ciudadano, quiero compartir mi ubicación en tiempo real con contactos de confianza para que puedan monitorear mi desplazamiento. | 8 | 12 | Ivan La Madrid | In Progress |
| 9 | US17 | Monitorear ubicación de un contacto | Como contacto de confianza, quiero monitorear la ubicación en tiempo real de un ciudadano que comparte su trayecto para velar por su seguridad. | 5 | 8 | Giorgio Awad | In Progress |
| 10 | US19 | Editar perfil de usuario | Como ciudadano, quiero editar mi perfil (nombre, foto, preferencias) para mantener mis datos actualizados. | 2 | 3 | Billy Ruiz | Done |
| 11 | US20 | Cerrar sesión | Como ciudadano, quiero cerrar sesión en la aplicación para proteger mi cuenta en dispositivos compartidos. | 1 | 1 | Billy Ruiz | Done |
| 12 | US22 | Visualizar heatmap de zonas de riesgo | Como ciudadano, quiero visualizar un heatmap (mapa de calor) sobre el mapa para identificar las zonas con mayor concentración de incidentes. | 5 | 8 | Ivan La Madrid | In Progress |
| 13 | TS04 | Implementar API REST de alertas y geolocalización | Como developer, quiero implementar los endpoints para el módulo de alertas, compartición de ubicación y notificaciones push. | 8 | 12 | Ivan La Madrid | In Progress |
| 14 | TS05 | Integrar Google Maps SDK en aplicaciones móviles | Como developer, quiero integrar el SDK de Google Maps en las apps Android y Flutter para mostrar el mapa de incidentes con marcadores y heatmap. | 8 | 12 | Giorgio Awad | In Progress |


##### 4.2.2.3. Development Evidence for Sprint Review 

Durante el Sprint 2 se completó la implementación de todos los módulos del núcleo funcional de UrbanVoice. El equipo logró finalizar la infraestructura backend al 100%, consolidando los endpoints REST para la gestión de incidentes, alertas geolocalizadas, compartición de ubicación en tiempo real, autenticación y panel de administración. Además, se desarrolló la integración del mapa interactivo con heatmap de zonas de riesgo y la capa de geolocalización.

En el lado móvil, se implementó el detalle de incidentes, el filtrado por tipo y fecha, el reporte anónimo, la gestión de perfil de usuario, el cierre de sesión, y se integró el SDK de Google Maps con marcadores y heatmap. También se habilitaron las funcionalidades de alertas por proximidad y compartición de ubicación en tiempo real. En el panel administrativo, se implementó la moderación de reportes y la gestión de categorías. Estas funcionalidades representan el corazón operativo del sistema, permitiendo la interacción directa entre ciudadanos, contactos de confianza y administradores.

Todo lo desarrollado, se ve reflejado en los siguientes commits en cada unos de los repositorios:

#### Frontend Flutter:

| Repository | Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|---|
| Front-End | main | 97837f96d7a0b51807688dd4ca73e085045f9dc8 | fix/ mapa riesgos | 2026-06-16 10:56:20 -0500 |
| Front-End | main | 8508cea0f7e7121e289aca20bf65dd7c855cd09d | feat/app-version1 | 2026-06-16 10:44:48 -0500 |
| Front-End | main | a36f0502482d5a9b85710f8c2f41618f98341c9c | Initial commit | 2026-06-16 08:51:51 -0500 |

#### Frontend Android:

| Repository | Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|---|
| Front-End-Android | v1.0 | b68660f967abd9f3d11550ee560639373ddd8f35 | fix: Api google | 2026-06-22 22:11:40 -0500 |
| Front-End-Android | v1.0 | 76aa869d9a0aa609b7d9c66c14b4a4d2f130a3d9 | fix/ dependencias | 2026-06-22 22:03:31 -0500 |
| Front-End-Android | main / v1.0 | b321f1c3354584a43fca5d209548615e49b9278e | fix/ mapa | 2026-06-22 21:09:34 -0500 |
| Front-End-Android | main / v1.0 | 4510150e4ad83573adb2c1266bb285bc0ded545b | feat/ alertas | 2026-06-22 21:06:57 -0500 |
| Front-End-Android | main / v1.0 | 33e12707cf1ac6afcbbfec16378db606689ec666 | feat/ reportes | 2026-06-22 21:05:06 -0500 |
| Front-End-Android | main / v1.0 | 5801a5c9192e6db0f6665aaf4aedfdc02a0a1f38 | feat/ mapa | 2026-06-22 21:04:31 -0500 |
| Front-End-Android | main / v1.0 | 8c594cbbc2a45d543a1961616ab78bb9320ab13a | feat: data layer | 2026-06-22 21:03:15 -0500 |
| Front-End-Android | main / v1.0 | 54cef59acb45fc44769005a0cf36a60c343f3f77 | feat: domain layer | 2026-06-22 21:02:50 -0500 |
| Front-End-Android | main / v1.0 | 5d7b477d327b75f0211b82d92c8e648929e0fa0a | feat: initial project | 2026-06-22 21:02:24 -0500 |
| Front-End-Android | main | 4c8393052527d1816461e1a89306f14c9ed738bd | Initial commit | 2026-06-22 20:49:26 -0500 |

#### Backend:
| Repository | Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|---|
| Backend-UrbanVoice | main | e18b3b41216e55d53249936e031eaed3c4480931 | feat/ version 2.5 | 2026-05-14 10:51:01 -0500 |
| Backend-UrbanVoice | develop | 36a8981a60cb893532dfdd6695a383d2d00609e8 | feat/ pruebas | 2026-05-11 15:05:21 -0500 |
| Backend-UrbanVoice | main | 8e1c43d772057b07ad11c78aff4f010b61eee954 | Merge pull request #2 from develop | 2026-05-11 14:42:57 -0500 |
| Backend-UrbanVoice | develop | 26f30beb000bde09fa58ae3023a8a05318bce5fd | feat/ steps y features | 2026-05-11 14:42:02 -0500 |
| Backend-UrbanVoice | main | 83cdec5db70d7230d453412ba88e5d4c048598f0 | Merge pull request #1 from develop | 2026-05-11 14:32:32 -0500 |
| Backend-UrbanVoice | develop | 3bdeca1a674105b13048617ad5dddac0008b739a | fix/ report | 2026-05-11 14:27:46 -0500 |
| Backend-UrbanVoice | develop | c008eade2a60b68b14ffd25c06626cab2c152bac | feat/ v2 | 2026-05-11 13:47:53 -0500 |
| Backend-UrbanVoice | develop | 84a69f47912c3536c2419279e3cf2809e227bce3 | feat/ reports | 2026-05-10 18:45:55 -0500 |
| Backend-UrbanVoice | develop | 9788eb84229a6b5ee693a349d6e1fc06e300225e | feat/ version sin autenticacion | 2026-05-10 18:36:46 -0500 |
| Backend-UrbanVoice | develop | c6e1b63560d32e319e52564f094670f8b507e44e | feat/ backend v1 1.0 | 2026-05-10 18:08:58 -0500 |
| Backend-UrbanVoice | develop | d8e2d2bc8a6a286a675ac67708d423de44631d08 | Initial commit | 2026-05-10 17:34:40 -0500 |

#### Landing Page:

| Repository | Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|---|
| landing-page | main | 809cbc0a8bc2891228d8cf213e3a2be3ba99ac26 | feat: agrega mapas reales con OpenStreetMap | 2026-06-14 03:20:37 -0500 |
| landing-page | main | 248511cff036bb351ca62cdf6701cc90eac1b886 | feat/ Landing v1 | 2026-05-10 17:30:33 -0500 |
| landing-page | main | ec7ad0b86c049f8d283d62effa2672427d77895c | Initial commit | 2026-05-10 17:04:44 -0500 |

##### 4.2.2.4. Testing Suite Evidence for Sprint Review 


Durante el Sprint 2 se ejecutó pruebas funcionales e integrales para validar las principales funcionalidades implementadas en UrbanVoice. Estas pruebas tuvieron como objetivo asegurar la correcta interacción entre frontend móvil y backend, así como verificar la estabilidad de los servicios REST y la lógica de negocio relacionada con geolocalización y reportes ciudadanos.

El alcance de las pruebas se centró en los módulos de autenticación, permisos de ubicación, visualización del mapa, registro de incidentes, carga de evidencia multimedia, reporte anónimo, alertas geolocalizadas, compartición de ubicación en tiempo real y panel de administración.

##### Cobertura de Pruebas

| Module | Feature Tested | Type |
|---|---|---|
| Authentication | Login, registration, password recovery | Integration |
| Incident Management | Incident creation, detail, filtering, anonymous mode | Integration |
| Evidence Management | Upload of multimedia files | Functional |
| Location & Alerts | GPS permissions, geolocation, proximity alerts | Functional |
| Admin Panel | Report moderation, category management | Functional |


##### Casos de Prueba Ejecutados


| Test ID | User Story | Escenario de prueba | Resultado esperado | Resultado obtenido | Estado |
|---|---|---|---|---|---|
| TC-01 | US16 | El usuario comparte su ubicación en tiempo real | El sistema genera un enlace de monitoreo activo | El enlace se generó correctamente y el contacto pudo ver la ubicación | Passed |
| TC-02 | US04 | El usuario abre el mapa de incidentes | El mapa carga con los marcadores de incidentes | El mapa se renderizó correctamente con datos de la API | Passed |
| TC-03 | US05 | El usuario envía un reporte de incidente | El incidente se almacena con su geolocalización | El incidente fue registrado correctamente en la base de datos | Passed |
| TC-04 | US06 | El usuario adjunta evidencia multimedia | El archivo se carga y se vincula al reporte | Imagen y video se cargaron correctamente | Passed |
| TC-05 | US11 | El usuario activa el modo anónimo | El reporte oculta la identidad del usuario | El campo anónimo se persistió correctamente | Passed |
| TC-06 | US15 | El usuario recibe una alerta de incidente cercano | El sistema envía notificación push con los detalles | La notificación se recibió en el dispositivo en menos de 5 segundos | Passed |
| TC-07 | TS04 | El frontend consume los endpoints de alertas | Los endpoints devuelven respuestas válidas | Se validaron correctamente respuestas HTTP (200, 201, 400) | Passed |

Los resultados obtenidos validan la estabilidad de las funcionalidades principales del Sprint 2, asegurando que UrbanVoice cuenta con una base sólida para la implementación de los módulos avanzados de pruebas de seguridad, WebSockets, caché y funcionalidades adicionales en el Sprint 3.

##### 4.2.2.5. Execution Evidence for Sprint Review 

El Sprint 2 fue ejecutado siguiendo la planificación establecida y priorizando las historias de usuario de mayor valor para la propuesta de UrbanVoice. La mayoría de tareas fueron completadas dentro del tiempo estimado, mientras que algunas historias (como las alertas por proximidad y la compartición de ubicación en tiempo real) continuaron en estado *In Progress* debido a ajustes técnicos en integración con Firebase Cloud Messaging y Google Maps SDK.

Se realizaron reuniones de seguimiento para monitorear el avance y resolver bloqueos relacionados con geolocalización, notificaciones push y almacenamiento multimedia. La ejecución permitió consolidar la base operativa del producto y preparar el sistema para funcionalidades avanzadas en el Sprint 3.

#### Capturas de la Landing Page:

**Presentacion:**
<img src="assets/LandingPage-1.png"/><br/>

**Funcionalidades:**
<img src="assets/LandingPage-2.png"/><br/>

**Footer:**
<img src="assets/LandingPage-3.png"/><br/>

#### Capturas del backend:

<img src="assets/BackEnd.png"/><br/>

#### Capturas del frontend:

##### Inicio de sesión:
<img src="assets/front-end/Front-End-1.png"/><br/>

<img src="assets/Pantalla de inicio de sesión de UrbanVoice.png" alt="Pantalla de inicio de sesión de UrbanVoice"/><br/>

##### Pantalla de registro de usuario

<img src="assets/Pantalla de registro de usuario de UrbanVoice.png" alt="Pantalla de registro de usuario de UrbanVoice"/><br/>

##### Navbar:
<img src="assets/front-end/Front-End-2.png"/><br/>

##### Perfil de usuario:
<img src="assets/front-end/Front-End-3.png"/><br/>

##### Mapa:
<img src="assets/front-end/Front-End-4.png"/><br/>

##### Reportes:
<img src="assets/front-end/Front-End-5.png"/><br/>


##### 4.2.2.6. Services Documentation Evidence for Sprint Review 

Durante este sprint se documentaron los servicios principales del backend correspondientes al núcleo funcional del sistema.

Los servicios implementados incluyen:

- **Incident Service:** Registro, consulta y almacenamiento de incidentes reportados.
- **Evidence Service:** Manejo de evidencia multimedia asociada a reportes.
- **Location Service:** Obtención de ubicación actual y cálculo de rutas seguras.

La documentación de endpoints se realizó utilizando Swagger/OpenAPI, permitiendo la validación de contratos REST y facilitando futuras integraciones.

##  Locations  
API para gestionar ubicaciones y zonas de riesgo.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener todas las ubicaciones | GET | `/api/v1/locations` | Ninguno | `[{"id":1,"name":"Parque Central","district":"Surco"}]` |
| Crear nueva ubicación | POST | `/api/v1/locations` | Body: `{ "name":"Plaza Norte","district":"Independencia" }` | `{ "id":2,"name":"Plaza Norte","district":"Independencia" }` |
| Obtener ubicación por ID | GET | `/api/v1/locations/{id}` | Path: `id` | `{ "id":1,"name":"Parque Central","district":"Surco" }` |
| Eliminar ubicación | DELETE | `/api/v1/locations/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Obtener ubicaciones cercanas | GET | `/api/v1/locations/nearby` | Query: `lat,long` | `[{"id":3,"name":"Plaza Mayor"}]` |
| Obtener ubicaciones por distrito | GET | `/api/v1/locations/district/{district}` | Path: `district` | `[{"id":4,"name":"Plaza Norte"}]` |
| Obtener ubicaciones peligrosas | GET | `/api/v1/locations/dangerous` | Ninguno | `[{"id":5,"name":"Zona Roja"}]` |

---

##  User Profiles  
API para gestionar perfiles de usuario.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener perfil por ID | GET | `/api/v1/profiles/{id}` | Path: `id` | `{ "id":5,"email":"user@mail.com" }` |
| Actualizar perfil | PUT | `/api/v1/profiles/{id}` | Path: `id`, Body: `{ "email":"new@mail.com" }` | `{ "id":5,"email":"new@mail.com","status":"updated" }` |
| Eliminar perfil | DELETE | `/api/v1/profiles/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Crear nuevo perfil | POST | `/api/v1/profiles` | Body: `{ "email":"user@mail.com","name":"Juan" }` | `{ "id":6,"status":"created" }` |
| Obtener perfil por email | GET | `/api/v1/profiles/email/{email}` | Path: `email` | `{ "id":6,"email":"user@mail.com" }` |

---

##  Incident Reports  
API para gestionar reportes de incidentes.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener reporte por ID | GET | `/api/v1/reports/{id}` | Path: `id` | `{ "id":10,"description":"Accidente en Av. Primavera" }` |
| Actualizar reporte | PUT | `/api/v1/reports/{id}` | Path: `id`, Body: `{ "description":"Actualización del reporte" }` | `{ "id":10,"status":"updated" }` |
| Eliminar reporte | DELETE | `/api/v1/reports/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Crear nuevo reporte | POST | `/api/v1/reports` | Body: `{ "userId":5,"description":"Accidente en Av. Primavera" }` | `{ "id":10,"status":"created" }` |
| Obtener reportes de un usuario | GET | `/api/v1/reports/user/{userId}` | Path: `userId` | `[{"id":11,"description":"Caída en Av. Benavides"}]` |
| Obtener reportes cercanos | GET | `/api/v1/reports/nearby` | Query: `lat,long` | `[{"id":12,"description":"Incidente en Parque Kennedy"}]` |

---

##  Alerts  
API para gestionar alertas y notificaciones.  

| Acción | Verbo HTTP | Sintaxis | Parámetros | Ejemplo Response |
|--------|------------|----------|------------|------------------|
| Obtener todas las alertas | GET | `/api/v1/alerts` | Ninguno | `[{"id":1,"message":"Zona peligrosa detectada"}]` |
| Crear nueva alerta | POST | `/api/v1/alerts` | Body: `{ "message":"Nueva alerta" }` | `{ "id":2,"status":"created" }` |
| Eliminar todas las alertas | DELETE | `/api/v1/alerts` | Ninguno | `{ "status":"deleted_all" }` |
| Obtener alerta por ID | GET | `/api/v1/alerts/{id}` | Path: `id` | `{ "id":2,"message":"Nueva alerta" }` |
| Eliminar alerta por ID | DELETE | `/api/v1/alerts/{id}` | Path: `id` | `{ "status":"deleted" }` |
| Obtener alertas por usuario | GET | `/api/v1/alerts/user/{userId}` | Path: `userId` | `[{"id":3,"message":"Alerta personalizada"}]` |


##### 4.2.2.7. Software Deployment Evidence for Sprint Review 
En este Sprint se realizó el despliegue del backend de UrbanVoice en Render, junto con la actualización de la Landing Page previamente desplegada en GitHub Pages. El backend se desplegó asegurando la conectividad con los frontends móviles mediante la API REST. Los frontends Android y Flutter se desplegaron en los repositorios correspondientes para su distribución.

**Paso 1:** Configurar el entorno de producción del backend 

<img src="assets/Paso1-Despliegue-Backend.png"/><br/>

**Paso 2:** Crear urbanvoice-db en Render

<img src="assets/Paso2-Despliegue-Backend.png"/><br/>

**Paso 3:** Guardar variables

<img src="assets/Paso3-Despliegue-Backend.png"/><br/>

**Paso 4:** Crear Web Service en Render

<img src="assets/Paso4-Despliegue-Backend.png"/><br/>

**Paso 5:** Desplegar Web Service

<img src="assets/Paso5-Despliegue-Backend.png"/><br/>

**Paso 6:** Probar Web Service desplegado

<img src="assets/Paso6-Despliegue-Backend.png"/><br/>


##### 4.2.2.8. Team Collaboration Insights during Sprint

Durante el Sprint 2 el equipo mantuvo una colaboración activa y coordinada para abordar la implementación de las funcionalidades core del sistema. La comunicación constante permitió resolver rápidamente dependencias entre frontend móvil y backend, especialmente en la integración de mapas y endpoints de reportes.

Se evidenció una mejor distribución de responsabilidades en comparación con el Sprint 1, optimizando tiempos de desarrollo y reduciendo bloqueos. El equipo identificó como principal aprendizaje la importancia de definir claramente las dependencias técnicas antes de iniciar nuevas funcionalidades, especialmente aquellas relacionadas con servicios externos como geolocalización y almacenamiento multimedia.

<img src="assets/Evidence Sprint Review.png"/><br/>

<img src="assets/Network.png"/><br/>


#### 4.2.3. Sprint 3

##### 4.2.3.1. Sprint Planning 3

Para este tercer sprint el equipo se enfocará en completar las funcionalidades restantes de UrbanVoice y consolidar la calidad del producto. Se implementarán las funcionalidades de gestión de contactos de confianza, activación/desactivación de alertas por zona, generación de reportes estadísticos para administradores, envío de notificaciones masivas, historial de reportes del ciudadano, confirmación de reportes procesados y valoración de reportes de otros usuarios. Además, se implementarán las mejoras técnicas necesarias: WebSockets para actualizaciones en tiempo real, sistema de caché con Redis para optimización de consultas, pruebas unitarias y de integración, y pruebas de seguridad y penetración.

| Sprint # | Sprint 3 |
|---|---|
| **Sprint Planning Background** | |
| **Date** | 20/05/2026 |
| **Time** | 07:00 PM |
| **Location** | Servidor de Discord del Equipo |
| **Prepared By** | Billy Jake Ruiz Madrid |
| **Attendees (to planning meeting)** | Ivan La Madrid / Jeremy Quijada / Billy Ruiz / Santiago Gordillo / Giorgio Awad |
| **Sprint 3 Review Summary** | En esta sesión se definió la implementación de las funcionalidades finales del sistema, incluyendo contactos de confianza, historial de reportes, reportes estadísticos, pruebas de seguridad y optimización con WebSockets y caché. |
| **Sprint 3 Retrospective Summary** | El equipo acordó priorizar la finalización de todas las funcionalidades pendientes, la optimización del rendimiento mediante WebSockets y caché, y la aseguramiento de la calidad mediante pruebas unitarias, de integración y de seguridad. |
| **Sprint Goal & User Stories** | |
| **Sprint 3 Goal** | Completar al 100% todas las funcionalidades de UrbanVoice en ambos frontends (Android y Flutter), implementar el sistema de valoración de reportes, historial de reportes ciudadanos, confirmación de reportes procesados, gestión de contactos de confianza, activación/desactivación de alertas por zona, reportes estadísticos y notificaciones masivas. Además, incorporar WebSockets para tiempo real, caché con Redis para optimización, y garantizar la calidad mediante pruebas unitarias, de integración y de seguridad. El éxito se logrará cuando ambas plataformas móviles tengan paridad de funcionalidades y el sistema supere todas las pruebas de seguridad. |
| **Sprint 3 Velocity** | 47 Velocity |
| **Sum of Story Points** | 47 Story Points |

---

##### 4.2.3.2. Sprint Backlog 3

| # Orden | User Story ID | Título | Descripción | Story Points | Estimation (hours) | Assigned To | Status |
|:---:|:---:|---|---|:---:|:---:|---|:---:|
| 1 | US18 | Activar o desactivar alertas por zona geográfica | Como ciudadano, quiero activar o desactivar las alertas de incidentes cercanos para ciertas zonas geográficas para personalizar mi experiencia. | 3 | 4 | Billy Ruiz | Pending |
| 2 | US21 | Gestionar contactos de confianza | Como ciudadano, quiero gestionar mi lista de contactos de confianza (agregar, eliminar) para compartir mi ubicación con personas de confianza. | 3 | 4 | Billy Ruiz | Pending |
| 3 | US23 | Generar reporte estadístico de incidentes | Como administrador, quiero generar reportes estadísticos de incidentes por período, zona y categoría para analizar tendencias de seguridad. | 5 | 8 | Jeremy Quijada | Pending |
| 4 | US24 | Enviar notificaciones masivas desde administración | Como administrador, quiero enviar notificaciones push masivas a los usuarios para comunicar alertas generales o información importante. | 3 | 4 | Jeremy Quijada | Pending |
| 5 | US25 | Visualizar historial de incidentes reportados | Como ciudadano, quiero ver el historial de todos los incidentes que he reportado para darles seguimiento. | 3 | 4 | Santiago Gordillo | Pending |
| 6 | US26 | Recibir confirmación de reporte procesado | Como ciudadano, quiero recibir una confirmación cuando mi reporte sea procesado por un administrador para saber su estado. | 2 | 3 | Santiago Gordillo | Pending |
| 7 | US27 | Valorar utilidad de reportes de otros usuarios | Como ciudadano, quiero valorar (like/dislike) los reportes de otros usuarios para destacar la información útil. | 2 | 3 | Santiago Gordillo | Pending |
| 8 | TS06 | Implementar pruebas unitarias y de integración | Como developer, quiero implementar pruebas unitarias y de integración para garantizar la calidad del backend y detectar regresiones. | 8 | 12 | Ivan La Madrid | Pending |
| 9 | TS07 | Implementar WebSockets para actualizaciones en tiempo real | Como developer, quiero implementar WebSockets en el backend para notificar cambios en tiempo real a los clientes conectados. | 5 | 8 | Ivan La Madrid | Pending |
| 10 | TS08 | Implementar sistema de caché y optimización de consultas | Como developer, quiero implementar un sistema de caché (Redis) para optimizar las consultas geolocalizadas y reducir la latencia. | 5 | 8 | Ivan La Madrid | Pending |
| 11 | TS09 | Realizar pruebas de seguridad y penetración | Como developer, quiero realizar pruebas de seguridad y penetración en la API para identificar y corregir vulnerabilidades antes del despliegue final. | 8 | 12 | Giorgio Awad | Pending |

---
##### 4.2.3.3. Development Evidence for Sprint Review 

Durante el Sprint 3 se concreto el funcionamiento de UrbanVoice. El equipo logró finalizar la infraestructura backend al 100%, consolidando los endpoints REST para la gestión de incidentes, alertas geolocalizadas, compartición de ubicación en tiempo real, autenticación y panel de administración. Además, se finalizo el desarrollo de las aplicaciones móviles para Android y Flutter, implementando la funcionalidad de mapas y notificaciones.

Todo lo desarrollado, se ve reflejado en los siguientes commits en cada unos de los repositorios:

##### *Front-End-Flutter*

| Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|
| main | ece3963 | fix: Mapa de riesgo | 04/07/2026 |
| main | dd7b668 | feat/ bakcend deployada | 04/07/2026 |
| main | 583e55f | fix: Terminos y condiciones | 04/07/2026 |
| main | cfcc99c | feat/ Tokens | 04/07/2026 |
| main | 5398b93 | feat/ Maps | 04/07/2026 |
| feature/location-domain-docs | 254b865 | docs: add Flutter app architecture overview | 01/07/2026 |
| feature/location-domain-docs | 0973a9a | docs(core): document API and app constants | 01/07/2026 |
| feature/location-domain-docs | 59fd7d6 | docs(domain): document Location and Alert entity fields | 01/07/2026 |
| chore/-code-clean-up | 4734021 | Update index.html | 01/07/2026 |
| chore/-code-clean-up | 3a8aac7 | fixing and update .gitignore | 01/07/2026 |
| chore/-code-clean-up | 19c31ae | Update main.dart to clean up | 01/07/2026 |
| location-ui-cleanup | 38aa6b4 | Add model conversion tests | 01/07/2026 |
| location-ui-cleanup | ff881ad | Improve register form validation | 01/07/2026 |
| location-ui-cleanup | b6ec676 | Fix incident type dropdown | 01/07/2026 |
| feature/home-screen | 97837f9 | fix/ mapa riesgos | 16/06/2026 |
| feature/home-screen | 8508cea | feat/app-version1 | 16/06/2026 |

##### *Front-End-Android*

| Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|
| v1.0 | 7fb76c0 | feat/ bakcend deployada | 04/07/2026 |
| v1.0 | 7660e82 | fix: Terminos y condiciones | 04/07/2026 |
| v1.0 | 68c0614 | fix: errors | 02/07/2026 |
| v1.0 | db7e18c | fix: errors | 02/07/2026 |
| v1.0 | 5cb3b49 | fix: errors | 02/07/2026 |
| v1.0 | c1b85b1 | fix: preferences | 02/07/2026 |
| v1.0 | 49f589a | fix: revision | 02/07/2026 |
| v1.0 | 7c2327c | feat/ Shared location | 01/07/2026 |
| feature/ui-update | 09a4d45 | Update README.md | 01/07/2026 |
| feature/ui-update | 89cfc13 | Adding rules to .gitignore | 01/07/2026 |
| feature/ui-update | 7d4e226 | Update gradle.properties | 01/07/2026 |
| main | 1204455 | docs: update frontend README. | 01/07/2026 |
| location-map-polish | 7a97015 | feat(location): show map marker summary | 01/07/2026 |
| location-map-polish | e734682 | fix(location): show map loading errors | 01/07/2026 |
| location-map-polish | 1f01ed4 | refactor(location): name map search defaults | 01/07/2026 |
| v1.0 | 5ef30d9 | feat/ Terminos y Condiciones | 01/07/2026 |
| v1.0 | c2b92b3 | fix/ Mapa de riesgo | 01/07/2026 |
| v1.0 | d589143 | fix: token iam | 01/07/2026 |
| v1.0 | 476a9cd | feat/IAM | 01/07/2026 |
| v1.0 | 685374e | feat/log In | 01/07/2026 |
| v1.0 | 90dfde5 | fix(auth): trim email before submit | 01/07/2026 |
| v1.0 | 2ea4c2c | fix(profile): avoid empty name initials crash | 01/07/2026 |
| v1.0 | 9dc29d8 | refactor(home): extract default Lima map coordinates | 01/07/2026 |
| v1.0 | 6e06efc | fix(register): show password mismatch error | 01/07/2026 |
| v1.0 | 459da93 | fix: gradle | 24/06/2026 |
| v1.0 | 000d5b6 | fix: map views | 23/06/2026 |
| fix-v1.0 | b68660f | fix: Api google | 22/06/2026 |
| v1.0 | 76aa869 | fix/ dependencias | 22/06/2026 |
| v1.0 | b321f1c | fix/ mapa | 22/06/2026 |
| v1.0 | 4510150 | feat/ alertas | 22/06/2026 |
| v1.0 | 33e1270 | feat/ reportes | 22/06/2026 |
| v1.0 | 5801a5c | feat/ mapa | 22/06/2026 |
| v1.0 | 8c594cb | feat: data layer | 22/06/2026 |
| v1.0 | 54cef59 | feat: domain layer | 22/06/2026 |
| v1.0 | 5d7b477 | feat: initial project | 22/06/2026 |

##### *Backend-UrbanVoice*

| Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|
| main | 0937433 | fix: incidents | 02/07/2026 |
| main | e130714 | fix: dependencies | 02/07/2026 |
| main | 47d2e74 | feat/ Password | 02/07/2026 |
| main | b383509 | Merge branch 'main' | 01/07/2026 |
| main | 68003a3 | feat/ Shared location | 01/07/2026 |
| feature/report-status | 267b861 | fix(reports): persistence and repository mappings | 01/07/2026 |
| feature/report-status | a3f14c1 | fix(reports): persistence and repository mappings | 01/07/2026 |
| feature/report-status | d397ed8 | fix(reports): application service | 01/07/2026 |
| feature/report-status | 9a5d2e5 | fix(reports): domain model and validation | 01/07/2026 |
| feature/report-status | 60b95ea | fix(reports): queries | 01/07/2026 |
| feature/report-status | 59409f1 | fix(reports): commands | 01/07/2026 |
| feature/report-status | 6cf33ff | Merge branch 'main' into feature/report-status | 01/07/2026 |
| feature/-clean-and-format-comments-imports | c67a16d | Update Dockerfile | 01/07/2026 |
| feature/-clean-and-format-comments-imports | 1e10072 | fixing backend .gitignore | 01/07/2026 |
| feature/locations-notifications-docs | 0644406 | docs: add high-level backend architecture overview | 01/07/2026 |
| feature/locations-notifications-docs | 2e07823 | docs(iam,districts): bounded context package-info | 01/07/2026 |
| feature/locations-notifications-docs | 060f06d | docs(notifications): document package layout | 01/07/2026 |
| feature/locations-notifications-docs | 8594310 | docs(locations): add Javadoc to Location entity | 01/07/2026 |
| feature/locations-notifications-docs | 8348ae9 | docs(locations): add package-info documentation | 01/07/2026 |
| main | 6062cbc | Update README.md | 01/07/2026 |
| main | bca53e6 | docs: update backend README. | 01/07/2026 |
| feature/iam-docs-cleanup | e7a4d69 | refactor(iam): centralize bearer token prefix | 01/07/2026 |
| feature/iam-docs-cleanup | 8b4aee1 | docs: list iam and districts contexts | 01/07/2026 |
| feature/iam-docs-cleanup | 8430985 | docs: align backend stack requirements | 01/07/2026 |
| main | ddbe07d | Fix Dockerfile: skip test compilation | 01/07/2026 |
| main | 34309c6 | Add local defaults for env vars | 01/07/2026 |
| main | a73d027 | Configure env vars for Render deployment | 01/07/2026 |
| main | 135ed3c | fix/ mensajes de respuesta de los endpoints | 01/07/2026 |
| main | aadfb23 | feat/Iam | 01/07/2026 |
| main | ef67c2e | fix: AlertController | 23/06/2026 |
| main | 9cac218 | fix: indicent managment | 23/06/2026 |

##### *UrbanVoice*

| Branch | CommitID | Commit Message | Commit On |
|---|---|---|---|
| TF | 74500e6 | feat/ Software Deployment Evidence for Sprint Review | 04/07/2026 |
| TF | 67bb106 | Video link in README for About the product | 04/07/2026 |
| TF | 0d00834 | docs: add testing suite evidence | 04/07/2026 |
| TF | d7d0657 | Revise Sprint 3 execution evidence in README | 04/07/2026 |
| TF | dc78f20 | Update README with sprint review sections | 04/07/2026 |
| TF | b0e883b | Add files via upload | 04/07/2026 |
| TF | b82500e | Add files via upload | 04/07/2026 |
| TF | 0e920e0 | Replace old image paths with new ones | 04/07/2026 |
| TF | 026b9be | Add files via upload | 04/07/2026 |
| TF | fea9405 | Add files via upload | 04/07/2026 |
| TF | 3151095 | Update README.md | 04/07/2026 |
| TF | c88172b | Add files via upload | 04/07/2026 |
| TF | 6304b23 | Update README with new images and features | 04/07/2026 |
| TF | 21d4662 | Add files via upload | 04/07/2026 |
| TF | c56ebfb | Update README Sprint 3 evidence | 04/07/2026 |
| main | 6f32f6c | Fix image paths in README | 04/07/2026 |
| main | 84d278e | Add files via upload | 04/07/2026 |
| TB2 | d1c6c13 | Add team link to README | 02/07/2026 |
| TB2 | ef9f44e | Enhance product and team information | 02/07/2026 |
| TB2 | 9631128 | feat/ Sprint 3 | 01/07/2026 |
| TB2 | 6170613 | fix: Sprint 1 | 01/07/2026 |
| TB2 | d8219a8 | fix: product backlog | 01/07/2026 |
| TB2 | cac723f | fix: user stories | 01/07/2026 |
| TB2 | 38675ce | Add product details and YouTube link | 01/07/2026 |
| TB2 | 953f9f7 | feat/ Student Outcome | 24/06/2026 |
| TB2 | d11af4b | fix: product backlog | 24/06/2026 |
| TB2 | 575eac6 | feat/ Sprint Evidences | 23/06/2026 |
| TB2 | a91195f | feat/ Sprint 2 y Sprint 3 | 23/06/2026 |
| TB2 | 184b339 | fix: user flows | 23/06/2026 |
| TB2 | 98029fb | docs(chapter4): add sprint 2 documentation. | 17/06/2026 |
| main | e97b60c | Adjust productk backlog | 08/06/2026 |
| main | 09aebb2 | Merge pull request #8 from .../TP | 08/06/2026 |

---

##### 4.2.3.4. Testing Suite Evidence for Sprint Review 

Durante el Sprint 3 se continuó con la validación de las funcionalidades principales de UrbanVoice, enfocándonos principalmente en los servicios del backend relacionados con reportes ciudadanos, perfiles de usuario, ubicaciones de riesgo y alertas. Para esta etapa se utilizó un enfoque de pruebas BDD, elaborando escenarios en lenguaje Gherkin mediante archivos `.feature` y conectándolos con archivos `Steps` desarrollados en Java. Estas pruebas permiten validar que los Web Services respondan correctamente según los criterios de aceptación definidos para las historias de usuario del sprint.

Las pruebas automatizadas se ubicaron dentro del repositorio del backend, en la carpeta `src/test`, separando los escenarios BDD en `src/test/resources/features` y las definiciones de pasos en `src/test/java/com/upc/pre/urbanvoiceapp/bdd/steps`. Además, se configuró un runner de Cucumber para ejecutar la suite de pruebas y una configuración de Spring Boot para levantar el contexto de la aplicación durante la validación.

### Relación de pruebas diseñadas

| Test ID | User Story relacionada | Tipo de prueba | Feature File | Steps File | Escenarios validados | Estado |
|---|---|---|---|---|---|---|
| TS01 | Como ciudadano, quiero reportar incidentes para informar a otros usuarios sobre amenazas de seguridad. | Acceptance Test / BDD | `IncidentReporting.feature` | `IncidentReportingSteps.java` | Crear reporte, registrar ubicación, reporte anónimo, actualizar reporte, obtener por ID, listar por usuario, eliminar reporte y validar tipo de incidente inválido. | Completed |
| TS02 | Como usuario, quiero gestionar mi perfil para poder usar las funcionalidades de UrbanVoice. | Acceptance Test / BDD | `UserProfiles.feature` | `UserProfileSteps.java` | Crear perfil, validar email duplicado, actualizar datos, buscar por email, manejar perfil inexistente y eliminar perfil. | Completed |
| TS03 | Como ciudadano, quiero consultar zonas de riesgo para evitar lugares peligrosos. | Acceptance Test / BDD | `LocationRiskAnalysis.feature` | `LocationRiskAnalysisSteps.java` | Identificar riesgo bajo, medio, alto y crítico; buscar incidentes cercanos; obtener zonas por nivel de riesgo y validar coordenadas inválidas. | Completed |
| TS04 | Como ciudadano, quiero recibir alertas sobre incidentes cercanos para mantenerme informado. | Acceptance Test / BDD | `AlertNotifications.feature` | `AlertNotificationsSteps.java` | Recibir alerta por incidente cercano, alerta por zona crítica, evitar alertas por incidentes lejanos, notificación push, email, lectura de alerta, archivo de alertas y desactivación temporal. | Completed |

### Descripción de los archivos de pruebas

| Archivo | Ubicación | Descripción |
|---|---|---|
| `IncidentReporting.feature` | `src/test/resources/features` | Define los escenarios BDD para validar el flujo de reportes de incidentes ciudadanos. |
| `UserProfiles.feature` | `src/test/resources/features` | Define los escenarios BDD para validar la creación, consulta, actualización y eliminación de perfiles. |
| `LocationRiskAnalysis.feature` | `src/test/resources/features` | Define los escenarios para validar el análisis de riesgo por ubicación y la búsqueda de incidentes cercanos. |
| `AlertNotifications.feature` | `src/test/resources/features` | Define los escenarios para validar el sistema de alertas y notificaciones. |
| `IncidentReportingSteps.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd/steps` | Implementa los pasos de prueba para los escenarios de reportes. |
| `UserProfileSteps.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd/steps` | Implementa los pasos de prueba para los escenarios de perfiles de usuario. |
| `LocationRiskAnalysisSteps.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd/steps` | Implementa los pasos de prueba para los escenarios de riesgo por ubicación. |
| `AlertNotificationsSteps.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd/steps` | Implementa los pasos de prueba para los escenarios de alertas y notificaciones. |
| `RunCucumberTest.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd` | Runner encargado de ejecutar la suite de pruebas BDD con Cucumber. |
| `CucumberSpringConfiguration.java` | `src/test/java/com/upc/pre/urbanvoiceapp/bdd` | Configuración para integrar Cucumber con el contexto de Spring Boot. |

### Evidencia de commits relacionados con Testing

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed on |
|---|---|---|---|---|---|
| `urbanvoice-3248-dispo-moviles/Backend-UrbanVoice` | `main` | `26f30be` | `feat/ steps y features` | Se agregaron los archivos `.feature`, los Steps de Cucumber, el runner de pruebas y la configuración BDD para validar perfiles, reportes, ubicaciones y alertas. | 11/05/2026 |
| `urbanvoice-3248-dispo-moviles/Backend-UrbanVoice` | `main` | `e18b3b4` | `feat/ version 2.5` | Se actualizaron dependencias y ajustes de configuración del backend, incluyendo dependencias de testing para Cucumber, JUnit Platform y H2. | 14/05/2026 |
| `urbanvoice-3248-dispo-moviles/UrbanVoice` | `TF` | `c3f668b` | `feat/ Testing Suite Evidence for Sprint Review` | Se agregó al informe la evidencia de Testing Suite, incluyendo capturas de Features, Steps y backend. | 11/05/2026 |

### Evidencia de validación funcional durante el Sprint

Además de las pruebas BDD del backend, durante el Sprint 3 se realizaron validaciones funcionales sobre la aplicación móvil y la API desplegada. Estas validaciones permitieron comprobar que los flujos principales de UrbanVoice funcionaran correctamente desde la interfaz móvil y desde herramientas de prueba como Postman. Entre los flujos revisados se encuentran el registro de reportes, consulta de reportes, validación de perfiles, consulta de ubicaciones y revisión de alertas.

| Repositorio | Validación realizada | Resultado |
|---|---|---|
| `Backend-UrbanVoice` | Validación de endpoints para perfiles, reportes, ubicaciones y alertas. | Los endpoints principales respondieron correctamente. |
| `Front-End-Android` | Validación de navegación, autenticación, perfil, reportes, mapa y alertas. | Se identificaron y corrigieron errores menores de interfaz y flujo. |
| `Front-End-Flutter` | Validación de pantallas principales, mapa y términos/condiciones. | Se realizaron ajustes de integración y presentación. |

En conclusión, la Testing Suite del Sprint 3 permitió verificar los principales flujos del sistema desde el backend y complementar la validación con pruebas funcionales en las aplicaciones móviles. Esto ayudó a reducir errores antes de la Sprint Review y a confirmar que las funcionalidades principales de UrbanVoice se encontraban listas para ser demostradas.

---
##### 4.2.3.5. Execution Evidence for Sprint Review 

El Sprint 3 fue ejecutado siguiendo la planificación establecida y priorizando las historias de usuario de mayor valor para la propuesta de UrbanVoice. La mayoría de tareas fueron completadas dentro del tiempo estimado, y las historias pendientes del sprint 2 fueron completadas.

#### Capturas de la Landing Page:

**Presentacion:**
<img src="assets/landing1.png"/><br/>

**Funcionalidades:**
<img src="assets/funcionalidades2.png"/><br/>

**Footer:**
<img src="assets/final1.png"/><br/>

#### Capturas del backend:

<img src="assets/BackEnd.png"/><br/>

#### Capturas del frontend:

##### Inicio de sesión:
<img src="assets/front-end/Front-End-1.png"/><br/>

<img src="assets/Pantalla de inicio de sesión de UrbanVoice.png" alt="Pantalla de inicio de sesión de UrbanVoice"/><br/>

##### Pantalla de registro de usuario

<img src="assets/Pantalla de registro de usuario de UrbanVoice.png" alt="Pantalla de registro de usuario de UrbanVoice"/><br/>

##### Mapa principal de riesgo

<img src="assets/front-end/Front-End-3.png"/><br/>

##### Pantalla de mis reportes

<img src="assets/front-end/Front-End-5.png"/><br/>

<img src="assets/Pantalla de mis reportes realizados.png" alt="Pantalla de mis reportes realizados"/><br/>

##### Navbar:
<img src="assets/front-end/Navbar.png"/><br/>

##### Perfil de usuario:

<img src="assets/front-end/Perfil.png"/><br/>

<img src="assets/Pantalla de perfil del usuario.png" alt="Pantalla de perfil del usuario"/><br/>

##### Ruta Segura:

<img src="assets/front-end/RutaSegura.png"/><br/>

<img src="assets/RutaSegura1.png" alt="RutaSegura"/><br/>

##### Compartir Ubicacion:

<img src="assets/front-end/Ubicacion.png"/><br/>

<img src="assets/Ubicacion2.png" alt="Ubicacion"/><br/>

---
##### 4.2.3.6. Services Documentation Evidence for Sprint Review
<img src="assets/endpoint-1.png"/><br/>
<img src="assets/endpoint-2.png"/><br/>
<img src="assets/endpoint-3.png"/><br/>
<img src="assets/endpoint-4.png"/><br/>
<img src="assets/endpoint-5.png"/><br/>
<img src="assets/endpoint-6.png"/><br/>
---
##### 4.2.3.7. Software Deployment Evidence for Sprint Review 

En este Sprint se realizó el despliegue del backend de UrbanVoice en Render. Se desplegó asegurando la conectividad con los frontends móviles mediante la API REST. Los frontends Android y Flutter se desplegaron en los repositorios correspondientes para su distribución.

**Paso 1:** Configurar el entorno de producción del backend 

<img src="assets/Paso1-Despliegue-Backend.png"/><br/>

**Paso 2:** Crear urbanvoice-db en Render

<img src="assets/Paso2-Despliegue-Backend.png"/><br/>

**Paso 3:** Guardar variables

<img src="assets/Paso3-Despliegue-Backend.png"/><br/>

**Paso 4:** Crear Web Service en Render

<img src="assets/Paso4-Despliegue-Backend.png"/><br/>

**Paso 5:** Desplegar Web Service

<img src="assets/Paso5-Despliegue-Backend.png"/><br/>

**Paso 6:** Probar Web Service desplegado

<img src="assets/Paso6-Despliegue-Backend.png"/><br/>


Ademas en este Sprint se realizó el despliegue del frontend de UrbanVoice en Firebase.


---
##### 4.2.3.8. Team Collaboration Insights during Sprint

Durante el Sprint 3 el equipo consolidó su dinámica de trabajo colaborativo, logrando coordinar eficientemente los esfuerzos entre los desarrolladores de backend y los dos frentes móviles (Android y Flutter). La comunicación fluida a través de Discord permitió resolver rápidamente incidencias de integración, especialmente en la sincronización de WebSockets y el consumo de los endpoints de reportes y alertas.

Se evidenció una madurez en la distribución de responsabilidades, logrando que ambos frontends avanzaran en paralelo con el backend sin cuellos de botella. El equipo identificó como principal aprendizaje la importancia de mantener una comunicación temprana sobre los cambios en la API y la necesidad de contar con ambientes de prueba sincronizados para evitar desfases entre repositorios. La colaboración constante permitió cumplir con las metas del sprint y entregar un producto funcional en ambas plataformas móviles.

<img src="assets/Evidence Sprint Review.png"/><br/>

<img src="assets/Network.png"/><br/>

### Conclusiones

*  Como equipo, logramos dar el salto de una idea social a un modelo técnico sólido. El uso de **EventStorming y el Modelo C4** nos permitió visualizar no solo cómo se ve la app, sino cómo fluye la información entre los módulos de reportes y geolocalización, asegurando que la arquitectura soporte el tráfico de datos en tiempo real que planeamos para Lima.
* Mediante las entrevistas y el proceso de **Needfinding**, confirmamos que nuestra propuesta de valor es acertada. Identificamos que el usuario no solo quiere ver el peligro, sino sentirse acompañado; por ello, la inclusión del "Círculo de Confianza" y las alertas de proximidad se convirtieron en pilares fundamentales que diferencian a UrbanVoice de otras apps de mapas convencionales.

###  About the product:

UrbanVoice es una aplicación móvil tecnológica y colaborativa enfocada en fortalecer la seguridad ciudadana en Lima Metropolitana. Ante la alarmante cifra de que casi el 90% de los ciudadanos percibe inseguridad en las calles, esta plataforma surge como una herramienta preventiva que no solo informa, sino que conecta a la comunidad para evitar situaciones de riesgo. Si deseas conocer mas sobre la aplicacion te invitamos a ver el siguiente video.

Link: https://youtu.be/Lvl-K2Y__hM 


###  About the Team:

Link: https://youtu.be/-vnQ4Qf8-AU

###  APP Validation:

### Recomendaciones

* Recomendamos enfocarnos de inmediato en los "Spikes" de integración con Google Maps y Firebase. Como el mapa de calor es el corazón de nuestra solución, necesitamos asegurar cuanto antes que el renderizado de múltiples puntos de riesgo no afecte el rendimiento del celular, especialmente en dispositivos de gama media que usa gran parte de nuestro segmento objetivo.
* Sugerimos profundizar en el diseño del "Panel de Moderación" para administradores. Para mantener la confianza de la comunidad, es vital establecer filtros automáticos o procesos de validación comunitaria (votos) que eviten que reportes maliciosos o falsos ensucien el mapa de riesgo, algo que identificamos como una debilidad potencial en el análisis de competidores.

## Anexo

**Repositorio Report:**  https://github.com/urbanvoice-3248-dispo-moviles/UrbanVoice

**Repositorio Landing Page:** https://github.com/urbanvoice-3248-dispo-moviles/Landing-Page

**Repositorio BackEnd:** https://github.com/urbanvoice-3248-dispo-moviles/Backend-UrbanVoice

**Repositorio FrontEnd Android:** https://github.com/urbanvoice-3248-dispo-moviles/Front-End-Android

**Repositorio FrontEnd Flutter:** https://github.com/urbanvoice-3248-dispo-moviles/Front-End-Flutter

**Enlace Deploy Landing Page:** https://urbanvoice-3248-dispo-moviles.github.io/Landing-Page/

**Enlace Deploy Front-End:** https://backend-urbanvoice.onrender.com/swagger-ui/index.html


# Glosario

* **Bounded Context:** Límite explícito dentro del cual vive un modelo de dominio específico y su lenguaje ubicuo.
* **C4 Model:** Marco de trabajo para documentar arquitecturas de software mediante niveles (Contexto, Contenedor, Componente y Código).
* **FCM (Firebase Cloud Messaging):** Servicio utilizado para el envío de notificaciones push geolocalizadas.
* **Geofencing:** Perímetro virtual para un área geográfica real que dispara alertas cuando un dispositivo entra o sale.
* **Heatmap (Mapa de Calor):** Representación gráfica de datos donde los valores se denotan por colores para mostrar la densidad de incidentes.
* **JWT (JSON Web Token):** Estándar para la transmisión segura de información entre partes como un objeto JSON, usado para autenticación.
* **Lean UX:** Metodología que se enfoca en la experiencia de usuario y la validación rápida de hipótesis mediante productos mínimos viables.


