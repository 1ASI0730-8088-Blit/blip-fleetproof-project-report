# Capítulo V: Product Implementation, Validation & Deployment

## 5.1 Software Configuration Management

### 5.1.1 Software Development Environment Configuration

En esta sección se detallan las herramientas y plataformas de software adoptadas por el equipo para coordinar, diseñar, implementar y documentar el ciclo de vida del producto digital. Se especifican el propósito de uso de cada herramienta, su tipo de ejecución y la ruta de acceso o descarga oficial correspondiente:

| Herramienta / Software | Tipo / Modelo | Propósito en el Proyecto | Actividad Asociada | Enlace de Referencia / Acceso |
| :--- | :--- | :--- | :--- | :--- |
| **Miro** | SaaS (Nube) | Plataforma de pizarra visual colaborativa utilizada para la realización de las dinámicas de *EventStorming* (Big Picture y Design-Level), mapeo de procesos de negocio y exploración visual del dominio. | Requirements Management & Domain Modeling | [https://miro.com/](https://miro.com/) |
| **Figma** | SaaS (Nube) | Herramienta de diseño de interfaces vectoriales y prototipado empleada para definir la guía de estilos visuales, *wireframes*, *mock-ups* y los flujos de interacción del *Landing Page* y la aplicación web. | Product UX/UI Design | [https://figma.com/](https://figma.com/) |
| **HackMD (HackMD.io)** | SaaS (Nube) | Entorno de edición colaborativa en tiempo real en formato Markdown, utilizado para redactar, revisar y sincronizar colectivamente el contenido de las secciones del informe de proyecto. | Project Documentation & Reporting | [https://hackmd.io/](https://hackmd.io/) |
| **GitHub** | SaaS (Nube) | Plataforma de alojamiento de repositorios Git utilizada para la gestión centralizada del código fuente, aplicación del flujo *GitFlow*, seguimiento de *commits*, métricas de contribución y control de versiones del informe del proyecto. | Source Code Management & Collaboration | [https://github.com/](https://github.com/) |

### 5.1.2 Source Code Management

Para garantizar la integridad, trazabilidad y el trabajo colaborativo en el desarrollo de la solución, el equipo utiliza **GitHub** como plataforma centralizada de alojamiento y control de versiones bajo Git.

##### Repositorios del Proyecto

| Producto / Artefacto | Propósito | Enlace al Repositorio en GitHub |
| :--- | :--- | :--- |
| **Project Documentation Report** | Repositorio para la elaboración colaborativa del informe técnico del proyecto en formato Markdown. | [blip-fleetproof-project-report](https://github.com/1ASI0730-8088-Blit/blip-fleetproof-project-report) |
| **Landing Page** | Repositorio del sitio web estático para la presentación comercial y conversión del modelo de negocio. | [fleetproof-landing-page](https://github.com/1ASI0730-8088-Blit/fleetproof-landing-page) |
##### Flujo de Ramas: GitFlow Workflow

El equipo implementa el modelo de flujo de trabajo **GitFlow**, estructurando el ciclo de desarrollo a través de ramas principales y ramas temporales de soporte:

1. **Ramas Principales:**
   * `main`: Contiene el código fuente en estado de producción, estable y totalmente desplegable. Todo cambio en esta rama proviene exclusivamente de fusiones validadas de ramas de lanzamiento (*release*) o parches urgentes (*hotfix*).
   * `develop`: Actúa como la rama de integración continua y base para el desarrollo diario. En ella se consolidan todas las funcionalidades culminadas y revisadas que formarán parte de la siguiente iteración.

2. **Ramas de Soporte:**
   * `feature/<nombre-de-tarea>`: Se desprenden de `develop` para la construcción aislada de una historia de usuario, componente de interfaz o sección de documentación. Una vez completada y verificada la tarea, se integra nuevamente en `develop` a través de un *Pull Request* con revisión previa de pares.
     * *Convención para desarrollo de software:* `feature/<US-ID>-<short-description>` (Ejemplo: `feature/US01-landing-hero`, `feature/US02-pricing-cards`).
     * *Convención para informe de proyecto:* `feature/sprint<n>-capitulo-<id>` (Ejemplo: `feature/sprint1-capitulo-5`).
   * `release/v<MAJOR.MINOR.PATCH>`: Se crean a partir de `develop` al alcanzar el congelamiento de características planeadas para un hito de entrega (Sprint Review). Sirven para realizar pruebas de aceptación finales, ajustes menores de documentación y preparar el despliegue. Se fusionan hacia `main` (etiquetando el lanzamiento) y de vuelta hacia `develop`.
   * `hotfix/v<MAJOR.MINOR.PATCH>`: Se desprenden directamente de `main` en caso de requerir la corrección crítica e inmediata de un defecto en el entorno de producción. Se fusionan simultáneamente a `main` y a `develop`.

##### Versionado Semántico (Semantic Versioning 2.0.0)

Para el control de versiones y etiquetado de los lanzamientos oficiales (*releases*), se adopta el estándar **SemVer 2.0.0** bajo la nomenclatura `vMAJOR.MINOR.PATCH`:

* **MAJOR:** Incrementa ante cambios incompatibles con versiones previas (*breaking changes*) o entregas de arquitectura estructurales mayores (Ejemplo: transición de entregas mayores finales).
* **MINOR:** Incrementa cuando se añaden nuevas funcionalidades, vistas o endpoints que son compatibles con las versiones existentes hacia atrás (Ejemplo: cierre de un nuevo Sprint como `v0.1.0` para Sprint 1, `v0.2.0` para Sprint 2).
* **PATCH:** Incrementa cuando se introducen correcciones de errores, ajustes de accesibilidad o parches menores que no alteran la compatibilidad previa (Ejemplo: `v0.1.1`).

##### Convención de Mensajes: Conventional Commits

Para mantener un historial de confirmaciones (*commits*) claro, legible y automatizable, los mensajes deben redactarse en idioma inglés siguiendo la especificación de **Conventional Commits**:

* **Estructura obligatoria:**
  ```text
  <type>(<scope>): <short description in present tense>

### 5.1.3 Source Code Style Guide & Coding Conventions

TODO: Documentar convenciones para HTML, CSS, JavaScript y C#. Toda nomenclatura de código debe estar en inglés.

### 5.1.4 Software Deployment Configuration

TODO: Especificar configuración de despliegue de Landing Page, Frontend Web Application y Web Services.

## 5.2 Landing Page, Services & Applications Implementation

### 5.2.1 Sprint 1

#### 5.2.1.1 Sprint Planning 1

| Campo | Valor |
|---|---|
| Sprint # | Sprint 1 |
| Date | TODO |
| Time | TODO |
| Location | TODO |
| Prepared By | Reyes Limo Sebastian |
| Attendees | Reyes Limo Sebastian / Palomino Murga Daniel Stalin / Becerra Durand Sebastian Uriel / Gómez De La Torre Huertas Rodrigo Fernando / Payesa Torres Harrison Hubert |
| Sprint 1 Goal | Our focus is on presenting FleetProof's value proposition and segment-specific calls to action through the first deployed Landing Page. We believe it delivers clarity to fleet companies and vehicle owners. This will be confirmed when visitors can understand the product and access the corresponding call-to-action for their segment. |
| Sprint 1 Velocity | TODO |
| Sum of Story Points | TODO |

#### 5.2.1.2 Aspect Leaders and Collaborators

| Team Member | GitHub Username | SCM and Rubric | Lean UX | UX Research | Requirements | Product Design and Landing Page |
|---|---|---|---|---|---|---|
| Reyes Limo Sebastian | llegastian11 | L | C | C | C | C |
| Palomino Murga Daniel Stalin | DanielPM23 | C | L | C | C | C |
| Becerra Durand Sebastian Uriel | TODO | C | C | L | C | C |
| Gómez De La Torre Huertas Rodrigo Fernando | TODO | C | C | C | L | C |
| Payesa Torres Harrison Hubert | TODO | C | C | C | C | L |

#### 5.2.1.3 Sprint Backlog 1

| Sprint # | Story Id | Story Title | Task Id | Task Title | Task Description | Estimation (Hours) | Assigned To | Status |
|---|---|---|---|---|---|---:|---|---|
| Sprint 1 | US001 | View value proposition | T001 | Draft Landing Page content | Redactar propuesta de valor, segmentos y beneficios. | 2 | Payesa Torres Harrison Hubert | To-do |
| Sprint 1 | US002 | Fleet monitoring CTA | T002 | Implement fleet CTA | Crear call-to-action hacia flujo empresarial. | 2 | Payesa Torres Harrison Hubert | To-do |
| Sprint 1 | US003 | Vehicle report CTA | T003 | Implement vehicle CTA | Crear call-to-action hacia flujo particular. | 2 | Payesa Torres Harrison Hubert | To-do |
| Sprint 1 | US004 | Compare plans | T004 | Add plan comparison | Presentar tres planes con límites. | 3 | Gómez De La Torre Huertas Rodrigo Fernando | To-do |
| Sprint 1 | US005 | View legal pages | T005 | Add legal links | Crear Terms and Conditions y Privacy Policy. | 2 | Reyes Limo Sebastian | To-do |

#### 5.2.1.4 Development Evidence for Sprint Review

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Committed on |
|---|---|---|---|---|---|
| TODO | TODO | TODO | TODO | TODO | TODO |

#### 5.2.1.5 Execution Evidence for Sprint Review

TODO: Incluir screenshots de Landing Page desplegada y video de navegación.

#### 5.2.1.6 Services Documentation Evidence for Sprint Review

Para AV1, los Web Services se registran como planificación técnica si todavía no forman parte del alcance implementado.

| Endpoint | HTTP Verb | Description | Status | Evidence |
|---|---|---|---|---|
| `/api/v1/plans` | GET | List plans | Planned | TODO |
| `/api/v1/report-requests` | POST | Create report request | Planned | TODO |

#### 5.2.1.7 Software Deployment Evidence for Sprint Review

TODO: Incluir URL desplegada, capturas del proveedor y versión `v1.0.0` del Landing Page.

#### 5.2.1.8 Team Collaboration Insights during Sprint

TODO: Incluir capturas de commits, Pull Requests, merges y contributors.

## 5.3 Validation Interviews

### 5.3.1 Diseño de Entrevistas

TODO: Definir tareas de validación para Landing Page y Web Application.

### 5.3.2 Registro de Entrevistas

TODO: Registrar entrevistas de validación por segmento.

### 5.3.3 Evaluaciones según heurísticas

TODO: Aplicar formato de evaluación UX por heurísticas.

## 5.4 Video About-the-Product

TODO: Incluir screenshot, URL Microsoft Stream, URL YouTube y duración.

