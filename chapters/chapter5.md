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
| **Landing Page** | Amazon S3 & CloudFront | Estático (HTML/CSS/JS puro) con CDN para baja latencia. |
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
| **Date** | 2026-04-20 |
| **Time** | 19:00 PM |
| **Location** | Reunión virtual (Microsoft Teams) |
| **Prepared By** | Peñaranda Caldas, Gabriel Augusto |
| **Attendees (to planning meeting)** | Peñaranda Caldas, Gabriel Augusto / Ayllon Pauccar, Juan David / Bottger Salazar, Johan Karl / Limache Coronel, Imanol Fabrizio |
| **Sprint n – 1 Review Summary** | Al ser el primer Sprint de desarrollo, la revisión anterior corresponde a la fase de ideación. Resultados alcanzados: arquitectura C4 finalizada, bases de datos diseñadas y repositorios GitHub configurados. El Product Owner brindó el feedback necesario para iniciar la codificación orientada al dominio. |
| **Sprint n – 1 Retrospective Summary** | Como retrospectiva inicial de la forma de trabajo, el equipo identificó como acierto el uso de diagramas compartidos, pero reconoció como oportunidad de mejora establecer reglas más estrictas de GitFlow para evitar colisiones en los Pull Requests futuros. |
| **Sprint Goal & User Stories** | |
| **Sprint n Goal** | **Contexto:** El equipo decidió enfocar el primer esfuerzo de codificación en sentar las bases operativas de la plataforma, desarrollando la Landing Page para presentar el producto y construyendo el sistema central de autenticación y gestión de identidad, lo cual es requisito previo para cualquier operación de acceso físico. <br><br> **Sprint Goal:**<br>*"Our focus is on offering a secure and reliable authentication gateway for the initial users of SmartLock, while establishing the product's digital presence through a responsive Landing Page.*<br>*We believe it delivers a trustworthy onboarding experience to administrators and clear product value proposition to prospective customers.*<br>*This will be confirmed when administrators can successfully register, log in using 2FA, and access the main dashboard, and visitors can navigate the Landing Page features without errors."* |
| **Sprint n Velocity** | 30 Story Points. (Velocidad estimada basada en la capacidad inicial del equipo para configurar los entornos y desarrollar los módulos de autenticación básicos). |
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

Nuestro objetivo ha sido consolidar el núcleo de seguridad y gestión de identidades del sistema SmartLock. De manera técnica, hemos logrado la implementación de mecanismos de autenticación, aislamiento total de datos por cliente y blindaje contra ataques externos. Con esto, hemos transformado un diseño conceptual en una infraestructura técnica funcional que garantiza que solo las personas correctas tengan acceso a los recursos adecuados, bajo un entorno de comunicación 100% cifrado y seguro. Esperamos que nuestros clientes tengan siempre la certeza de que nuestro producto será 100% confiable y eficiente.

* **Enlace al Backlog del Proyecto:** [Tablero Jira - SmartLock](https://upc-team-open-source.atlassian.net/jira/software/projects/SMAR/boards/1)

##### **Sprint 1 - Tareas Asignadas**

| **User Story** | | **Work-Item / Task** | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Id** | **Título** | **Id** | **Título** | **Descripción** | **Est. (Hrs)** | **Asignado** | **Status** |
| SMAR-33 | Encriptación | T-33-1 | Hash de claves | Programar la función para que las contraseñas se guarden encriptadas en la DB usando Bcrypt. | 4 | Juan | To-Do |
| SMAR-33 | Encriptación | T-33-2 | Pruebas de Login | Verificar que al loguearse, el sistema compare la clave escrita con la encriptada en la DB. | 3 | Juan | To-Do |
| SMAR-34 | Datos en tránsito | T-34-1 | Configuración HTTPS | Configurar el servidor para que la URL use certificados SSL. | 4 | Gabriel | To-Do |
| SMAR-34 | Datos en tránsito | T-34-2 | Redirección Segura | Hacer que si alguien entra por HTTP, la web lo redirija automáticamente a HTTPS. | 2 | Gabriel | To-Do |
| SMAR-45 | Data Isolation | T-45-1 | Campo de Empresa | Agregar la columna "Empresa_Id" en todas las tablas para separar los datos de cada cliente. | 6 | Imanol | To-Do |
| SMAR-45 | Data Isolation | T-45-2 | Filtro de Consultas | Programar la lógica para que un usuario solo pueda ver los registros de su "Empresa_Id". | 8 | Imanol | To-Do |
| SMAR-01 | Login estándar | T-01-1 | Maquetado de Login | Crear la página visual (HTML/CSS) con el formulario de correo y contraseña responsivo. | 5 | Johan | To-Do |
| SMAR-01 | Login estándar | T-01-2 | Conexión Backend | Programar el endpoint que recibe datos del formulario y valida si el usuario existe. | 6 | Johan | To-Do |
| SMAR-03 | Creación usuarios | T-03-1 | Formulario Registro | Diseñar la interfaz para que el Admin pueda ingresar datos de nuevos empleados. | 5 | Gabriel | To-Do |
| SMAR-03 | Creación usuarios | T-03-2 | Guardado Usuario | Crear función que inserta al nuevo usuario validando que el correo no esté repetido. | 5 | Gabriel | To-Do |
| SMAR-04 | Asignación roles | T-04-1 | Tabla de Roles | Crear en la base de datos los niveles (Admin, Staff, Monitor) y asignarlos. | 4 | Johan | To-Do |
| SMAR-04 | Asignación roles | T-04-2 | Control de Accesos | Programar que ciertas páginas o botones solo se activen si se tiene el rol adecuado. | 6 | Johan | To-Do |
| SMAR-23 | Reset de clave | T-23-1 | Envío de Correo | Integrar servicio de AWS para que el sistema envíe mail automático al pedir el reset. | 6 | Imanol | To-Do |
| SMAR-23 | Reset de clave | T-23-2 | Link Temporal | Crear página donde el usuario escriba su nueva clave usando enlace que expire en 1 hora. | 5 | Imanol | To-Do |
| SMAR-26 | Cierre de sesión | T-26-1 | Botón de Salir | Programar la acción que borre los datos de sesión guardados en el navegador. | 2 | Imanol | To-Do |
| SMAR-26 | Cierre de sesión | T-26-2 | Limpieza de Token | Asegurar que el servidor rechace el token anterior una vez que el usuario cerró sesión. | 4 | Imanol | To-Do |
| SMAR-44 | Anti-Brute Force | T-44-1 | Contador Fallos | Programar un contador que identifique si una persona falla su clave más de 5 veces. | 5 | Juan | To-Do |
| SMAR-44 | Anti-Brute Force | T-44-2 | Bloqueo por tiempo | Impedir el acceso a esa cuenta por 15 minutos tras los fallos detectados. | 4 | Juan | To-Do |
| SMAR-51 | Complejidad clave | T-51-1 | Reglas de Clave | Crear validaciones para clave segura (mínimo 8 letras, número y símbolo). | 3 | Gabriel | To-Do |
| SMAR-51 | Complejidad clave | T-51-2 | Mensajes de Error | Mostrar mensajes en rojo al usuario si su clave es muy débil mientras la escribe. | 3 | Gabriel | To-Do |
| SMAR-81 | Manejo Errores | T-81-1 | Pantalla de Error | Crear alerta amigable para cuando el servidor falle, sin mostrar código técnico. | 5 | Johan | To-Do |
| SMAR-81 | Manejo Errores | T-81-2 | Auditoría Interna | Configurar que el sistema guarde un archivo log con los errores reales para revisión. | 4 | Johan | To-Do |
| SMAR-82 | CORS Policy | T-82-1 | Permisos Dominio | Configurar el sistema para que solo acepte peticiones desde tu web oficial. | 3 | Gabriel | To-Do |
| SMAR-82 | CORS Policy | T-82-2 | Cabeceras Seguras | Definir qué acciones HTTP (GET, POST, DELETE) están permitidas. | 3 | Gabriel | To-Do |
| **TOTAL HORAS** | | | | | **105** | | |

## 5.3. Validation Interviews.
### 5.3.1. Diseño de Entrevistas.
### 5.3.2. Registro de Entrevistas.
### 5.3.3. Evaluaciones según heurísticas.

## 5.4. Video About-the-Product.
