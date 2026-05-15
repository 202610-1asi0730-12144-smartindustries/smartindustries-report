# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management

En esta sección, el equipo establece las decisiones, herramientas y convenciones que permiten mantener la consistencia técnica durante el ciclo de vida de **SmartLock**. Para la gestión del código fuente, se utiliza **GitHub** bajo una estrategia de **GitHub Flow**, donde las ramas `main` y `develop` centralizan el código estable, aplicando la convención de **Conventional Commits** para garantizar un historial de cambios legible.

El entorno de desarrollo se ha estandarizado utilizando **Visual Studio Code** para el frontend y **Visual Studio 2026** (o VS Code) para el backend. El stack tecnológico comprende una **Landing Page** construida estrictamente con HTML, CSS y JavaScript puro (Vanilla), sin el uso de librerías de diseño adicionales; una **Web Application** desarrollada con el framework **Vue.js** utilizando **JavaScript** para la interactividad y componentes reactivos; y un **Backend** robusto desarrollado en **C# (.NET 10 y ASP.NET Core)**. La persistencia de datos se maneja en **MySQL 8.0** mediante el ORM **Entity Framework Core**, siguiendo convenciones de nomenclatura y normalización 3FN para las tablas del sistema.

En cuanto a la configuración del despliegue, el equipo ha optado por un ecosistema basado íntegramente en **Amazon Web Services (AWS)**. El frontend y la Landing Page se alojan en buckets de **Amazon S3** distribuidos mediante **Amazon CloudFront** para asegurar baja latencia y certificados SSL vía HTTPS. El backend se despliega sobre **AWS Elastic Beanstalk** (configurado para entornos .NET Core) para aprovechar el autoescalado y balanceo de carga, mientras que la base de datos se gestiona a través de **Amazon RDS (MySQL)**, lo que garantiza respaldos automatizados y alta disponibilidad. Finalmente, se utiliza **GitHub Actions** para automatizar el pipeline de CI/CD, permitiendo que cada integración validada se sincronice de forma inmediata con la infraestructura de nube.

### 5.1.1. Software Development Environment Configuration

En esta sección, se especifican las herramientas y productos de software utilizados por los miembros del equipo para colaborar en todas las fases del ciclo de vida de **SmartLock**. La configuración del entorno de desarrollo asegura la interoperabilidad y consistencia técnica, cubriendo desde la gestión del proyecto hasta el despliegue final en la nube.

| Producto | Categoría | Propósito de uso | Ruta de Referencia / Descarga |
| :--- | :--- | :--- | :--- |
| **Jira Software** | Project & Requirements Management | Gestión del Product Backlog, planificación de Sprints y seguimiento de User Stories. | [Jira Workspace](https://upc-team-open-source.atlassian.net/) |
| **Figma** | Product UX/UI Design | Diseño de Wireframes, Mock-ups y prototipado interactivo de la Web App y Landing Page. | [https://www.figma.com/](https://www.figma.com/) |
| **UXPressia** | Product UX Design | Elaboración de artefactos de diseño de experiencia como User Personas y Journey Maps. | [https://uxpressia.com/](https://uxpressia.com/) |
| **Visual Studio Code** | Software Development | IDE principal para el desarrollo del Frontend (Vue.js) y la Landing Page (HTML/CSS/JS puro). | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| **Visual Studio 2026** | Software Development | IDE principal para el desarrollo del Backend RESTful API utilizando C# y ASP.NET Core. | [https://visualstudio.microsoft.com/](https://visualstudio.microsoft.com/) |
| **MySQL Workbench** | Software Development | Herramienta para el diseño, modelado y gestión local de la base de datos relacional. | [https://dev.mysql.com/downloads/workbench/](https://dev.mysql.com/downloads/workbench/) |
| **GitHub** | SCM & Software Documentation | Repositorio centralizado de código fuente y documentación técnica del proyecto. | [GitHub Organization](https://github.com/202610-1asi0730-12144-SmartIndustries) |
| **AWS Console** | Software Deployment | Gestión y monitoreo de servicios en la nube (S3, CloudFront, Elastic Beanstalk y RDS). | [https://aws.amazon.com/console/](https://aws.amazon.com/console/) |
| **Swagger / OpenAPI** | Software Documentation | Documentación interactiva y pruebas de los servicios web RESTful del backend. | Integrado en ASP.NET Core. |

### 5.1.2. Source Code Management

En esta sección, el equipo establece los medios y el esquema de organización que aplicará para el seguimiento de modificaciones durante el ciclo de vida de **SmartLock**. Para ello, utilizamos **GitHub** como plataforma centralizada y sistema de control de versiones.

A continuación, se presentan los enlaces a la organización y los 4 repositorios que conforman la solución integral:

* **Organización en GitHub:** [https://github.com/202610-1asi0730-12144-SmartIndustries](https://github.com/202610-1asi0730-12144-SmartIndustries)
* **Landing Page:** [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--website](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--website)
* **Frontend Web Application:** [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--webapp](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--webapp)
* **Web Services (Core Backend API):** [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--platform](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--platform)
* **Project Report:** [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--report](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--report)

#### Implementación de GitFlow
Para mantener un flujo de trabajo ordenado, el equipo ha implementado **GitFlow** como *workflow* de control de versiones. Este modelo estructura nuestro trabajo en las siguientes ramas (*branches*):

**Ramas Principales:**
* `main`: Rama principal que contiene el código estable y listo para producción.
* `develop`: Rama de integración donde se fusionan las nuevas características antes de pasar a producción.

**Ramas de Soporte y Convenciones:**
* **Feature branches:** Cada nueva historia de usuario tiene su propia rama. Se crean a partir de `develop` y se fusionan de vuelta en `develop`.
  * *Convención de nombre:* `feature/<descripcion-corta>` (Ejemplo: `feature/qr-generation`).
* **Release branches:** Se utilizan para preparar una nueva versión para producción. Se ramifican desde `develop` y se fusionan en `main` y `develop`.
  * *Convención de nombre:* `release/v<version>` (Ejemplo: `release/v1.1.0`).
* **Hotfix branches:** Destinadas a solucionar errores críticos en producción. Se crean desde `main` y se fusionan en `main` y `develop`.
  * *Convención de nombre:* `hotfix/<descripcion-error>` (Ejemplo: `hotfix/login-crash`).

#### Semantic Versioning (SemVer)
Para nombrar las versiones en nuestras ramas de Release y en los *tags* de producción, aplicamos **Semantic Versioning 2.0.0** (`vMAJOR.MINOR.PATCH`):
* **MAJOR:** Cambios incompatibles en la API.
* **MINOR:** Nuevas funcionalidades retrocompatibles.
* **PATCH:** Corrección de errores retrocompatibles.

#### Conventional Commits
El equipo aplica el estándar **Conventional Commits** en todos los mensajes de los commits para asegurar un historial legible:
* `feat`: Nueva característica (ej. `feat(auth): add login`).
* `fix`: Corrección de un error (ej. `fix(ui): adjust button spacing`).
* `docs`: Modificaciones en documentación (ej. `docs: update repo links`).
* `style`: Cambios de formato que no afectan la lógica.
* `refactor`: Mejora de código sin añadir funciones ni arreglar bugs.
* `test`: Adición o corrección de pruebas.
* `chore`: Mantenimiento y actualización de configuraciones.

### 5.1.3. Source Code Style Guide & Conventions

Para garantizar la mantenibilidad, legibilidad y colaboración eficiente dentro del equipo **SmartIndustries**, se han adoptado guías de estilo y convenciones de codificación internacionales. Como regla mandatoria, **toda la nomenclatura (clases, métodos, variables, comentarios y documentación) se realiza estrictamente en inglés**.

#### A. HTML & CSS (Google HTML/CSS Style Guide)
Se siguen las recomendaciones de la *Google HTML/CSS Style Guide* para la Landing Page, asegurando un marcado limpio:
* **HTML:** Uso de etiquetas semánticas, indentación de 2 espacios y estructuración modular.
* **CSS:** Al tratarse de CSS puro (Vanilla), se utiliza la metodología BEM (Block Element Modifier) o nomenclaturas en **kebab-case** para nombres de clases (ej. `.access-button-primary`). Se implementan variables nativas de CSS (`--primary-color`) para facilitar la mantenibilidad visual.

#### B. JavaScript & Vue.js (Vue.js Style Guide)
Para el desarrollo de la Web Application, se aplican las guías oficiales de Vue.js:
* **Componentes:** Uso de *Single-File Components* (`.vue`). Los nombres de los componentes se escriben en `PascalCase` (ej. `UserDashboard.vue`).
* **Variables/Métodos:** Uso de `camelCase` para la lógica en JavaScript.
* **Directivas:** Uso de abreviaturas consistentes para las directivas de Vue (ej. `:` para `v-bind` y `@` para `v-on`).

#### C. C# & ASP.NET Core (Microsoft C# Coding Conventions)
El backend sigue las convenciones oficiales de codificación de Microsoft para C# y .NET:
* **Clases y Métodos:** Uso de `PascalCase` (ej. `AccessPolicyController`, `GenerateQrCode()`).
* **Variables Locales y Parámetros:** Uso de `camelCase`.
* **Interfaces:** Siempre deben estar prefijadas con la letra "I" (ej. `IAccessService`).
* **Estructura:** Se implementa inyección de dependencias nativa de .NET y se hace uso de *Data Annotations* y *Fluent API* (Entity Framework Core) para la validación de modelos y diseño de la base de datos.
* **Documentación:** El código debe incluir *XML Documentation Comments* (`///`) para métodos públicos complejos.

#### D. Gherkin (Readable Specifications)
Para la definición de los criterios de aceptación en las historias de usuario, se sigue la sintaxis de **Gherkin** (Given-When-Then), asegurando que las especificaciones sean legibles tanto para el equipo técnico como para los stakeholders.

---

### 5.1.4. Software Deployment Configuration

La estrategia de despliegue de **SmartLock** se basa en un modelo de **Integración y Despliegue Continuo (CI/CD)** utilizando **GitHub Actions**, lo que permite que cada cambio validado en la rama `main` se publique automáticamente en la infraestructura de **Amazon Web Services (AWS)**.

#### Ecosistema de Despliegue
| Producto | Entorno de Hosting | Tecnología de Despliegue |
| :--- | :--- | :--- |
| **Landing Page** | Github Pages | Estático (HTML/CSS/JS puro) con CDN para baja latencia. |
| **Frontend Web App** | Amazon S3 & CloudFront | Vue.js Build (`dist` folder) con certificados SSL. |
| **Web Services** | Amazon Elastic Beanstalk | Entorno .NET Core con autoescalado y balanceo de carga. |
| **Database** | Amazon RDS (MySQL) | Instancia gestionada con backups automáticos. |

#### Pasos para el Despliegue Satisfactorio

1.  **Build Local & Testing:** El desarrollador valida el código localmente ejecutando pruebas (xUnit para C#, Vitest/Jest para Vue).
2.  **Push a GitHub:** Se realiza el *push* a la rama de funcionalidad y se abre un Pull Request hacia `develop`.
3.  **CI Pipeline (GitHub Actions):** * Se dispara un flujo de trabajo que restaura dependencias y compila el proyecto (`dotnet publish` para el backend C#, `npm run build` para la app Vue.js).
    * Se ejecutan las pruebas automatizadas. Si alguna falla, el despliegue se detiene de forma preventiva.
4.  **Deployment (Frontend & Landing Page):** Una vez aprobada la fusión a `main`, los archivos estáticos de la Landing Page y los compilados de Vue.js se sincronizan con los respectivos buckets de **Amazon S3**. Se invalida la caché de **CloudFront** para que los usuarios vean los cambios inmediatamente.
5.  **Deployment (Backend):** El paquete compilado del proyecto ASP.NET Core se envía a **AWS Elastic Beanstalk**. El servicio gestiona el balanceo de carga y aprovisiona el entorno Windows/Linux para ejecutar el servidor Kestrel subyacente.
6.  **Verificación:** Se realiza una prueba de humo (*smoke test*) en los endpoints expuestos en producción para asegurar la conectividad con **Amazon RDS** utilizando Entity Framework Core.

## 5.2. Landing Page, Services & Applications Implementation

En esta sección se detalla y evidencia el proceso continuo de implementación, pruebas de software, documentación técnica y despliegue en la nube de los componentes de la solución: Landing Page, RESTful Web Services y Frontend Web Applications. A partir de la priorización establecida en el Product Backlog, el desarrollo se ha estructurado mediante iteraciones ágiles, garantizando que tanto los procesos *core* del negocio (validación de accesos) como los procesos de soporte (autenticación) sean construidos y desplegados progresivamente aplicando principios de *Responsive Web Design*.

### 5.2.1. Sprint 1

En esta sección se registra y explica el avance obtenido durante el primer ciclo de desarrollo (Sprint 1), abarcando tanto la construcción de los productos de software iniciales como el trabajo colaborativo del equipo. Se incluyen los detalles de planificación, los líderes de cada aspecto, el backlog comprometido y las evidencias de ejecución, documentación y despliegue del trabajo completado.

#### 5.2.1.1. Sprint Planning 1

El Sprint Planning Meeting marcó el inicio formal del desarrollo del código de SmartLock. Durante esta sesión, el equipo de desarrollo junto al Product Owner seleccionaron las Historias de Usuario más prioritarias del Product Backlog para definir el objetivo central de la iteración. A continuación, se presenta el cuadro resumen con los detalles y acuerdos de esta reunión:

| **Sprint #** | Sprint 1 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2026-04-21 |
| **Time** | 19:00 PM |
| **Location** | Reunión virtual (Microsoft Teams) |
| **Prepared By** | Peñaranda Caldas, Gabriel Augusto |
| **Attendees (to planning meeting)** | Peñaranda Caldas, Gabriel Augusto / Ayllon Pauccar, Juan David / Bottger Salazar, Johan Karl / Limache Coronel, Imanol Fabrizio |
| **Sprint n – 1 Review Summary** | - |
| **Sprint n – 1 Retrospective Summary** | - |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | **Contexto:** El equipo decidió enfocar el primer esfuerzo de codificación en sentar las bases operativas de la plataforma, desarrollando la Landing Page para presentar el producto y construyendo el sistema central de autenticación y gestión de identidad, lo cual es requisito previo para cualquier operación de acceso físico. <br><br> **Sprint Goal:**<br>*"Our focus is on offering a secure and reliable authentication gateway for the initial users of SmartLock, while establishing the product's digital presence through a responsive Landing Page.*<br>*We believe it delivers a trustworthy onboarding experience to administrators and clear product value proposition to prospective customers.*<br>*This will be confirmed when administrators can successfully register and access the main dashboard, and visitors can navigate the Landing Page features without errors."* |
| **Sprint 1 Velocity** | 30 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos y desarrollar los módulos de autenticación básicos). |
| **Sum of Story Points** | 29 Story Points. |

#### 5.2.1.2. Aspect Leaders and Collaborators

En esta sección se presenta la **Leadership-and-Collaboration Matrix (LACX)**. Esta matriz detalla los líderes (L) y colaboradores (C) para cada aspecto clave del Sprint, asegurando una comunicación clara y una distribución de responsabilidades eficiente para el proyecto **SmartLock**. La organización está directamente relacionada con la selección de tareas (*tasks*) que se desarrollarán durante el Sprint.

> **Leyenda:** <br>
> **L:** Líder (Responsable de la revisión y entrega del módulo). <br>
> **C:** Colaborador (Apoyo en desarrollo y tareas específicas).

| Team Member (Last Name, First Name) | GitHub Username | Arquitectura & DB | Backend API & Seguridad | Frontend (Landing & Web App) | QA & Deployment |
| :--- | :--- | :---: | :---: | :---: | :---: |
| Peñaranda Caldas, Gabriel Augusto | gapc2124 | L | C | C | C |
| Ayllon Pauccar, Juan David | JuanDPAUC | C | L | C | C |
| Bottger Salazar, Johan Karl | johan-bottger | C | C | L | C |
| Limache Coronel, Imanol Fabrizio | ImaLi06 | C | C | C | L |

#### 5.2.1.3. Sprint Backlog 1

Durante el primer sprint, el equipo se centró en desarrollar una landing page que fuera tanto atractiva como funcional, organizando y distribuyendo tareas en el tablero de Sprint de acuerdo con las habilidades de cada integrante.

* **Enlace al Backlog del Proyecto:** [Tablero Jira - SmartLock](https://upc-team-open-source.atlassian.net/jira/software/projects/SMAR/boards/1)

##### **Sprint 1 - Tareas Asignadas**

| **User Story** |  | **Work-Item / Task** |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Id** | **Título** | **Id** | **Título** | **Descripción** | **Est. (Hrs)** | **Asignado** | **Status** |
| HU-01 | Inicio de sesión estándar | T-01 | Diseñar formulario login | Crear interfaz responsive de login con email y contraseña | 3 | Gabriel | Done |
| HU-01 | Inicio de sesión estándar | T-02 | Implementar endpoint autenticación | Crear endpoint backend para validación de credenciales | 4 | Johan | Done |
| HU-01 | Inicio de sesión estándar | T-03 | Manejo de errores login | Mostrar mensajes amigables para credenciales inválidas | 2 | Gabriel | Done |
| HU-23 | Reset de contraseña | T-04 | Crear pantalla recuperación | Diseñar formulario de recuperación de contraseña | 2 | Johan | Done |
| HU-23 | Reset de contraseña | T-05 | Configurar envío email | Integrar servicio SMTP/email | 3 | Imanol | Done |
| HU-23 | Reset de contraseña | T-06 | Implementar cambio contraseña | Permitir actualizar contraseña mediante token | 3 | Gabriel | Done |
| HU-26 | Cierre de sesión | T-07 | Implementar logout | Invalidar token y limpiar sesión frontend | 2 | Johan | Done |
| HU-37 | Acceso rápido para clientes | T-08 | Agregar botón login landing | Incorporar botón destacado hacia login | 1 | Juan | Done |
| HU-31 | Navegación fluida por secciones | T-09 | Configurar navegación smooth scroll | Implementar scroll suave entre secciones | 2 | Imanol | Done |
| HU-33 | Botón de acción resaltado | T-10 | Diseñar CTA principal | Crear botón visualmente destacado para demo | 1 | Gabriel | Done |
| HU-34 | Tarjetas de beneficios visuales | T-11 | Crear sección features | Diseñar cards con iconos y descripciones | 4 | Johan | Done |
| HU-35 | Formulario de contacto limpio | T-12 | Diseñar formulario contacto | Crear inputs accesibles y botón interactivo | 3 | Juan | Done |
| HU-35 | Formulario de contacto limpio | T-13 | Validación landing page formulario | Validar campos requeridos y formato email | 2 | Imanol | Done |
| HU-36 | Visualización de casos de uso | T-14 | Construir sección casos de uso | Crear bloques organizados por categorías | 3 | Gabriel | Done |
| HU-38 | Tabla de precios comparativa | T-15 | Crear cards pricing | Diseñar tabla comparativa de planes | 4 | Johan | Done |
| HU-39 | Estadísticas de confianza | T-16 | Implementar sección estadísticas | Mostrar métricas destacadas del producto | 2 | Juan | Done |
| HU-40 | Adaptabilidad a pantallas móviles | T-17 | Adaptar grid responsive | Ajustar layouts para pantallas pequeñas | 4 | Gabriel | Done |
| HNF-02 | Rendimiento carga | T-18 | Optimizar assets landing page | Comprimir imágenes y minimizar CSS/JS | 2 | Johan | Done |
| HNF-04 | Datos en tránsito | T-19 | Configurar HTTPS local | Configurar entorno seguro HTTPS/TLS | 1 | Imanol | Done |
| HNF-06 | Diseño Responsivo | T-20 | Validación responsive QA | Verificar comportamiento en móvil/tablet | 2 | Gabriel | Done |
| HNF-10 | Compatibilidad | T-21 | Cross-browser testing | Validar funcionamiento en Chrome, Firefox y Safari | 3 | Johan | Done |
| HNF-13 | Accesibilidad | T-22 | Revisar contraste y labels | Ajustar accesibilidad WCAG básica | 2 | Juan | Done |
| HNF-18 | Mensajes de error | T-23 | Crear componentes error UI | Diseñar mensajes visuales reutilizables | 2 | Imanol | Done |
| HNF-29 | Design System | T-24 | Definir estilos globales | Crear paleta, tipografía y spacing base | 3 | Juan | Done |
| N/A | Configuración general | T-25 | Inicializar repositorio landing page | Configurar estructura base del proyecto landing page | 1 | Imanol | Done |
| N/A | Configuración general | T-26 | Inicializar backend auth | Crear estructura inicial backend autenticación | 2 | Gabriel | Done |
| N/A | Configuración general | T-27 | Configurar base de datos usuarios | Crear tablas iniciales de usuarios y sesiones | 3 | Johan | Done |
| N/A | Configuración general | T-28 | Configurar CI/CD básico | Automatizar build y deploy inicial | 2 | Juan | Done |
| N/A | Configuración general | T-29 | Deploy Landing Page | Publicar landing page en entorno cloud | 2 | Imanol | Done |
| N/A | Configuración general | T-30 | Configurar dominio y DNS | Asociar dominio a landing page | 1 | Gabriel | Done |
| N/A | Configuración general | T-31 | Configurar variables entorno | Gestionar secrets y configuración segura | 1 | Johan | Done |
| N/A | Configuración general | T-32 | Documentación técnica inicial | Crear README y guía setup proyecto | 2 | Juan | Done |
| N/A | Configuración general | T-33 | Sprint QA y testing final | Ejecutar pruebas funcionales integrales | 4 | Imanol | Done |
| **TOTAL HORAS** |  |  |  |  | **78** |  |  |

#### 5.2.1.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 1 fue el desarrollo de la Landing Page institucional del producto, incorporando navegación fluida entre secciones, diseño responsive para dispositivos móviles, tablas comparativas de planes, tarjetas visuales de beneficios, estadísticas de confianza y secciones de casos de uso orientadas a potenciales clientes.
A continuación, se presentan los commits más importantes del Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo del Landing Page.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| smartlock-website | develop | d1e7f8bb5557e48ea7c2e54cde7eb91ec101ac50 | feat: Landing Page development | - | 12-05-2026 |
| smartlock-website | develop | 43b5a493d77dd4809c77b96bdd14e62ad4ff0728 | feat: added Script | - | 14-05-2026 |
| smartlock-website | develop | 55fd6bc2899a113555c20b13eb07e41078879f35 | feat: added landing page header | - | 12-05-2026 |
| smartlock-website | develop | 8782695d930241cd0631d5b4419565efedd5f86d | feat: implementing price section cards and i18 tags | - | 12-05-2026 |

#### 5.2.1.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución de la Landing Page de la aplicación como evidencia. La Landing Page es compuesta por varias secciones que se presentan en las capturas a continuación.

<img src="/Resources/Chapter5/sprint1/execution-evidence1.png"/>
<img src="/Resources/Chapter5/sprint1/execution-evidence2.png"/>
<img src="/Resources/Chapter5/sprint1/execution-evidence3.png"/>

[Execution Evidence Sprint 1 Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210735_upc_edu_pe/IQAICoZ4E8mcQrsknhxiw7YpASuZuy538vsp8p72Yx0w9C8?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=ljd3tg)

#### 5.2.1.6. Services Documentation Evidence for Sprint Review.
No aplica a primer sprint y desarrollo de Landing Page.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.
El despliegue de la Landing Page se realizó en el servicio de Github Pages, se seleccionó esta alternativa debido a la rapidez de despliegue y su sencillez, apropiada para una página estática.
Se incluye la evidencia de despliegue del Landing Page en la plataforma Github Pages: 
[https://202610-1asi0730-12144-smartindustries.github.io/smartlock-website/](https://202610-1asi0730-12144-smartindustries.github.io/smartlock-website/)


<img src="/Resources/Chapter5/sprint1/deployment-evidence1.png"/>
<img src="/Resources/Chapter5/sprint1/deployment-evidence2.png"/>

#### 5.2.1.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 1:

<img src="/Resources/Chapter5/sprint1/collab-insights1.png"/>


### 5.2.2. Sprint 2

En esta sección se registra y explica el avance obtenido durante el segundo ciclo de desarrollo (Sprint 2), abarcando tanto la construcción de los productos de software intermedios como el trabajo colaborativo del equipo. Se incluyen los detalles de planificación, los líderes de cada aspecto, el backlog comprometido y las evidencias de ejecución, documentación y despliegue del trabajo completado.

#### 5.2.2.1. Sprint Planning 2

Durante esta sesión, el equipo de desarrollo junto al Product Owner seleccionaron las Historias de Usuario más prioritarias del Product Backlog para definir el objetivo central de la iteración. A continuación, se presenta el cuadro resumen con los detalles y acuerdos de esta reunión:

| **Sprint #** | Sprint 2 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2026-05-01 |
| **Time** | 19:00 PM |
| **Location** | Reunión virtual (Microsoft Teams) |
| **Prepared By** | Peñaranda Caldas, Gabriel Augusto |
| **Attendees (to planning meeting)** | Peñaranda Caldas, Gabriel Augusto / Ayllon Pauccar, Juan David / Bottger Salazar, Johan Karl / Limache Coronel, Imanol Fabrizio |
| **Sprint 1 Review Summary** | Durante el Sprint 1 el equipo logró completar la primera versión funcional de la Landing Page y del sistema base de autenticación de SmartLock. Se cumplió el objetivo principal del sprint al habilitar un flujo seguro de acceso para administradores y establecer la presencia digital inicial del producto. |
| **Sprint 1 Retrospective Summary** | a comunicación entre integrantes fue constante y facilitó la integración temprana. Mantener documentación y estándares técnicos actualizados durante el sprint. |
| **Sprint Goal & User Stories** | |
| **Sprint 2 Goal** | **Contexto:** **Sprint Goal:**<br>*"Our focus is on delivering the first operational version of the SmartLock Web Application while improving the quality, usability, and stability of artifacts created during Sprint 1.*<br>*We believe this delivers a more complete digital experience to administrators and prospective customers by providing the first functional version of the Frontend Web Application.*<br>*This will be confirmed when users can access the deployed web application, navigate the improved Landing Page without usability issues, and interact successfully with the first administrative frontend modules in a production-like environment."* |
| **Sprint 1 Velocity** | 30 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos y desarrollar los módulos de autenticación básicos). |
| **Sum of Story Points** | 29 Story Points. |

#### 5.2.2.2. Aspect Leaders and Collaborators

En esta sección se presenta la **Leadership-and-Collaboration Matrix (LACX)**. Esta matriz detalla los líderes (L) y colaboradores (C) para cada aspecto clave del Sprint, asegurando una comunicación clara y una distribución de responsabilidades eficiente para el proyecto **SmartLock**. La organización está directamente relacionada con la selección de tareas (*tasks*) que se desarrollarán durante el Sprint.

> **Leyenda:** <br>
> **L:** Líder (Responsable de la revisión y entrega del módulo). <br>
> **C:** Colaborador (Apoyo en desarrollo y tareas específicas).

| Team Member (Last Name, First Name) | GitHub Username | Arquitectura & DB | Backend API & Seguridad | Frontend (Landing & Web App) | QA & Deployment |
| :--- | :--- | :---: | :---: | :---: | :---: |
| Peñaranda Caldas, Gabriel Augusto | gapc2124 | L | C | C | C |
| Ayllon Pauccar, Juan David | JuanDPAUC | C | L | C | C |
| Bottger Salazar, Johan Karl | Deskjobo | C | C | L | C |
| Limache Coronel, Imanol Fabrizio | ImaLi06 | C | C | C | L |

#### 5.2.2.3. Sprint Backlog 2

Durante el segundo sprint, el equipo se centró en desarrollar la primera versión del Web Application funcional, organizando y distribuyendo tareas en el tablero de Sprint de acuerdo con las habilidades de cada integrante.

* **Enlace al Backlog del Proyecto:** [Tablero Jira - SmartLock](https://upc-team-open-source.atlassian.net/jira/software/projects/SMAR/boards/1)

##### **Sprint 2 - Tareas Asignadas**

| **User Story** |  | **Work-Item / Task** |  |  |  |  |  |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Id** | **Título** | **Id** | **Título** | **Descripción** | **Est. (Hrs)** | **Asignado** | **Status** |
| HU-03 | Creación de usuarios | T-01 | Implementar formulario organización | Crear formulario para registrar organizaciones | 4 | Gabriel | Done |
| HU-03 | Creación de usuarios | T-02 | Crear endpoint organizaciones | Implementar API CRUD básico de organizaciones | 5 | Johan | Done |
| HU-03 | Creación de usuarios | T-03 | Validar creación organización | Agregar validaciones frontend y backend | 2 | Juan | Done |
| HU-03 | Creación de usuarios | T-04 | Persistencia organizaciones | Configurar tablas y relaciones básicas en base de datos | 3 | Imanol | Done |
| HU-04 | Asignación de roles | T-05 | Implementar roles básicos | Configurar roles Admin y Staff | 3 | Gabriel | Done |
| HU-04 | Asignación de roles | T-06 | Asociar usuarios a organización | Relacionar usuarios registrados con organizaciones | 4 | Johan | Done |
| HU-19 | Desactivación rápida | T-07 | Implementar desactivación usuario | Permitir activar/desactivar usuarios desde panel | 3 | Juan | Done |
| HU-20 | Gestión de Puertas | T-08 | Crear módulo ingresos | Construir vista básica de registros de ingreso | 4 | Imanol | Done |
| HU-20 | Gestión de Puertas | T-09 | Registrar eventos ingreso | Implementar creación manual de ingresos | 4 | Gabriel | Done |
| HU-20 | Gestión de Puertas | T-10 | Mostrar historial ingresos | Visualizar lista simple de accesos registrados | 3 | Johan | Done |
| HU-40 | Adaptabilidad a pantallas móviles | T-11 | Responsive dashboard | Adaptar panel administrativo a móviles | 4 | Juan | Done |
| HNF-06 | Diseño Responsivo | T-12 | QA responsive frontend | Validar comportamiento responsive general | 2 | Imanol | Done |
| HNF-10 | Compatibilidad | T-13 | Cross-browser testing web app | Validar funcionamiento en navegadores principales | 3 | Gabriel | Done |
| HNF-18 | Mensajes de error | T-14 | Manejo visual errores | Estandarizar mensajes visuales del sistema | 2 | Johan | Done |
| HNF-29 | Design System | T-15 | Extender componentes UI | Reutilizar estilos y componentes globales | 3 | Juan | Done |
| N/A | Configuración general | T-16 | Inicializar frontend web app | Configurar estructura base aplicación web | 2 | Imanol | Done |
| N/A | Configuración general | T-17 | Configurar routing frontend | Implementar navegación protegida | 3 | Gabriel | Done |
| N/A | Configuración general | T-18 | Configurar estado global | Manejar sesión y datos principales | 3 | Johan | Done |
| N/A | Configuración general | T-19 | Deploy Web Application | Desplegar primera versión frontend | 3 | Juan | Done |
| N/A | Configuración general | T-20 | Actualizar Landing Page | Publicar versión corregida y mejorada | 2 | Imanol | Done |
| N/A | Configuración general | T-21 | QA integración final | Ejecutar pruebas funcionales integrales | 4 | Gabriel | Done |
| **TOTAL HORAS** |  |  |  |  | **66** |  |  |

#### 5.2.2.4. Development Evidence for Sprint Review

El principal avance durante el Sprint 2 fue el desarrollo de la primera version del frontend Web Application del producto, incorporando navegación fluida entre secciones, diseño responsive para dispositivos móviles, tablas comparativas de planes, tarjetas visuales de beneficios, estadísticas de confianza y secciones de casos de uso orientadas a potenciales clientes.
A continuación, se presentan los commits más importantes para el Sprint, los cuales muestran el ciclo de vida del proyecto, y toda la información que se usó para el desarrollo.

| Repository | Branch | Commit ID | Message | Body | Commit Date  |
|---|---|---|---|---|---|
| smartlock-webapp | feature/organization-list | 0d0cd05243704ddc8fa6df73c990bef1e7b2fff5 | feat: add json-server | - | 14-05-2026 |
| smartlock-webapp | feature/organization-list | c2f53edacb07b36c15792f75dd9989ad7d9031c5 | feat: add i18n support | - | 14-05-2026 |
| smartlock-webapp | develop | d70f8e8903e5fa33cc2d3a7568fc741a9d37f073 | feat: add base-api and base-endpoint | - | 14-05-2026 |
| smartlock-webapp | develop | 84f82709abf92fae60abb06b80103efcb85ee811 | feat: add environment configuration files | - | 12-05-2026 |

#### 5.2.2.5. Execution Evidence for Sprint Review
Se incluyen capturas detalladas de la ejecución de la primera versión del Frontend Web Application como evidencia.

<img src="/Resources/Chapter5/sprint2/execution-evidence1.png"/>

[Execution Evidence Sprint 2 Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210735_upc_edu_pe/IQB8j7Vc40nyRLf55dGjuPMrAeKZb6mCMAs7I2x7mXQ_xjg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=ySzFKD)


#### 5.2.2.6. Services Documentation Evidence for Sprint Review.
No aplica.

#### 5.2.2.7. Software Deployment Evidence for Sprint Review.
El despliegue de la primera versión del Frontend Web Application se realizó en la plataforma de Amazon S3 y CloudFront.
Se incluye la evidencia de despliegue: 
[https://feature-organization-list.dx10b2ahz129b.amplifyapp.com](https://feature-organization-list.dx10b2ahz129b.amplifyapp.com)


<img src="/Resources/Chapter5/sprint2/deployment-evidence1.png"/>


#### 5.2.2.8. Team Collaboration Insights for Sprint Review
Durante el transcurso de este sprint, todos los miembros participaron de forma activa y constante en la creación de las tareas asignadas. A continuación todos los analíticos que nos proporciona Github, en su apartado de Insights, sobre la colaboración del equipo durante el Sprint 2:

<img src="/Resources/Chapter5/sprint1/collab-insights1.png"/>



## 5.3. Validation Interviews.
### 5.3.1. Diseño de Entrevistas.
### 5.3.2. Registro de Entrevistas.
### 5.3.3. Evaluaciones según heurísticas.

## 5.4. Video About-the-Product.
