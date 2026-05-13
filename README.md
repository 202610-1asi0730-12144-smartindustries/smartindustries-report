<div align="center">

<img src="/Resources/Introduction/UPC/UPC-Logo.png" alt="Logo-UPC" width="180">

# Universidad Peruana de Ciencias Aplicadas
### Facultad de Ingeniería
**Carrera:** Ingeniería de Software

---

## **Informe de Trabajo Final**
### **Proyecto:** SmartLock
**Startup:** SmartTecnologies

**Curso:** Aplicaciones Web (SW61)
**Sección:** 12144
**Ciclo:** 2026-01
**Profesor:** Efraín Ricardo Bautista Ubillús

---

### **Relación de Integrantes**

| Nombre y Apellidos                | Código     |
| :-------------------------------- | :--------- |
| Bottger Salazar, Johan Karl       | u202210735 |
| Limache Coronel, Imanol Fabrizio  | u20231h067 |
| Ayllon Pauccar, Juan David        | u20241a860 |
| Peñaranda Caldas, Gabriel Augusto | u202210836 |

<br>
**Mayo, 2026**
</div>

---
### Registro de Versiones

<div align="center">

| **Versión** | **Fecha** | **Autor** | **Descripción de modificación** |
| :---: | :---: | :--- | :--- |
| **1.0** | 07/04/2026 | Johan Karl Bottger Salazar | Se agregó la estructura inicial del Capítulo I, la carátula, el Startup Profile, antecedentes y problemáticas. |
| **1.1** | 08/04/2026 | Juan David Ayllon Pauccar | Se desarrolló la sección 1.1 del documento. |
| **1.2** | 09/04/2026 | Juan David Ayllon Pauccar | Se redactó la sección 1.2 referente a la solución. |
| **1.3** | 10/04/2026 | Gabriel Augusto Peñaranda Caldas | Se elaboraron las secciones 1.3 y 1.4 del primer capítulo. |
| **1.4** | 11/04/2026 | Gabriel Augusto Peñaranda Caldas | Se finalizó el Capítulo 1 con los puntos restantes. |
| **2.0** | 12/04/2026 | Gabriel Augusto Peñaranda Caldas | Se dio inicio al Capítulo 2 con la redacción de las secciones 2.1 y 2.2. |
| **2.1** | 13/04/2026 | Gabriel Augusto Peñaranda Caldas | Se completó la sección 2.3 correspondiente a User Personas. |
| **2.2** | 14/04/2026 | Imanol Fabricio Limache Coronel | Se elaboró la sección 2.4 (Big Picture Event Storming). |
| **2.3** | 15/04/2026 | Imanol Fabricio Limache Coronel | Se redactó la sección 2.5 completando la etapa de diseño conceptual. |
| **2.4** | 16/04/2026 | Johan Karl Bottger Salazar | Se agregó el Style Guidelines y el Information Architecture. |
| **3.0** | 17/04/2026 | Imanol Fabricio Limache Coronel | Se estructuró y brindó apoyo inicial en la redacción de la sección 3.1. |
| **3.1** | 18/04/2026 | Imanol Fabricio Limache Coronel | Se finalizó la sección 3.1 y se avanzó con la sección 3.2. |
| **3.2** | 19/04/2026 | Johan Karl Bottger Salazar | Se desarrollaron las secciones 3.3 y 3.4 enfocadas en la gestión del proyecto. |
| **3.3** | 20/04/2026 | Imanol Fabricio Limache Coronel | Se finalizó el Capítulo 3 con la redacción de las secciones restantes. |
| **4.0** | 22/04/2026 | Johan Karl Bottger Salazar | Se agregó el diagrama de Clases tanto para Frontend como para Backend. |
| **4.1** | 23/04/2026 | Juan David Ayllon Pauccar | Se elaboró la sección 4.3 del documento técnico. |
| **4.2** | 24/04/2026 | Juan David Ayllon Pauccar | Se completó la sección 4.4 cerrando los requerimientos asignados. |
| **4.2** | 24/04/2026 | Juan David Ayllon Pauccar | Se completó la sección de Sprint 2 |
</div>
<br>

# Project Report Collaboration Insights
**URL de la Organización de GitHub:**
* [SmartIndustries - Organización](https://github.com/202610-1asi0730-12144-SmartIndustries)

---

**URLs de los Repositorios del Proyecto:**

* **Project Report:**
    [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--report](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--report)
* **Software Platform (Backend):**
    [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--platform](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--platform)
* **Web Application (Frontend):**
    [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--webapp](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--webapp)
* **Landing Page Website:**
    [https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--website](https://github.com/202610-1asi0730-12144-SmartIndustries/-SmartLock--website)

---

# Contenido

- [Contenido](#contenido)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
      - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
      - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)
- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
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
  - [2.4. Big Picture Event Storming](#24-big-picture-event-storming)
  - [2.5. Ubiquitous Language](#25-ubiquitous-language)
- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
  - [3.1. User Stories](#31-user-stories)
  - [3.2. Impact Mapping](#32-impact-mapping)
  - [3.3. Product Backlog](#33-product-backlog)
- [Capítulo IV: Product Design](#capítulo-iv-product-design)
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
    - [4.6.1. Design-Level Event Storming](#461-design-level-event-storming)
    - [4.6.2. Software Architecture Context Diagram](#462-software-architecture-context-diagram)
    - [4.6.3. Software Architecture Container Diagrams](#463-software-architecture-container-diagrams)
    - [4.6.4. Software Architecture Components Diagrams](#464-software-architecture-components-diagrams)
  - [4.7. Software Object-Oriented Design](#47-software-object-oriented-design)
    - [4.7.1. Class Diagrams](#471-class-diagrams)
  - [4.8. Database Design](#48-database-design)
    - [4.8.1. Database Diagrams](#481-database-diagrams)
- [Capítulo V: Product Implementation, Validation & Deployment](#capítulo-v-product-implementation-validation--deployment)
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

---

# Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:<br><br>
**ABET – EAC - Student Outcome 3**
Criterio: Capacidad de comunicarse efectivamente con un rango de audiencias.<br><br>
En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 3.<br><br>

<table>
<thead>
<tr>
<th colspan="3"><b>Criterio específico</b></th>
<th colspan="3"><b>Acciones realizadas</b></th>
<th colspan="3"><b>Conclusiones</b></th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="3">Comunica oralmente con efectividad a diferentes rangos de audiencia.</td>
<td colspan="3" align="justify">
<h4>Limache Coronel, Imanol Fabrizio</h4>
 <b>AV1:</b><p>Presentó la arquitectura de eventos (Big Picture) al equipo y a los stakeholders, explicando el flujo de datos de forma clara. Asimismo, dirigió las reuniones de daily scrum y sustentó el backlog del proyecto.</p>
<h4>Peñaranda Caldas, Gabriel Augusto</h4>
 <b>AV1:</b><p>Expuso el modelo de negocio, el proceso de User Personas y la propuesta de valor de SmartLock frente a la clase.</p>
<h4>Palacios Tinoco, Adrian Fernando</h4>
 <b>AV1:</b><p>Detalló los diagramas de clases y la arquitectura de la información durante la revisión del sprint técnico.</p>
<h4>Bottger Salazar, Johan Karl</h4>
 <b>AV1:</b><p>Explicó las secciones introductorias y la justificación de la solución propuesta en el pitch inicial del proyecto.</p>
</td>
<td colspan="3" align="justify">
<h4>Limache Coronel, Imanol Fabrizio</h4>
<b>AV1:</b> Demostró fluidez al explicar conceptos técnicos a un público no técnico y mantuvo una comunicación asertiva para el alineamiento del equipo.<br><br>
<h4>Peñaranda Caldas, Gabriel Augusto</h4>
<b>AV1:</b> Logró captar la atención de la audiencia al articular claramente los beneficios del sistema sin depender de tecnicismos.<br><br>
<h4>Palacios Tinoco, Adrian Fernando</h4>
<b>AV1:</b> Sustentó con seguridad las decisiones de diseño arquitectónico frente a las consultas del jurado calificador.<br><br>
<h4>Bottger Salazar, Johan Karl</h4>
<b>AV1:</b> Comunicó eficazmente el problema inicial y cómo la solución se alinea con los objetivos del cliente.
</td>
</tr>
<tr>
<td colspan="3">Comunica por escrito con efectividad a diferentes rangos de audiencia.</td>
<td colspan="3" align="justify">
<h4>Limache Coronel, Imanol Fabrizio</h4>
 <b>AV1:</b><p>Redactó la documentación del Design-Level Event Storming, documentó la gestión del proyecto en Jira y estructuró el backlog.</p>
<h4>Peñaranda Caldas, Gabriel Augusto</h4>
 <b>AV1:</b><p>Elaboró los perfiles de usuario, el análisis Lean UX y documentó los capítulos iniciales de la propuesta.</p>
<h4>Palacios Tinoco, Adrian Fernando</h4>
 <b>AV1:</b><p>Creó las guías de estilo, diagramas técnicos y manuales de arquitectura de software para el equipo de desarrollo.</p>
<h4>Bottger Salazar, Johan Karl</h4>
 <b>AV1:</b><p>Estructuró y redactó la problemática, los antecedentes y los requerimientos funcionales del sistema.</p>
</td>
<td colspan="3" align="justify">
<h4>Limache Coronel, Imanol Fabrizio</h4>
<b>AV1:</b> Produjo documentación técnica coherente y mantuvo un registro ordenado de la planificación para lectura ágil.<br><br>
<h4>Peñaranda Caldas, Gabriel Augusto</h4>
<b>AV1:</b> Redactó los artefactos de UX y negocio con un nivel de detalle excelente, estructura lógica y ortografía impecable.<br><br>
<h4>Palacios Tinoco, Adrian Fernando</h4>
<b>AV1:</b> Estructuró los diagramas y guías visuales acompañándolos con descripciones precisas y estandarizadas.<br><br>
<h4>Bottger Salazar, Johan Karl</h4>
<b>AV1:</b> Consolidó los antecedentes y requisitos en un texto claro, formal y académicamente riguroso.
</td>
</tr>
</tbody>
</table>

---

# Capítulo I: Introducción
## 1.1. Startup Profile
### 1.1.1. Descripción de la Startup
**Área:** Seguridad Digital y Control de Accesos

**SmartTecnologies** es una startup formada por un equipo de estudiantes de ingeniería de software de la Universidad Peruana de Ciencias Aplicadas (UPC) que nace con la meta de proponer una alternativa moderna a los sistemas de seguridad tradicionales, que muchas veces se quedan cortos en control y trazabilidad. Identificamos que la gestión de llaves físicas y el registro manual de entradas son procesos lentos y poco fiables, por lo que desarrollamos Smart Lock. Nuestra solución es una plataforma web integral que permite administrar y monitorear el ingreso a cualquier espacio físico desde un solo lugar, transformando la seguridad convencional en un sistema inteligente basado en datos y control en tiempo real.

* **Misión:** Nuestra misión en SmartTecnologies es darle a los administradores y dueños de espacios una herramienta tecnológica avanzada que simplifique cómo controlan sus accesos. Con Smart Lock, buscamos que el proceso de decidir quién entra y quién no deje de ser una preocupación, ofreciendo un sistema basado en reglas claras y alertas automáticas que garantice que cada movimiento quede registrado de forma transparente y segura.
<br></br>
* **Visión:** Nos proyectamos como la startup líder en digitalización de accesos dentro de la región, logrando que nuestra tecnología sea el estándar en edificios, oficinas y centros de estudio. Queremos que SmartTecnologies sea sinónimo de modernidad y eficiencia, impulsando una cultura donde la seguridad no sea una barrera, sino un proceso fluido y totalmente automatizado.
<br></br>
* **Valores:**

    * **Seguridad y Confidencialidad:** Como estudiantes de Ingeniería de Software, sabemos que los datos de acceso son críticos. Por eso, nos tomamos muy en serio la protección de la información, usando protocolos de autenticación y cifrado para que solo las personas autorizadas tengan el control.

    * **Precisión en los datos:** Nos comprometemos con la exactitud en la gestión de presupuestos y tareas, asegurando que la información reflejada en la plataforma sea un espejo fiel de la realidad del proyecto.

    * **Innovación aplicada:** No nos conformamos con lo que ya existe. Buscamos aplicar lo aprendido en nuestra formación para integrar funciones como la simulación de flujo sin hardware y reglas de acceso dinámicas que mantengan a Smart Lock a la vanguardia.

    * **Gestión Colaborativa y Simple:** Creemos que la tecnología debe ser fácil de usar. Centralizamos todo en un panel intuitivo para que la comunicación entre administradores y usuarios sea rápida, eliminando complicaciones innecesarias.

    * **Compromiso con la Excelencia:** Trabajamos para que nuestra plataforma soporte las exigencias de un entorno real, ofreciendo una herramienta robusta que aguante el flujo constante de usuarios sin perder fiabilidad.
### 1.1.2. Perfiles de integrantes del equipo

|**Integrante**|**Perfil**|**Imagen**|
|:-------------|----------|:--------:|
| **Juan David Ayllon Pauccar**|"Estudiante de 5to ciclo de Ingeniería de Software en la UPC. Cuento con conocimientos técnicos avanzados en desarrollo con C++, SQL, Python Intermedio, HTML, CSS. Me distingo por ser un integrante responsable y con gran capacidad de comunicación asertiva, facilitando la coordinación y el flujo de trabajo dentro del equipo. Mi compromiso con el proyecto SmartLock se refleja en mi disposición para aprender, resolver desafíos complejos y asegurar que cada entrega cumpla con los estándares esperados."|<img src="/Resources/Chapter1/Students profiles/Juan-David-Ayllon.jpg" width="2000"/>
| **Imanol Fabrizio Limache Coronel**|Soy un estudiante al que le gusta aprender cosas nuevas, sobre todo si se relacionan a la programación, además de la resolución de problemas.|<img src="/Resources/Chapter1/Students profiles/Imanol-Limache.jpeg" width="2000"/>|
| **Johan Karl Bottger Salazar**|Mi nombre es Johan Karl Bottger Salazar, tengo 21 años y estoy estudiando la carrera de ingeniería de software. Tengo experiencia con distintos frameworks de desarrollo de aplicaciones web. Destaco con liderazgo y autonomía. Me comprometo con el logro exitoso del proyecto junto a los integrantes del equipo.|<img src="/Resources/Chapter1/Students profiles/Johan-Bottger.jpg" width="2000"/>|
|**Peñaranda Caldas Gabriel Augusto - u202210836**|Estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas (UPC). Me encuentro llevando cursos de 5to y 6to ciclo de la carrera. Cuento con habilidades sobresalientes en cloud, python, typescript y UX/UI. Además se ser alguien muy preocupado por mis compañeros de equipo y amigable que las demás personas. Me comprometo a que el proyecto **SmartLock** se lleve a cabo con éxito brindando responsabilidad y puntualidad en las entregas y avances del proyecto.|<img src="/Resources/Chapter1/Students profiles/Gabriel-Peñaranda.jpg" alt="Foto de Gabriel Peñaranda Caldas" width="2000"/> |

## 1.2. Solution Profile
### 1.2.1. Antecedentes y problemática

**5W's y 2H's**

Para definir el problema central de Smart Lock, hemos aplicado la técnica de análisis detallado:
<br>

* **What?**
  <br>
  La falta de un sistema centralizado, auditable y seguro para gestionar el ingreso de personal, lo que genera vulnerabilidades en la seguridad física y administrativa.<br><br>


* **Why?**
  <br>
  Porque los sistemas convencionales no ofrecen trazabilidad. No se puede saber con certeza quién entró a una hora específica si no existe un registro digital automático y protegido contra alteraciones. <br><br>

* **Who?**
  <br>
  Administradores de oficinas, gestores de espacios de coworking y dueños de propiedades residenciales o comerciales que carecen de un control estricto sobre sus accesos.<br><br>

* **When?**
  <br>
  El problema se manifiesta diariamente, especialmente en horarios fuera de oficina o durante cambios de turno, donde el control se vuelve crítico y propenso a errores humanos.<br><br>

* **Where?**
  <br>
  En entornos urbanos con alta densidad de oficinas y espacios compartidos donde el flujo de personas es constante y difícil de registrar manualmente.<br><br>

* **How?**
  <br>
  La problemática se agrava mediante el uso de llaves duplicadas sin permiso, el olvido de registros en cuadernos físicos y la incapacidad de revocar accesos de manera inmediata ante una baja de personal.<br><br>

* **How much?**
  <br>
  El costo de una brecha de seguridad o la pérdida de activos por un acceso no autorizado puede ascender a miles de soles, sumado al gasto constante en cerrajería tradicional que representa un flujo de caja ineficiente para las startups y PYMES.

### 1.2.2. Lean UX Process
#### 1.2.2.1. Lean UX Problem Statements
El dominio de nuestro producto es la gestión de seguridad y control de acceso a espacios físicos (Domain). Actualmente, nuestros administradores de edificios, dueños de negocios y personal de seguridad (Customer Segments) sufren por la falta de visibilidad en tiempo real, la dificultad para gestionar permisos temporales o por horarios, y la tediosa tarea de auditar accesos manualmente (Pain Points). Esto genera una brecha significativa de seguridad y eficiencia operativa frente a sistemas tradicionales que son inflexibles o ciegos ante anomalías (Gap).

Nuestra visión es proporcionar a las empresas una plataforma web inteligente y escalable que no solo permita o deniegue el acceso, sino que automatice el monitoreo mediante reglas, alertas y un historial detallado en tiempo real (Vision/Strategy). Para comenzar a validar nuestra solución, nos enfocaremos en un segmento inicial de pequeñas y medianas empresas (pymes) o espacios de coworking que requieran un control estricto de horarios para sus empleados sin invertir inicialmente en hardware complejo (Initial Segment).
#### 1.2.2.2. Lean UX Assumptions
**Business Assumptions (Suposiciones del Negocio):**

- Creemos que las empresas están dispuestas a pagar una suscripción mensual recurrente (modelo SaaS) en lugar de un pago único por un software de escritorio tradicional.

- Creemos que la simulación de acceso a puertas será suficiente para convencer a los primeros clientes (early adopters) del valor del software antes de integrarlo con hardware físico.

- Creemos que el límite de usuarios y de historial en el "Plan Básico" será el principal motivador para que los clientes escalen al "Plan Profesional".

**User Assumptions (Suposiciones del Usuario):**

- Creemos que el personal de monitoreo adoptará la verificación de dos pasos (2FA) sin considerarlo un bloqueo para su productividad.

- Creemos que los administradores valoran más recibir alertas automáticas (ej. intentos fallidos o fuera de horario) que revisar un historial de registros de forma manual.
#### 1.2.2.3. Lean UX Hypothesis Statements
- Hipótesis 1 (Alertas): Creemos que reduciremos el tiempo de respuesta ante incidentes de seguridad en un 50% si el personal de monitoreo logra identificar anomalías instantáneamente usando el sistema de alertas por intentos fallidos repetidos o accesos fuera de horario.

- Hipótesis 2 (Gestión de roles): Creemos que aumentaremos la adopción del Plan Profesional si los administradores de recursos humanos logran automatizar la entrada de su personal usando el control de acceso segmentado por franjas horarias y días laborales.

- Hipótesis 3 (Seguridad): Creemos que las empresas confiarán la auditoría de sus instalaciones a nuestra plataforma si los auditores internos logran rastrear exactamente quién autorizó un ingreso usando el historial detallado de eventos y la autenticación segura (2FA).

#### 1.2.2.4. Lean UX Canvas

| 1. Business Problem | 2. Business Outcomes |
| :------------------ | :------------------- |
| Las empresas pierden tiempo y vulneran su seguridad gestionando accesos con métodos inflexibles o sin monitoreo en tiempo real. | - Conseguir suscripciones al Plan Básico/Pro.<br>- Alta retención mensual.<br>- Reducción de incidentes de seguridad de los clientes. |
| **3. Users / Customers** | **4. User Benefits** |
| - Administradores de instalaciones / RRHH.<br>- Personal de monitoreo / Prevención.<br>- Empleados (usuarios finales). | - Tranquilidad al tener control total de quién entra y cuándo.<br>- Ahorro de tiempo en auditorías.<br>- Alertas automáticas sin esfuerzo manual. |
| **5. Solutions / Ideas** | **6. Hypotheses** |
| - Panel en tiempo real.<br>- Sistema de reglas por horario y roles.<br>- Motor de alertas de anomalías.<br>- Log de auditoría inmutable. | - Creemos que reduciremos el tiempo de respuesta ante incidentes en un 50% si el personal logra identificar anomalías usando las alertas automáticas.<br>- Creemos que aumentaremos la adopción del Plan Pro si RRHH logra automatizar la entrada usando el control por franjas horarias. |
| **7. What's the most important thing to learn first?** | **8. What's the least amount of work we need to do to learn this? (MVP)** |
| ¿Los administradores confiarán en la gestión de permisos a través de una interfaz web antes de conectar hardware real? | Construir la plataforma web funcional con la función de **Simulación de acceso a puertas** para demostrar el flujo lógico a clientes potenciales. |
### 1.3. Segmentos objetivo
---

Para el desarrollo de **Smart Lock**, se han definido los siguientes segmentos objetivo, integrando sus perfiles, necesidades y comportamientos en la gestión de accesos:

| **Segmento** | **Descripción del Perfil** | **Necesidades Principales** | **Características Psicográficas y Comportamentales** |
| :--- | :--- | :--- | :--- |
| **Gerentes de Operaciones, TI y Seguridad Corporativa** | Líderes responsables de una empresa preocupada por la infraestructura y seguridad de sus espacios de trabajo, desde startups en crecimiento hasta corporativos con múltiples oficinas y alto flujo de personal. | - Centralizar el control de accesos de múltiples sedes en una sola plataforma.<br>- Eliminar la vulnerabilidad de las llaves físicas y tarjetas clonables.<br>- Automatizar el registro de asistencia y la revocación inmediata de permisos a gran escala. | - Priorizan la escalabilidad y la integración con herramientas SaaS existentes.<br>- Toman decisiones basadas en datos y registros de auditoría inmutables.<br>- Buscan máxima eficiencia operativa reduciendo el error humano en porterías. |
| **Administradores de Eventos y Espacios de Alto Tráfico** | Profesionales encargados de la logística en centros de convenciones, ferias o complejos de oficinas que requieren gestionar entradas masivas por periodos específicos. | - Creación rápida de credenciales digitales temporales para invitados o contratistas.<br>- Monitoreo en tiempo real de la ocupación por zonas para evitar aglomeraciones.<br>- Despliegue del sistema sin depender de instalaciones de hardware pesadas o fijas. | - Valoran la agilidad y la capacidad de respuesta inmediata ante incidentes.<br>- Están familiarizados con protocolos de seguridad dinámica (2FA y alertas móviles).<br>- Prefieren interfaces intuitivas que permitan delegar tareas de control de forma sencilla. |

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### **Kisi (Control de Acceso en la Nube)**
Es una solución global de gestión de accesos de nivel empresarial que centraliza el control de múltiples instalaciones en una única interfaz basada en la nube. Se especializa en modernizar infraestructuras existentes sin necesidad de reemplazarlas por completo.
<https://www.getkisi.com/enterprise>

#### **Características Principales**
* **Gestión de Identidad Avanzada:** Permite asignar privilegios detallados por usuario e integra sistemas de autenticación **SSO** y protocolos **SCIM** para sincronizar la base de datos de empleados automáticamente.
* **Seguridad y Auditoría:** Facilita el cumplimiento de normativas de seguridad física mediante la obtención de datos vía **API** y la generación de informes automáticos personalizados.
* **Seguridad Multicapa:** Ofrece opciones de autenticación de dos factores (**2FA**) y **WebAuthn** para elevar los estándares de protección.
* **Implementación Híbrida:** Su gran diferencial es la capacidad de conectarse a cerraduras y lectores ya instalados, lo que reduce los costos de implementación hasta en un **65%**.

#### **Estructura de Planes**

| Plan | Descripción / Enfoque | Ideal para |
| :--- | :--- | :--- |
| **Standard** | Control básico en la nube. | Oficinas pequeñas. |
| **CRM** | Integración con sistemas de gestión de clientes. | Negocios con membresías. |
| **Enterprise** | Auditorías estrictas e integraciones de IT avanzadas. | Grandes corporaciones. |

---
<https://pages.getkisi.com/hubfs/kisi-pricing-overview.pdf>
<br>

### **Acceso Total Perú (Soluciones Integrales de Automatización)**
**Perfil de la Empresa:** Empresa peruana en fase de expansión con más de 5 años de experiencia en el sector de seguridad inteligente. Su competitividad radica en la flexibilidad de hardware y una sólida trayectoria con instituciones públicas y privadas de alto perfil (MININTER, MINCETUR, UNI, entre otros).

#### **Líneas de Servicio y Planes**
* **Control de Acceso para Puertas:** Sistema versátil con soporte para múltiples métodos de validación: códigos, tarjetas, huellas biométricas, reconocimiento facial y **códigos QR**.
* **Gestión de Asistencia Biométrica:** Solución especializada para **Recursos Humanos** que permite el control detallado de asistencias, faltas y horas extras con gestión local o centralizada.
* **Control de Acceso Vehicular:** Automatización de entradas y salidas de vehículos enfocada en la eficiencia operativa y reducción de costos de personal.
* **Control Peatonal Centralizado:** Implementación de barreras físicas (**torniquetes o molinetes**) gestionadas por un software integrado e intuitivo para flujos masivos.

#### **Valor Agregado**

| Beneficio | Descripción |
| :--- | :--- |
| **Asesoría Personalizada** | Acompañamiento técnico previo para determinar la viabilidad según la infraestructura. |
| **Experiencia Local** | Conocimiento profundo del mercado peruano y cumplimiento de estándares para entidades estatales. |

---
<https://accesototalperu.com/control-de-acceso-puerta/>
<br>

### **Kronos por SEIDOR (Gestión de Fuerza Laboral y Tiempo)**
**Descripción General:** Solución de alto nivel distribuida por **SEIDOR**, diseñada para el control integral de la jornada laboral y la optimización de la productividad. Su enfoque principal es el cumplimiento normativo y la eficiencia operativa en empresas con grandes planillas y turnos complejos.

#### **Pilares Estratégicos**
* **Optimización de Costos Operativos:** Alinea el personal con la demanda del negocio. Controla el pago de **horas extras** y proyecta el gasto de horas-hombre en tiempo real mediante alertas automáticas.
* **Mitigación de Riesgos y Cumplimiento:** Automatiza la generación de horarios asegurando el cumplimiento de la **legislación laboral** y acuerdos sindicales. Valida que el personal cuente con certificaciones vigentes antes de asignar turnos.
* **Productividad y Rendimiento:** Gestiona descansos obligatorios para prevenir el agotamiento y facilita la creación de equipos basados en competencias específicas.
* **Experiencia del Empleado (Self-Service):** Interfaz intuitiva para dispositivos móviles (**iOS y Android**) que permite a los colaboradores gestionar su disponibilidad y preferencias de turnos.

#### **Resumen de Valor**

| Enfoque | Objetivo Principal |
| :--- | :--- |
| **Financiero** | Control de presupuestos y reducción de sobrecostos laborales. |
| **Legal** | Automatización del cumplimiento de normativas vigentes. |
| **Humano** | Autogestión y bienestar del colaborador mediante movilidad. |

---
<https://www.seidor.com/es-pe/kronos>
<br>


### 2.1.1. Análisis Competitivo

#### Competitive Analysis Landscape

<div align="justify">

> **¿Por qué llevar a cabo el desarrollo de un software de gestión de accesos habiendo modelos internacionales que gestionan la seguridad a nivel empresarial?**
> 
> **Objetivo:** El objetivo de nuestro equipo es que los clientes vean nuestro software como una aplicación viable para la gestión de accesos de sus eventos o empresas, pudiendo ver reportes de asistencias, tardanzas e identificación de usuarios. Asimismo, facilitar la visualización de reportes que permitan analizar estadísticamente a sus colaboradores.

| Sección | Detalle | SmartLock <br><img src="/Resources/Chapter2/Companies/SmartLock.png" alt="SmartLock" width="100"/> | Kisi <br><img src="/Resources/Chapter2/Companies/Kisi.png" alt="kisi" width="100"/> | Acceso total Peru <br><img src="/Resources/Chapter2/Companies/Atp.png" alt="Acceso-total-peru" width="100"/> | Kronos por Seidor <br><img src="/Resources/Chapter2/Companies/Seidor.jpg" alt="Kronos" width="100"/> |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Perfil** | Overview | Es un modelo de gestión de accesos "Asset-Light" que utiliza códigos QR dinámicos para eliminar la inversión en hardware, orientado a empresas y eventos que buscan una implementación inmediata, económica y escalable. | Es una solución de seguridad física basada en la nube que unifica el control de múltiples sedes globales en una sola interfaz, optimizando los costos de instalación al integrar infraestructura antigua con protocolos modernos de identidad (SSO/SCIM). | Se especializa en la integración de hardware y soporte técnico local, ofreciendo sistemas de barreras físicas y biometría para instituciones que requieren una fiscalización presencial estricta y cumplimiento de normativas nacionales. | Es una plataforma de Workforce Management estratégica enfocada en grandes corporaciones, cuyo objetivo es maximizar la rentabilidad del capital humano mediante la automatización de horarios complejos y el control de costos laborales. |
| | Ventaja competitiva (¿Qué valor ofrece?) | Optimiza la gestión de identidades mediante un modelo SaaS basado en códigos QR dinámicos, eliminando la dependencia de hardware costoso para ofrecer una solución ágil y de bajo costo en accesos corporativos y eventos temporales. | Se posiciona como una solución de control de accesos en la nube de nivel empresarial, cuyo objetivo es modernizar infraestructuras físicas antiguas integrándolas con sistemas de identidad avanzados como SSO y SCIM. | Se especializa en la integración de hardware y automatización local, enfocándose en la instalación de barreras físicas y sistemas biométricos para instituciones que requieren un control presencial robusto en el mercado peruano. | Ofrece una plataforma estratégica de Workforce Management, diseñada para grandes corporaciones que buscan maximizar la productividad y garantizar el cumplimiento legal mediante la gestión compleja de turnos y planillas. |
| **Perfil de Marketing** | Mercado objetivo | Se dirige a PYMES, startups y productoras de eventos que buscan una solución de acceso "ligera" y digital, priorizando la agilidad sobre la infraestructura física. | Su mercado son empresas tecnológicas y corporativos globales con múltiples sedes que necesitan centralizar la seguridad física en la nube e integrarla con su stack de IT (SSO/SCIM). | Enfocado en el sector público, industrial y educativo nacional, donde se requiere una fiscalización presencial estricta y soluciones de hardware robustas (torniquetes y biometría). | Orientada a grandes corporaciones con operaciones complejas (retail, manufactura, salud) que gestionan miles de empleados y requieren un control riguroso de normativas laborales. |
| | Estrategias de marketing | Basada en marketing digital, resaltando la facilidad de configuración, el ahorro en hardware y la flexibilidad del modelo por uso o suscripción. | Se posiciona mediante Inbound Marketing especializado en IT, ofreciendo contenido técnico sobre ciberseguridad física y eficiencia operativa para gerentes de tecnología y seguridad. | Utiliza una estrategia de ventas consultivas y licitaciones, apoyándose en su historial con el Estado y testimonios de grandes instituciones locales para generar confianza técnica. | Emplea un enfoque de ABM y eventos corporativos de alto nivel, posicionándose como un aliado estratégico para la transformación digital de Recursos Humanos. |
| **Perfil de Producto** | Productos & Servicios | Software de generación de QR dinámicos, panel de administración para gestión de planillas y módulos específicos para el control de asistencia en eventos masivos. | Controladores inteligentes de puertas, lectores compatibles con smartphones y una plataforma centralizada que integra autenticación de dos factores (2FA) con sistemas de oficina existentes. | Venta e instalación de terminales biométricos, molinetes y barreras vehiculares, acompañados de software de gestión local y servicios de mantenimiento preventivo. | Suite integral de Workforce Management que incluye módulos de planificación de horarios, control de fatiga, gestión de certificados y autoservicio para el empleado. |
| | Precios & Costos | Modelo de suscripción mensual escalable (SaaS) o pago por evento, eliminando los costos iniciales de instalación y mantenimiento de hardware especializado. | Estructura de precios por niveles (Standard, CRM, Enterprise) que combina una tarifa de software recurrente con el costo de adquisición de sus controladores propietarios. | Modelo de venta directa de activos (CAPEX) con un costo inicial alto por equipo e instalación, sumado a contratos opcionales de soporte técnico y licencias locales. | Inversión de nivel Enterprise que incluye costos significativos de consultoría, implementación personalizada y licencias anuales por volumen de empleados gestionados. |
| | Canales de distribución | Distribución 100% digital mediante plataforma Web para administración y App móvil nativa para que los usuarios finales validen sus accesos mediante QR. | Canal híbrido que utiliza plataforma Web para control global y aplicaciones móviles que emplean Bluetooth/NFC para la apertura de puertas físicas. | Distribución mediante ventas directas y consultoría presencial, utilizando interfaces de software locales (On-premise) o centralizadas para el monitoreo de hardware. | Ecosistema multi-dispositivo con interfaz Web robusta para la gestión administrativa y aplicaciones móviles (iOS/Android) enfocadas en la autogestión de turnos por el personal. |
| **Análisis SWOT** | Fortalezas | Su modelo "Asset-Light" basado en QR dinámicos elimina la inversión en hardware, permitiendo una implementación inmediata y costos operativos mínimos. | Excelente capacidad de integración híbrida, permitiendo gestionar infraestructuras antiguas desde una plataforma en la nube de nivel global. | Sólida presencia local y soporte técnico presencial, lo que les otorga una ventaja competitiva en licitaciones con el Estado y sector industrial. | Capacidad inigualable para gestionar cumplimiento legal y optimización de nómina en entornos corporativos con turnos altamente complejos. |
| | Debilidades | La dependencia total de la conectividad y batería del smartphone del usuario puede generar fricción en puntos de acceso de alta criticidad. | El costo de adquisición sigue siendo elevado debido a la necesidad de sus controladores propietarios para centralizar el mando. | Su modelo de negocio depende excesivamente de la venta e instalación de activos físicos (CAPEX), lo que dificulta una escalabilidad rápida. | Posee una curva de aprendizaje muy alta y procesos de implementación extremadamente largos y costosos para el cliente promedio. |
| | Oportunidades | Existe un mercado masivo en la digitalización de PYMES y eventos temporales que buscan seguridad profesional sin contratos de mantenimiento pesados. | El crecimiento del trabajo híbrido impulsa la demanda de soluciones que permitan gestionar oficinas desde cualquier parte del mundo. | Expansión hacia soluciones de ciudades inteligentes y automatización de edificios en el mercado inmobiliario peruano en auge. | La creciente regulación sobre el control de horas trabajadas y bienestar laboral obliga a las grandes empresas a adoptar sistemas tan robustos como este. |
| | Amenazas | La entrada de gigantes del software que integren funciones de acceso gratuitas en sus ecosistemas de oficina (como Microsoft o Google). | Startups con tecnologías puramente móviles (NFC/Bluetooth) que eliminan la necesidad de cualquier hardware intermedio. | El rechazo progresivo a los métodos de contacto físico (biometría de huella) frente a tecnologías de reconocimiento remoto o digital. | Herramientas de gestión de proyectos y comunicación que están añadiendo módulos de control de tiempo (Time Tracking) mucho más intuitivos. |
</div>

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

Para validar la propuesta de valor de **SmartLock**, se diseñaron entrevistas dirigidas a dos segmentos clave: **empresarios (dueños o administradores de negocios)** y **organizadores de eventos**, quienes enfrentan problemáticas relacionadas con el control de accesos y la seguridad en sus espacios.

El objetivo de estas entrevistas es comprender sus necesidades, problemas actuales, comportamientos y nivel de interés en una solución digital de control de accesos.

---

#### Segmento 1: Empresarios (dueños o administradores)

> **Objetivo:** Entender cómo gestionan actualmente el acceso a sus instalaciones, identificar problemas de seguridad y evaluar su disposición hacia soluciones digitales.

**Cuestionario de validación:**

1.  ¿Cómo gestionas actualmente el acceso de personas a tu negocio o instalaciones?
2.  ¿Qué tipo de problemas has tenido relacionados con el control de accesos?
3.  ¿Utilizas algún sistema digital o todo es manual? ¿Por qué?
4.  ¿Qué tan importante es para ti saber quién entra y sale en tiempo real?
5.  ¿Has tenido alguna situación de acceso no autorizado? ¿Cómo la manejaste?
6.  ¿Qué tan complicado es actualmente revocar el acceso a exempleados o terceros?
7.  ¿Qué herramientas utilizas para llevar un registro de accesos?
8.  ¿Cuánto tiempo inviertes en gestionar o supervisar estos accesos?
9.  ¿Qué características considerarías esenciales en un sistema de control de accesos?
10. ¿Estarías dispuesto a pagar por una solución que automatice este proceso? ¿Por qué?
11. ¿Qué nivel de confianza te generaría un sistema basado en la nube?
12. ¿Qué tan importante es para ti recibir alertas automáticas ante accesos sospechosos?
13. ¿Qué tan fácil debería ser implementar una solución como esta en tu negocio?
14. ¿Prefieres una solución sin hardware inicial (solo software)? ¿Por qué?
15. ¿Qué te haría decidirte por usar una plataforma como SmartLock?

---

#### Segmento 2: Organizadores de eventos

> **Objetivo:** Explorar cómo gestionan accesos en eventos, identificar dificultades operativas y validar oportunidades de mejora mediante tecnología.

**Cuestionario de validación:**

1.  ¿Cómo gestionas el ingreso de personas en los eventos que organizas?
2.  ¿Qué problemas has enfrentado al controlar accesos en eventos?
3.  ¿Cómo verificas la identidad o autorización de los asistentes?
4.  ¿Qué tan frecuente es que ocurran errores o accesos no autorizados?
5.  ¿Utilizas herramientas digitales para el control de ingreso? ¿Cuáles?
6.  ¿Qué tan importante es para ti tener un registro de asistencia en tiempo real?
7.  ¿Cómo manejas cambios de último momento en listas de invitados?
8.  ¿Qué tan complicado es coordinar el acceso con tu equipo de trabajo?
9.  ¿Has tenido problemas con sobreaforo o control de capacidad?
10. ¿Qué funcionalidades te gustaría tener en un sistema de control de accesos para eventos?
11. ¿Qué tan útil sería recibir alertas en tiempo real durante un evento?
12. ¿Estarías dispuesto a usar una plataforma web para gestionar accesos? ¿Por qué?
13. ¿Qué tan importante es la rapidez en el proceso de ingreso de asistentes?
14. ¿Qué te preocupa más: seguridad, rapidez o experiencia del usuario?
15. ¿Qué mejoras implementarías en tu proceso actual de control de accesos?

### 2.2.2. Registro de entrevistas

En esta sección se consolidan las seis entrevistas realizadas para la validación de la propuesta de valor de SmartLock. Cada sesión ha sido documentada para asegurar la trazabilidad de los hallazgos y la construcción de nuestros arquetipos.

| Nombre del Entrevistado | Edad | Distrito | Segmento | Captura de Video | Enlace de la Entrevista (Stream) | Tiempo de Inicio | Tiempo de Fin | Duración |
| :--- | :---: | :--- | :--- | :---: | :--- | :---: | :---: | :---: |
| Almendra Lucía Lavi | 21 | La Molina | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista1.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=0id4Mb) | 00:00 | 09:10 | 09:10 |
| Leugim Sajor | 32 | Surco | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista2.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=a2Ghfv) | 09:10 | 15:40 | 06:30 |
| Evelyn Jannet Caldas | 48 | Ate | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista3.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=uTUBUB) | 15:40 | 29:10 | 13:30 |
| Larissa Teofilo | 28 | Surco | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista4.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=CY27NN) | 29:10 | 35:50 | 06:40 |
| Hugo Rojas O. | 72 | La Molina | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista5.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=Ypp2WU) | 35:50 | 47:00 | 11:10 |
| Hugo Ricardo Rojas P. | 35 | Ate | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista6.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=Pw5K7G) | 47:00 | 55:20 | 08:20 |

---

### 2.2.3. Análisis de entrevistas

A continuación, se presenta un análisis detallado de cada una de las sesiones de validación. En este apartado se describen los comportamientos detectados, los puntos de dolor específicos, rasgos de personalidad y la recepción de la propuesta de valor de SmartLock.

#### Segmento: Organizadores de Eventos

**1. Almendra Lucía Lavi Cuyubamba**
Almendra, de 21 años, es estudiante de la carrera de Marketing en la USIL y organizadora de eventos corporativos en la empresa Okawa. De personalidad extrovertida, detallista y muy dinámica, siempre busca la eficiencia y la mejor experiencia para sus asistentes. Suele organizar sus eventos llevando un conteo de registros en Google Forms, pero no tiene una manera ágil de asegurarse que la persona registrada tenga permiso real de ingreso. Esto le genera aglomeraciones cerca de la hora de inicio. Le parece innovadora la idea de SmartLock para controlar el aforo en tiempo real y estaría dispuesta a usarlo si los beneficios superan el precio, prefiriendo que la solución abarque tanto una app web como móvil.

**2. Leugim Sajor**
Leugim, de 32 años y residente en el distrito de Surco, es un ciudadano extranjero que organiza eventos exclusivos para el sector inmobiliario, donde se presentan proyectos y se atraen nuevos clientes. Posee una personalidad analítica, diplomática y muy estructurada, lo que le ha permitido mantener un negocio muy estable con pocos problemas operativos. Su principal necesidad es mantener la exclusividad y privacidad de las presentaciones inmobiliarias. SmartLock le resulta muy atractivo para gestionar invitaciones VIP con códigos QR temporales, asegurando un ingreso fluido que esté a la altura del perfil de sus clientes de alto poder adquisitivo.

**3. Evelyn Jannet Caldas Párraga**
Evelyn, de 48 años y graduada de Administración en la UPC, es secretaria y organizadora de eventos en el colegio Norteamericano Abraham Lincoln. Tiene una personalidad metódica, resolutiva y con un alto sentido del control y la seguridad. Gestiona accesos a eventos institucionales utilizando plataformas como Joinnus. Su mayor problema es la logística con proveedores y los cambios de personal de último minuto que requieren verificaciones manuales y demoran el proceso. Evelyn tiene una clara preferencia por soluciones 100% en la nube (SaaS), rechazando el hardware por costos. Le atraen las alertas automáticas de acceso denegado y la generación de reportes de asistencia para optimizar la seguridad contable.

---

#### Segmento: Empresarios (Dueños/Administradores)

**4. Larissa Teofilo**
Larissa, de 28 años y residente en Surco, forma parte de la directiva y gerencia de una exitosa cadena de gimnasios brasileños en el país. De personalidad carismática, observadora y muy orientada al servicio al cliente, ella misma confiesa no ser una experta en el apartado tecnológico, pero es sumamente consciente de los defectos del mismo cuando los sistemas actuales de los gimnasios fallan (como tarjetas perdidas o huellas que no leen). SmartLock le parece una excelente iniciativa para modernizar el ingreso de los socios a través de sus propios celulares, reduciendo las quejas en recepción y mejorando la percepción de innovación de la marca.

**5. Hugo Rojas Olivera**
Hugo, de 72 años y residente en La Molina, es médico pediatra graduado y con maestría por la UNMSM, y actualmente se desempeña como gerente del Hospital de Emergencias de Villa El Salvador. Posee una personalidad serena, reflexiva, empática y con una profunda vocación de servicio. Lidera una institución crítica que utiliza un software nacional que presenta múltiples defectos, lo que a menudo contribuye a la saturación del hospital en áreas de control y recepción. Para Hugo, una herramienta como SmartLock podría ser vital para agilizar el flujo de personal médico y administrativo, mitigando los cuellos de botella tecnológicos que actualmente padecen.

**6. Hugo Ricardo Rojas P.**
Hugo, de 35 años y residente del distrito de Ate, es ingeniero ambiental graduado de la Universidad Nacional Agraria La Molina (UNALM) y gerente de la empresa Gestam Consulting. Tiene una personalidad directa, práctica, resolutiva y muy orientada a la protección de los activos de su empresa. Actualmente tiene problemas serios de seguridad para revocar el acceso a exempleados, por lo que necesita una solución inmediata. Es tajante en mencionar que no invertiría en la instalación de hardware físico. Para él, una membresía económica de SmartLock basada puramente en software es la solución perfecta, destacando la importancia de los reportes periódicos de asistencia.

---

#### Síntesis de hallazgos (Insights principales)

* **Insight 1 (Rechazo a la infraestructura física):** La mayoría de los perfiles empresariales entrevistados rechazan la inversión y mantenimiento de hardware nuevo debido a sus altos costos, destacando casos puntuales como el de Hugo Ricardo Rojas y Evelyn Caldas. Por este motivo, la propuesta de SmartLock basada en el modelo SaaS y el uso de dispositivos móviles propios (BYOD) es el principal gatillador de interés, junto con la posibilidad de visualizar el aforo en tiempo real.
* **Insight 2 (Gestión crítica de identidades y exclusiones):** Más allá de registrar asistencias, el problema central radica en la invalidación de accesos. Empresarios como Hugo R. Párraga necesitan revocar permisos a exempleados en tiempo real, mientras que organizadores como Almendra y Leugim necesitan asegurar la identidad del asistente para evitar intrusiones.
* **Insight 3 (Carencias en los sistemas tradicionales):** La mayoría de los entrevistados reporta fricciones graves con sus sistemas actuales (desde software hospitalario saturado hasta registros manuales en papel). Existe una necesidad latente por un software que priorice la rapidez y la facilidad de implementación sin barreras tecnológicas complejas.

### 2.2.1. Diseño de entrevistas

Para validar la propuesta de valor de **SmartLock**, se diseñaron entrevistas dirigidas a dos segmentos clave: **empresarios (dueños o administradores de negocios)** y **organizadores de eventos**, quienes enfrentan problemáticas relacionadas con el control de accesos y la seguridad en sus espacios.

El objetivo de estas entrevistas es comprender sus necesidades, problemas actuales, comportamientos y nivel de interés en una solución digital de control de accesos.

---

#### Segmento 1: Empresarios (dueños o administradores)

> **Objetivo:** Entender cómo gestionan actualmente el acceso a sus instalaciones, identificar problemas de seguridad y evaluar su disposición hacia soluciones digitales.

**Cuestionario de validación:**

1.  ¿Cómo gestionas actualmente el acceso de personas a tu negocio o instalaciones?
2.  ¿Qué tipo de problemas has tenido relacionados con el control de accesos?
3.  ¿Utilizas algún sistema digital o todo es manual? ¿Por qué?
4.  ¿Qué tan importante es para ti saber quién entra y sale en tiempo real?
5.  ¿Has tenido alguna situación de acceso no autorizado? ¿Cómo la manejaste?
6.  ¿Qué tan complicado es actualmente revocar el acceso a exempleados o terceros?
7.  ¿Qué herramientas utilizas para llevar un registro de accesos?
8.  ¿Cuánto tiempo inviertes en gestionar o supervisar estos accesos?
9.  ¿Qué características considerarías esenciales en un sistema de control de accesos?
10. ¿Estarías dispuesto a pagar por una solución que automatice este proceso? ¿Por qué?
11. ¿Qué nivel de confianza te generaría un sistema basado en la nube?
12. ¿Qué tan importante es para ti recibir alertas automáticas ante accesos sospechosos?
13. ¿Qué tan fácil debería ser implementar una solución como esta en tu negocio?
14. ¿Prefieres una solución sin hardware inicial (solo software)? ¿Por qué?
15. ¿Qué te haría decidirte por usar una plataforma como SmartLock?

---

#### Segmento 2: Organizadores de eventos

> **Objetivo:** Explorar cómo gestionan accesos en eventos, identificar dificultades operativas y validar oportunidades de mejora mediante tecnología.

**Cuestionario de validación:**

1.  ¿Cómo gestionas el ingreso de personas en los eventos que organizas?
2.  ¿Qué problemas has enfrentado al controlar accesos en eventos?
3.  ¿Cómo verificas la identidad o autorización de los asistentes?
4.  ¿Qué tan frecuente es que ocurran errores o accesos no autorizados?
5.  ¿Utilizas herramientas digitales para el control de ingreso? ¿Cuáles?
6.  ¿Qué tan importante es para ti tener un registro de asistencia en tiempo real?
7.  ¿Cómo manejas cambios de último momento en listas de invitados?
8.  ¿Qué tan complicado es coordinar el acceso con tu equipo de trabajo?
9.  ¿Has tenido problemas con sobreaforo o control de capacidad?
10. ¿Qué funcionalidades te gustaría tener en un sistema de control de accesos para eventos?
11. ¿Qué tan útil sería recibir alertas en tiempo real durante un evento?
12. ¿Estarías dispuesto a usar una plataforma web para gestionar accesos? ¿Por qué?
13. ¿Qué tan importante es la rapidez en el proceso de ingreso de asistentes?
14. ¿Qué te preocupa más: seguridad, rapidez o experiencia del usuario?
15. ¿Qué mejoras implementarías en tu proceso actual de control de accesos?

### 2.2.2. Registro de entrevistas

En esta sección se consolidan las seis entrevistas realizadas para la validación de la propuesta de valor de SmartLock. Cada sesión ha sido documentada para asegurar la trazabilidad de los hallazgos y la construcción de nuestros arquetipos.

| Nombre del Entrevistado | Edad | Distrito | Segmento | Captura de Video | Enlace de la Entrevista (Stream) | Tiempo de Inicio | Tiempo de Fin | Duración |
| :--- | :---: | :--- | :--- | :---: | :--- | :---: | :---: | :---: |
| Almendra Lucía Lavi | 21 | La Molina | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista1.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=0id4Mb) | 00:00 | 09:10 | 09:10 |
| Leugim Sajor | 32 | Surco | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista2.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=a2Ghfv) | 09:10 | 15:40 | 06:30 |
| Evelyn Jannet Caldas | 48 | Ate | Organizador | ![Captura](/Resources/Chapter2/interviews/entrevista3.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=uTUBUB) | 15:40 | 29:10 | 13:30 |
| Larissa Teofilo | 28 | Surco | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista4.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=CY27NN) | 29:10 | 35:50 | 06:40 |
| Hugo Rojas O. | 72 | La Molina | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista5.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=Ypp2WU) | 35:50 | 47:00 | 11:10 |
| Hugo Ricardo Rojas P. | 35 | Ate | Empresario | ![Captura](/Resources/Chapter2/interviews/entrevista6.jpeg) | [Ver Video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210836_upc_edu_pe/IQA6jpKKXFtsSbTrA9FoQNMJAYrLkhuEY2yz_XDPp9MF6d4?e=Pw5K7G) | 47:00 | 55:20 | 08:20 |

---

### 2.2.3. Análisis de entrevistas

A continuación, se presenta un análisis detallado de cada una de las sesiones de validación. En este apartado se describen los comportamientos detectados, los puntos de dolor específicos, rasgos de personalidad y la recepción de la propuesta de valor de SmartLock.

#### Segmento: Organizadores de Eventos

**1. Almendra Lucía Lavi Cuyubamba**
Almendra, de 21 años, es estudiante de la carrera de Marketing en la USIL y organizadora de eventos corporativos en la empresa Okawa. De personalidad extrovertida, detallista y muy dinámica, siempre busca la eficiencia y la mejor experiencia para sus asistentes. Suele organizar sus eventos llevando un conteo de registros en Google Forms, pero no tiene una manera ágil de asegurarse que la persona registrada tenga permiso real de ingreso. Esto le genera aglomeraciones cerca de la hora de inicio. Le parece innovadora la idea de SmartLock para controlar el aforo en tiempo real y estaría dispuesta a usarlo si los beneficios superan el precio, prefiriendo que la solución abarque tanto una app web como móvil.

**2. Leugim Sajor**
Leugim, de 32 años y residente en el distrito de Surco, es un ciudadano extranjero que organiza eventos exclusivos para el sector inmobiliario, donde se presentan proyectos y se atraen nuevos clientes. Posee una personalidad analítica, diplomática y muy estructurada, lo que le ha permitido mantener un negocio muy estable con pocos problemas operativos. Su principal necesidad es mantener la exclusividad y privacidad de las presentaciones inmobiliarias. SmartLock le resulta muy atractivo para gestionar invitaciones VIP con códigos QR temporales, asegurando un ingreso fluido que esté a la altura del perfil de sus clientes de alto poder adquisitivo.

**3. Evelyn Jannet Caldas Párraga**
Evelyn, de 48 años y graduada de Administración en la UPC, es secretaria y organizadora de eventos en el colegio Norteamericano Abraham Lincoln. Tiene una personalidad metódica, resolutiva y con un alto sentido del control y la seguridad. Gestiona accesos a eventos institucionales utilizando plataformas como Joinnus. Su mayor problema es la logística con proveedores y los cambios de personal de último minuto que requieren verificaciones manuales y demoran el proceso. Evelyn tiene una clara preferencia por soluciones 100% en la nube (SaaS), rechazando el hardware por costos. Le atraen las alertas automáticas de acceso denegado y la generación de reportes de asistencia para optimizar la seguridad contable.

---

#### Segmento: Empresarios (Dueños/Administradores)

**4. Larissa Teofilo**
Larissa, de 28 años y residente en Surco, forma parte de la directiva y gerencia de una exitosa cadena de gimnasios brasileños en el país. De personalidad carismática, observadora y muy orientada al servicio al cliente, ella misma confiesa no ser una experta en el apartado tecnológico, pero es sumamente consciente de los defectos del mismo cuando los sistemas actuales de los gimnasios fallan (como tarjetas perdidas o huellas que no leen). SmartLock le parece una excelente iniciativa para modernizar el ingreso de los socios a través de sus propios celulares, reduciendo las quejas en recepción y mejorando la percepción de innovación de la marca.

**5. Hugo Rojas Olivera**
Hugo, de 72 años y residente en La Molina, es médico pediatra graduado y con maestría por la UNMSM, y actualmente se desempeña como gerente del Hospital de Emergencias de Villa El Salvador. Posee una personalidad serena, reflexiva, empática y con una profunda vocación de servicio. Lidera una institución crítica que utiliza un software nacional que presenta múltiples defectos, lo que a menudo contribuye a la saturación del hospital en áreas de control y recepción. Para Hugo, una herramienta como SmartLock podría ser vital para agilizar el flujo de personal médico y administrativo, mitigando los cuellos de botella tecnológicos que actualmente padecen.

**6. Hugo Ricardo Rojas P.**
Hugo, de 35 años y residente del distrito de Ate, es ingeniero ambiental graduado de la Universidad Nacional Agraria La Molina (UNALM) y gerente de la empresa Gestam Consulting. Tiene una personalidad directa, práctica, resolutiva y muy orientada a la protección de los activos de su empresa. Actualmente tiene problemas serios de seguridad para revocar el acceso a exempleados, por lo que necesita una solución inmediata. Es tajante en mencionar que no invertiría en la instalación de hardware físico. Para él, una membresía económica de SmartLock basada puramente en software es la solución perfecta, destacando la importancia de los reportes periódicos de asistencia.

---

#### Síntesis de hallazgos (Insights principales)

* **Insight 1 (Rechazo a la infraestructura física):** la mayoria de los perfiles empresariales aceptan la inversión y mantenimiento de hardware nuevo, excepto por Hugo Rojas. Sin embargo, La propuesta de SmartLock basada en el modelo SaaS y uso de dispositivos móviles propios (BYOD) es el principal gatillador de interés junto con el aforo en tiempo real.
* **Insight 2 (Gestión crítica de identidades y exclusiones):** Más allá de registrar asistencias, el problema central radica en la invalidación de accesos. Empresarios como Hugo R. Párraga necesitan revocar permisos a exempleados en tiempo real, mientras que organizadores como Almendra y Leugim necesitan asegurar la identidad del asistente para evitar intrusiones.
* **Insight 3 (Carencias en los sistemas tradicionales):** La mayoría de los entrevistados reporta fricciones graves con sus sistemas actuales (desde software hospitalario saturado hasta registros manuales en papel). Existe una necesidad latente por un software que priorice la rapidez y la facilidad de implementación sin barreras tecnológicas complejas.

## 2.3. Needfinding

En esta sección, el equipo explica y presenta los artefactos resultantes del proceso de análisis de la información recolectada en las fases previas. A partir del estudio competitivo frente a alternativas como Kisi o Acceso Total Perú, y tras el análisis de las entrevistas a nuestros segmentos objetivo, comprobamos que existe una fuerte resistencia a la inversión en hardware físico y una clara insatisfacción con los sistemas tradicionales o manuales. La necesidad principal de los usuarios radica en obtener una solución ágil, centralizada en la nube (SaaS) y orientada al uso de dispositivos móviles (BYOD) que permita validar identidades, controlar aforos y revocar accesos en tiempo real. 

Para traducir estos *insights* y puntos de dolor en requerimientos de diseño y de negocio para **SmartLock**, en este apartado se incluyen las secciones de *User Personas, User Task Matrix, User Journey Maps, Empathy Mapping, As-is Scenario Mapping, Big Picture Event Storming* y *Ubiquitous Language*. Estas herramientas nos permiten empatizar a profundidad con el entorno operativo de nuestros arquetipos (el gerente corporativo y la organizadora de eventos), asegurando que la arquitectura y la experiencia de usuario del software resuelvan directamente las fricciones descubiertas.

### 2.3.1. User Personas

En esta sección se presentan las fichas de **User Persona** desarrolladas para los dos segmentos clave de **SmartLock**. La creación de estos arquetipos no es arbitraria; surge directamente del análisis de las entrevistas realizadas y del estudio de la competencia (Kisi, Acceso Total y Kronos). 

De las entrevistas, identificamos que la principal fricción es la **dependencia de registros manuales y hardware costoso**, lo que nos llevó a priorizar la agilidad y la movilidad en nuestros perfiles. Del análisis competitivo, detectamos un vacío en soluciones **"Asset-Light"** para PYMES y eventos, lo que define las metas de nuestros personajes: eficiencia sin inversión pesada en infraestructura.

Para la elaboración de estos artefactos, se utilizó la herramienta **UXPressia**, asegurando que cada ficha incluya dimensiones demográficas, psicográficas, metas, frustraciones y el entorno tecnológico del usuario.

---

#### Segmento 1: Gerentes de Operaciones y TI

##### **Carlos Ortega - "El Protector Eficiente"**

Carlos representa nuestro segmento B2B corporativo. Es el tomador de decisiones que busca transformar la seguridad de su edificio en un activo estratégico basado en datos y no solo en llaves físicas.

![User Persona - Carlos Ortega](/Resources/Chapter2/docs/Carlos%20Ortega.png)

**Resumen del Perfil:**
* **Relación con el problema:** Sufre por la falta de trazabilidad en los accesos de su edificio de oficinas. Su mayor temor es una brecha de seguridad que no pueda auditar.
* **Características Clave:** * **Metas:** Centralizar el control de múltiples sedes y automatizar reportes de asistencia para RRHH.
    * **Frustraciones:** El costo de reposición de tarjetas/llaves y la lentitud de los procesos manuales.
    * **Tecnología:** Usuario avanzado de herramientas SaaS y monitoreo móvil constante.

---

#### Segmento 2: Organizadores de Eventos y Espacios de Alto Tráfico

##### **Valeria Rios - "La Productora Perfeccionista"**

Valeria representa el segmento dinámico de SmartLock. Su necesidad no es la permanencia, sino la velocidad y la seguridad temporal masiva durante picos de tráfico.

![User Persona - Valeria Rios](/Resources/Chapter2/docs/Valeria%20Rios.png)

**Resumen del Perfil:**
* **Relación con el problema:** El caos en el ingreso es su mayor enemigo. Necesita un sistema que sea fácil de desplegar (sin hardware pesado) y que garantice que nadie use entradas falsificadas.
* **Características Clave:**
    * **Metas:** Fluidez total en el ingreso masivo y control de aforo en tiempo real por seguridad.
    * **Frustraciones:** Listas de invitados desactualizadas y el fraude con capturas de pantalla de códigos QR estáticos.
    * **Tecnología:** Mobile-first extremo; depende de su smartphone y la nube para coordinar a su staff en terreno.

### 2.3.2. User Task Matrix

En esta sección se presenta el **User Task Matrix**, una herramienta que permite mapear las actividades críticas que nuestros arquetipos realizan para alcanzar sus objetivos de seguridad y gestión. Este artefacto es el resultado directo de la síntesis entre las entrevistas a profundidad y el análisis de la competencia, permitiéndonos identificar qué procesos son rutinarios y cuáles son vitales para el éxito de la operación.

Para este análisis, consideramos a nuestros dos segmentos objetivo representados por:
* **Carlos Ortega:** Gerente de Operaciones (Segmento Corporativo/Oficinas).
* **Valeria Rios:** Organizadora de Eventos (Segmento de Espacios de Alto Tráfico).

A continuación, se detallan las tareas identificadas, evaluando su **Frecuencia (F)** y su **Importancia (I)** en una escala de Bajo, Medio y Alto.

| Tareas (Tasks) | Carlos: Frecuencia | Carlos: Importancia | Valeria: Frecuencia | Valeria: Importancia |
| :--- | :---: | :---: | :---: | :---: |
| Registro de entrada y salida del personal/asistentes | Alta | Alta | Alta | Alta |
| Verificación de identidad en puntos de control | Alta | Alta | Alta | Alta |
| Gestión y entrega de credenciales físicas (llaves, carnets) | Media | Media | Baja | Media |
| Supervisión de la capacidad máxima de los recintos (aforo) | Baja | Media | Alta | Alta |
| Gestión de permisos para visitas o contratistas externos | Media | Alta | Alta | Alta |
| Elaboración de informes de permanencia y puntualidad | Alta | Alta | Baja | Media |
| Eliminación de credenciales de personal que ya no labora | Media | Alta | Baja | Media |
| Respuesta ante intentos de ingreso no autorizados | Baja | Alta | Media | Alta |

#### **Explicación del Cuadro**

Al analizar la matriz, se observan coincidencias estratégicas y diferencias operativas marcadas por la naturaleza de cada segmento:

* **Tareas Críticas (Coincidencias):** El **Registro de entrada/salida** y la **Verificación de identidad** son las tareas con mayor frecuencia e importancia para ambos. Esto valida que el núcleo de *SmartLock* debe ser la rapidez y la seguridad en estos puntos de fricción.
* **Diferencias en Frecuencia:** Para Carlos, la **Elaboración de informes** es una tarea de alta frecuencia debido a la necesidad de control administrativo constante (asistencia), mientras que para Valeria es una tarea de baja frecuencia que solo ocurre al cierre del evento. Por otro lado, la **Supervisión de aforo** es crítica y frecuente para Valeria por razones de seguridad civil, mientras que para Carlos es una tarea secundaria.
* **Puntos de Dolor Identificados:** La **Eliminación de credenciales** tiene una importancia Alta para Carlos (evitar que un exempleado ingrese), pero su frecuencia es Media. En el caso de Valeria, la **Gestión de permisos temporales** es constante debido a la naturaleza volátil del staff de eventos, lo que representa una carga operativa mayor que la de una oficina tradicional.

### 2.3.3. User Journey Mapping

En esta sección se presentan los **User Journey Maps (As-Is)** correspondientes a los dos arquetipos de usuarios principales definidos previamente: Carlos Ortega (Gerente de Operaciones) y Valeria Rios (Organizadora de Eventos). 

El objetivo de estos diagramas es ilustrar el *end-to-end journey* de la situación actual que enfrentan ambos perfiles al intentar gestionar la seguridad y el control de accesos **sin contar con una solución tecnológica centralizada como SmartLock**. Se evidencia el proceso tradicional, desde el descubrimiento de la necesidad operativa, pasando por la gestión manual mediante el uso de llaves físicas o listas impresas, hasta las tareas de auditoría post-ingreso. 

A través de estos mapas, se identifican claramente los puntos de fricción (pain points), las frustraciones y las caídas en la experiencia del usuario, justificando así la necesidad de desarrollar nuestra propuesta de valor digital. Cada mapa está directamente vinculado a su ficha de *User Persona* desarrollada en la plataforma UXPressia.

#### A. User Journey Map: Carlos Ortega (Segmento Corporativo)
Este mapa detalla la experiencia diaria de Carlos, quien actualmente depende de un sistema obsoleto basado en llaves físicas, registros manuales en cuadernos de portería y reportes poco fiables. Se ilustra la frustración frente a la pérdida de llaves y la falta de visibilidad en tiempo real sobre el flujo de sus empleados.

![Customer Journey Map - Carlos Ortega](/Resources/Chapter2/docs/Customer%20Carlos.png)

#### B. User Journey Map: Valeria Rios (Segmento de Eventos)
Este mapa ilustra el proceso acelerado y estresante de Valeria durante la organización y ejecución de un evento. Se muestra su recorrido "As-Is", donde la gestión de invitados se realiza mediante listas de Excel impresas, generando lentitud en la validación de identidades, largas colas en la puerta y vulnerabilidad ante falsificaciones.

![Customer Journey Map - Valeria Rios](/Resources/Chapter2/docs/Customer%20Valeria.png)

### 2.3.4. Empathy Mapping

En esta sección, el equipo resume el proceso de elaboración y presenta las capturas de los Empathy Maps realizados en la plataforma UXPressia para cada uno de nuestros User Personas. 

El proceso de elaboración inició con una fase de preparación estratégica, colocando al centro a nuestro User Persona correspondiente. A continuación, procedimos a colocar en cada sección de la herramienta las observaciones debatidas por los miembros del equipo, buscando responder de forma analítica a las siguientes preguntas clave: ¿Con quién estamos empatizando?, ¿Qué necesita hacer?, ¿Qué está diciendo?, ¿Qué está viendo?, ¿Qué está haciendo?, ¿Qué está escuchando? y ¿Cómo se siente y qué piensa? 

Finalmente, logramos identificar los **Pains** (frustraciones y miedos) y **Gains** (beneficios y alegrías) de cada perfil en base a las preguntas fundamentales del modelo: ¿Qué le preocupa?, ¿Qué puede ayudar a resolver sus problemas?, y sobre todo, ¿Qué puede convencerlo de que SmartLock es la alternativa correcta en el mercado?

#### A. Empathy Map: Carlos Ortega (Segmento Corporativo B2B)
El siguiente mapa de empatía ilustra el entorno corporativo de Carlos, resaltando su constante presión por mantener los costos operativos bajos y su frustración ante la pérdida recurrente de llaves físicas o tarjetas de acceso en sus instalaciones.

![Empathy Map - Carlos Ortega](/Resources/Chapter2/docs/Carlos%20Empathy%20map.png)

#### B. Empathy Map: Valeria Rios (Segmento de Eventos)
En este mapa empatizamos con el entorno de alta presión de Valeria. Se destacan sus preocupaciones principales relacionadas con las largas colas en los eventos, la vulnerabilidad ante entradas falsificadas y su necesidad urgente de una solución ágil que no requiera instalación de hardware.

![Empathy Map - Valeria Rios](/Resources/Chapter2/docs/Valeria%20Empathy%20map.png)

### 2.3.5. As-is Scenario Mapping

En esta sección, se desarrollan los **As-is Scenario Maps** para nuestros dos arquetipos de usuario: Carlos Ortega y Valeria Rios. A diferencia del Journey Map, que evalúa el ciclo de vida completo del cliente, esta herramienta nos permite desglosar paso a paso las acciones, pensamientos y emociones de los usuarios frente a un **escenario crítico y específico** dentro de su contexto operativo actual (antes de la implementación de SmartLock).

El mapeo de estos escenarios detalla las fases cronológicas de la situación, lo que el usuario "hace", "piensa" y "siente", permitiendo a nuestro equipo identificar las deficiencias técnicas, los altos costos de resolución y los cuellos de botella que justifican el desarrollo de nuestra plataforma digital.

#### A. As-is Scenario Map: Carlos Ortega (Segmento Corporativo)
**Escenario evaluado:** Gestión de un incidente de seguridad por pérdida de llave o tarjeta maestra.
En este mapa se ilustra el proceso tradicional y reactivo que debe seguir Carlos cuando un empleado reporta la pérdida de su credencial de acceso o cuando un ex-empleado no la devuelve. Se evidencia la ineficiencia de depender de un cerrajero, el alto costo económico del reemplazo de cerraduras físicas y el estrés generado por el tiempo en que las instalaciones quedan vulnerables.

![As-is Scenario Map - Carlos Ortega](/Resources/Chapter2/docs/Carlos-As-is-Scenario.png)

#### B. As-is Scenario Map: Valeria Rios (Segmento de Eventos)
**Escenario evaluado:** Control de acceso y validación de aforo durante la "hora pico" de un evento masivo.
Este escenario detalla el momento más crítico para Valeria: la apertura de puertas de un evento utilizando listas de Excel impresas y validación manual. Se destacan las acciones de su personal de seguridad (staff), la frustración ante la lentitud del proceso, la presión por las largas colas de asistentes y la imposibilidad de tener un conteo real del aforo en tiempo real para reportar a Defensa Civil.

![As-is Scenario Map - Valeria Rios](/Resources/Chapter2/docs/Valeria-As-is-Scenario.png)

## 2.4. Big Picture Event Storming

En esta sección, el equipo introduce y resume el proceso colaborativo realizado para entender el dominio del negocio de **SmartLock**. Durante la sesión, nos enfocamos en identificar los eventos significativos, procesos clave y las relaciones entre ellos, permitiéndonos mapear el flujo completo desde que un usuario solicita un acceso hasta que la cerradura se activa mediante el código QR dinámico.

Esta primera aproximación visual de alto nivel nos permitió explorar el landscape del negocio, exponiendo potenciales problemas de sincronización y validación, así como oportunidades para optimizar la experiencia del usuario final al eliminar la dependencia de hardware físico tradicional.

![Big Picture Event Storming](/Resources/Chapter2/eventStormin/bigpicture.jpeg)

**Explicación de las etapas:**
* **Identificación de Eventos de Dominio:** Plasmamos en color naranja todos los sucesos relevantes (ej. QR generado, Acceso validado).
* **Ordenamiento Cronológico:** Organizamos los eventos en una línea de tiempo para asegurar la coherencia del proceso.
* **Identificación de Hotspots:** Marcamos puntos críticos o dudas técnicas que requieren mayor análisis.
* **Definición de Actores y Sistemas:** Vinculamos los eventos con los usuarios (clientes/visitantes) y sistemas externos (servicios de nube y dispositivos IoT).

## 2.5. Ubiquitous Language

En esta sección se define el **Lenguaje Ubicuo (Ubiquitous Language)** del proyecto, un concepto clave dentro de la arquitectura orientada al dominio (Domain-Driven Design). El objetivo es establecer un vocabulario estandarizado y compartido entre los desarrolladores y los expertos del negocio para evitar ambigüedades. A continuación, se detallan los términos en inglés organizados por sus respectivos contextos (*Bounded Contexts*).

### Identity & Auth Context

**Términos (Terms):**
* **Subscription:** Platform tenant subscription.
* **System User:** Admin/Operator/Auditor who accesses the web platform.
* **Authentication:** Verifying user identity (login + 2FA).
* **Role:** Permission level (Super Admin, Admin, Operator, Auditor).
* **2FA:** Two-factor authentication.
* **Quota:** Usage limits (users, subscription limits).
* **Billing Cycle:** Recurring payment period.
* **Quota Warning:** Alert when reaching usage limits.
* **User Lock:** Account lockout after failed attempts.

---

### Physical Space Context

**Términos (Terms):**
* **Location:** Physical site/office where doors are installed.
* **Door:** Physical entry point with access control.
* **Access Mode:** How door grants access (card, biometric, PIN, etc.).
* **Door Status:** Current state of door (open, closed, locked).
* **Maintenance:** Updates/repairs to doors.

---

### Access Control Context

**Términos (Terms):**
* **Access User:** Person who passes through physical doors.
* **Access Policy:** Set of rules defining who can access.
* **Schedule:** Time windows for access (workdays, hours).
* **Holiday Schedule:** Special dates with different access rules.
* **Policy Assignment:** Linking policy to doors/users.
* **Access Attempt:** Any attempt to enter through a door.
* **Access Grant:** Successful access.
* **Access Denial:** Failed access attempt.

---

### Security Context

**Términos (Terms):**
* **Security Alert:** Notification of suspicious/unsafe activity.
* **Access Denial Reason:** Why access was denied (invalid credentials, out of schedule, policy violation).
* **Repeated Failed Attempts:** Multiple failed access attempts.
* **Unauthorized Access:** Access by unauthorized person.
* **Suspicious Behavior:** Activity that violates normal patterns.
* **Emergency Override:** Bypass all security to unlock doors.
* **Alert Acknowledgment:** Operator confirms alert.
* **Alert Resolution:** Alert issue resolved.

---

### Billing & Subscription Context

**Términos (Terms):**
* **Subscription Plan:** Paid tier (Free, Professional, Enterprise).
* **Subscription Upgrade/Downgrade:** Plan level changes.
* **Payment Failure:** Failed billing transaction.
* **Billing Renewal:** Automatic recurring payment.
* **History Archive:** Storing old access logs.
* **Deactivation:** Disabling user/location access.

# Capítulo III: Requirements Specification

## 3.1. User Stories

---

### Historias de Usuario Funcionales (40)

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) | Relacionado con |
| :--- | :--- | :--- | :--- | :--- |
| **HU-01** | Inicio de sesión estándar | Acceso al panel administrativo. | **Dado** que el administrador está en el login, **Cuando** ingresa correo y clave correctos, **Entonces** accede al panel de control. | **EPIC-01** |
| **HU-02** | Autenticación 2FA | Verificación de identidad reforzada. | **Dado** que el personal ingresó clave válida, **Cuando** el sistema procesa el primer paso, **Entonces** solicita código 2FA y valida que no haya expirado. | **EPIC-01** |
| **HU-03** | Creación de usuarios | Registro de empleados/miembros. | **Dado** que el admin de RRHH está en el módulo, **Cuando** ingresa datos requeridos y correo único, **Entonces** el sistema registra al usuario. | **EPIC-02** |
| **HU-04** | Asignación de roles | Gestión de niveles de permiso. | **Dado** que se edita un usuario, **Cuando** se selecciona un rol (Staff/Limpieza), **Entonces** se asignan permisos automáticos del rol. | **EPIC-02** |
| **HU-05** | Acceso días laborales | Restricción por calendario. | **Dado** que el usuario tiene acceso L-V, **Cuando** intenta acceder un sábado, **Entonces** el sistema deniega y registra el evento. | **EPIC-03** |
| **HU-06** | Acceso franjas horarias | Restricción por horas. | **Dado** que el acceso es de 9AM a 6PM, **Cuando** intenta acceder 6:05PM, **Entonces** deniega la entrada y genera registro fallido. | **EPIC-03** |
| **HU-07** | Accesos temporales | Permisos con caducidad. | **Dado** que el permiso vence a las 5:00PM, **Cuando** el reloj marca las 5:01PM, **Entonces** el permiso se revoca automáticamente. | **EPIC-03** |
| **HU-08** | Dashboard Real-Time | Visualización de eventos. | **Dado** que el dashboard está abierto, **Cuando** ocurre un evento en cualquier puerta, **Entonces** aparece en la lista sin recargar la página. | **EPIC-04** |
| **HU-09** | Simulación exitosa | Prueba de flujo sin hardware. | **Dado** que se usa la web sin cerraduras, **Cuando** se simula acceso en puerta permitida, **Entonces** registra evento exitoso en dashboard. | **EPIC-05** |
| **HU-10** | Simulación denegada | Prueba de reglas de negocio. | **Dado** que se usa el simulador, **Cuando** se simula acceso en horario no permitido, **Entonces** genera registro rojo y dispara alertas. | **EPIC-05** |
| **HU-11** | Alerta intentos fallidos | Detección de intrusos. | **Dado** que el sistema está activo, **Cuando** hay >3 fallos en 5 min, **Entonces** genera alerta visual de seguridad. | **EPIC-04** |
| **HU-12** | Alerta fuera de horario | Notificación preventiva. | **Dado** que el monitoreo corre, **Cuando** hay intento de apertura fuera de franja, **Entonces** genera notificación destacada en panel. | **EPIC-04** |
| **HU-13** | Historial detallado | Auditoría de movimientos. | **Dado** que se ingresa a "Historial", **Cuando** carga la vista, **Entonces** muestra lista paginada con usuario, fecha, hora, puerta y estado. | **EPIC-06** |
| **HU-14** | Filtros de historial | Búsqueda avanzada de eventos. | **Dado** que hay miles de registros, **Cuando** se filtra por estado y fecha, **Entonces** la tabla muestra solo los criterios coincidentes. | **EPIC-06** |
| **HU-15** | Límites Plan Básico | Bloqueo por suscripción. | **Dado** que se alcanzó el límite de usuarios, **Cuando** se intenta crear uno nuevo, **Entonces** muestra modal para mejorar al Plan Profesional. | **EPIC-07** |
| **HU-16** | Upgrade Profesional | Escalabilidad de cuenta. | **Dado** que se completa el pago del Plan Profesional, **Cuando** se confirma, **Entonces** elimina límites y desbloquea control avanzado. | **EPIC-07** |
| **HU-17** | Gestión multi-sede | Centralización operativa. | **Dado** que se tiene Plan Empresarial, **Cuando** se accede al panel, **Entonces** permite crear y cambiar entre Sedes independientes. | **EPIC-07** |
| **HU-18** | Reportes avanzados | Análisis de flujo. | **Dado** que se tiene Plan Empresarial, **Cuando** se pide reporte de horas pico, **Entonces** exporta PDF/Excel con gráficas. | **EPIC-06** |
| **HU-19** | Desactivación rápida | Revocación instantánea. | **Dado** que se visualiza lista de empleados, **Cuando** se pulsa "Desactivar", **Entonces** el acceso se revoca en tiempo real en toda la red. | **EPIC-02** |
| **HU-20** | Gestión de Puertas | CRUD de infraestructura. | **Dado** que se configura el espacio, **Cuando** se entra a "Puertas", **Entonces** permite crear, editar y eliminar puntos de acceso. | **EPIC-03** |
| **HU-21** | Acceso por puerta | Permisos granulares. | **Dado** que se edita el rol "Limpieza", **Cuando** se marcan puertas específicas, **Entonces** deniega acceso en el resto de puertas. | **EPIC-03** |
| **HU-22** | Alerta uso indebido | Prevención de espionaje. | **Dado** que hay zonas restringidas, **Cuando** hay intento sin autorización, **Entonces** etiqueta como "Uso indebido" y emite alerta. | **EPIC-04** |
| **HU-23** | Reset de contraseña | Autogestión de cuenta. | **Dado** que el usuario olvidó su clave, **Cuando** la solicita, **Entonces** recibe enlace tokenizado válido por 15 minutos. | **EPIC-01** |
| **HU-24** | Exportación de datos | Descarga de reportes. | **Dado** que se aplicaron filtros en historial, **Cuando** se pulsa "Exportar", **Entonces** descarga CSV con los registros filtrados. | **EPIC-06** |
| **HU-25** | Cierre de alertas | Gestión de incidencias. | **Dado** que hay alerta activa, **Cuando** se pulsa "Resolver", **Entonces** desaparece de la vista y se archiva como resuelta. | **EPIC-04** |
| **HU-26** | Cierre de sesión | Seguridad de terminal. | **Dado** que el usuario está logueado, **Cuando** pulsa "Cerrar sesión", **Entonces** destruye el token y redirige al login. | **EPIC-01** |
| **HU-27** | Invitación masiva | Onboarding eficiente. | **Dado** que se carga lista de correos, **Cuando** se envía, **Entonces** cada empleado recibe link único para crear su clave. | **EPIC-02** |
| **HU-28** | Edición de perfil | Actualización de datos. | **Dado** que el usuario está autenticado, **Cuando** edita su perfil, **Entonces** permite cambiar foto/teléfono pero bloquea cambio de rol. | **EPIC-01** |
| **HU-29** | Alerta desconexión | Monitoreo de hardware. | **Dado** que se monitorea hardware, **Cuando** una puerta pierde red, **Entonces** el ícono en dashboard cambia a "Offline" o rojo. | **EPIC-04** |
| **HU-30** | Notificación crítica | Alerta vía email. | **Dado** que hay notificaciones activas, **Cuando** ocurre emergencia (madrugada), **Entonces** envía email automático al dueño. | **EPIC-04** |
| **HU-31** | Navegación fluida por secciones | **Como** visitante, **quiero** que al pulsar los enlaces del menú la página se deslice suavemente, **para** no perder el hilo de la lectura mientras busco información. | **Dado** que el usuario visualiza la `navbar`, **Cuando** hace clic en un enlace (ej. "Precios"), **Entonces** la pantalla se desplaza con un efecto de scroll suave hasta la sección con el ID `#pricing`. | **EPIC-10** |
| **HU-32** | Selector de idioma visual | **Como** usuario que habla inglés, **quiero** ver un botón claro para cambiar el idioma, **para** entender la propuesta de valor sin tener que usar traductores externos. | **Dado** que el usuario localiza el botón `lang-btn`, **Cuando** lo presiona, **Entonces** todos los textos con el atributo `data-i18n` deben actualizarse visualmente al idioma seleccionado. | **EPIC-11** |
| **HU-33** | Botón de acción resaltado | **Como** interesado en el producto, **quiero** que el botón de "Solicitar Demo" tenga un color llamativo, **para** identificar rápidamente dónde debo registrarme. | **Dado** que el usuario carga el Hero de la página, **Cuando** observa los botones de navegación, **Entonces** el botón `.btn-nav-blue` debe destacar visualmente sobre los enlaces de texto plano. | **EPIC-07** |
| **HU-34** | Tarjetas de beneficios visuales | **Como** usuario curioso, **quiero** ver las ventajas del sistema organizadas en tarjetas con iconos, **para** que la lectura sea ágil y atractiva. | **Dado** que el usuario hace scroll hasta `#features`, **Cuando** revisa las tarjetas `.feat-card`, **Entonces** cada una debe presentar un icono representativo, un título y una descripción breve. | **EPIC-10** |
| **HU-35** | Formulario de contacto limpio | **Como** cliente con dudas, **quiero** un formulario con espacios claros para escribir, **para** enviar mi consulta de forma rápida y sin distracciones visuales. | **Dado** que el usuario llega a la sección `#contact`, **Cuando** interactúa con los campos de texto, **Entonces** el diseño debe mostrar etiquetas legibles y un botón de "Enviar" que reaccione al pasar el cursor (hover). | **EPIC-07** |
| **HU-36** | Visualización de casos de uso | **Como** dueño de un negocio, **quiero** leer ejemplos de aplicación de SmartLock por sectores, **para** visualizar cómo el sistema resolvería mis problemas de seguridad. | **Dado** que el usuario explora la sección `#use-cases`, **Cuando** lee los bloques de contenido, **Entonces** la información debe estar separada visualmente en categorías (ej. Corporativo, Eventos). | **EPIC-10** |
| **HU-37** | Acceso rápido para clientes | **Como** usuario ya registrado, **quiero** un botón de "Iniciar Sesión" bien ubicado, **para** entrar a mi panel de control sin tener que navegar por toda la web. | **Dado** que el usuario está en el menú superior, **Cuando** busca el acceso a la plataforma, **Entonces** el botón `.btn-nav-gray` debe estar claramente diferenciado y llevarlo directo al login. | **EPIC-01** |
| **HU-38** | Tabla de precios comparativa | **Como** comprador consciente, **quiero** comparar los planes y sus precios en columnas, **para** elegir la opción que mejor se adapte a mi presupuesto de un vistazo. | **Dado** que el usuario visualiza la sección `#pricing`, **Cuando** revisa los planes (Básico, Pro, Enterprise), **Entonces** cada tarjeta debe listar sus características con iconos de "check" para facilitar la comparación. | **EPIC-07** |
| **HU-39** | Estadísticas de confianza | **Como** visitante nuevo, **quiero** ver cifras grandes sobre el éxito de la empresa, **para** sentir la seguridad de que SmartLock es una solución probada y confiable. | **Dado** que el usuario carga la página inicial, **Cuando** visualiza la fila `.stats-row`, **Entonces** los números (ej. +500 edificios) deben resaltar por su tamaño de fuente y grosor frente al texto secundario. | **EPIC-10** |
| **HU-40** | Adaptabilidad a pantallas móviles | **Como** usuario que navega desde su celular, **quiero** que todo el diseño se ajuste a lo ancho de mi pantalla, **para** no tener que hacer zoom o scroll horizontal para leer. | **Dado** que se accede a la web desde un smartphone, **Cuando** la resolución es menor a 768px, **Entonces** el menú debe adaptarse (hamburguesa) y los elementos del grid deben apilarse verticalmente. | **EPIC-10** |

---

### Historias de Usuario No Funcionales (30)

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) | Epic Relacionada |
| :--- | :--- | :--- | :--- | :--- |
| **HNF-01** | Latencia Dashboard | Actualización inmediata. | **Dado** que ocurre validación en puerta, **Cuando** la DB registra el evento, **Entonces** actualiza el dashboard en < 1 segundo. | **EPIC-08** |
| **HNF-02** | Rendimiento carga | Carga de plataforma. | **Dado** que se ingresa a la URL, **Cuando** el navegador pide recursos, **Entonces** la página es interactiva en un máximo de 2 segundos. | **EPIC-08** |
| **HNF-03** | Encriptación | Hashing de seguridad. | **Dado** que se crea/cambia clave, **Cuando** se guarda en DB, **Entonces** debe usarse bcrypt y nunca texto plano. | **EPIC-09** |
| **HNF-04** | Datos en tránsito | Cifrado de red. | **Dado** que la web habla con la API, **Cuando** viajan datos sensibles, **Entonces** debe usarse HTTPS con TLS 1.2+. | **EPIC-09** |
| **HNF-05** | Disponibilidad | Continuidad operativa. | **Dado** que el sistema está en producción, **Cuando** se mide el uptime mensual, **Entonces** debe ser >= 99.9%. | **EPIC-08** |
| **HNF-06** | Diseño Responsivo | Adaptabilidad móvil. | **Dado** que se usa un móvil (320px), **Cuando** accede al panel, **Entonces** la interfaz adapta elementos sin pérdida de función. | **EPIC-10** |
| **HNF-07** | Inmutabilidad logs | Integridad de auditoría. | **Dado** que un evento se escribió en DB, **Cuando** un admin intenta borrarlo, **Entonces** la API debe rechazar el UPDATE/DELETE. | **EPIC-06** |
| **HNF-08** | Escalabilidad | Capacidad de carga. | **Dado** que es hora pico (9AM), **Cuando** hay 500 peticiones simultáneas, **Entonces** el servidor responde en < 500ms sin caídas. | **EPIC-08** |
| **HNF-09** | Timeout sesión | Protección por olvido. | **Dado** que la sesión quedó abierta, **Cuando** pasan 15 min sin actividad, **Entonces** destruye sesión y redirige al login. | **EPIC-09** |
| **HNF-10** | Compatibilidad | Multi-navegador. | **Dado** que se usa Chrome/Safari/Firefox, **Cuando** se abre la plataforma, **Entonces** debe renderizar sin fallos visuales ni de consola. | **EPIC-10** |
| **HNF-11** | Tolerancia fallos | Aislamiento de errores. | **Dado** que el simulador tiene un crash, **Cuando** el usuario navega el resto, **Entonces** dashboard e historial siguen operando. | **EPIC-08** |
| **HNF-12** | Velocidad 2FA/Email | Entrega de correos. | **Dado** que se pide 2FA, **Cuando** se dispara solicitud, **Entonces** el correo llega en < 5 segundos a la bandeja del usuario. | **EPIC-08** |
| **HNF-13** | Accesibilidad | Normas WCAG. | **Dado** que se evalúan colores, **Cuando** se mide el contraste, **Entonces** debe cumplir nivel AA de WCAG 2.1. | **EPIC-10** |
| **HNF-14** | Anti-Brute Force | Bloqueo de ataques. | **Dado** que hay ataque de clave, **Cuando** hay 5 fallos en mismo correo, **Entonces** bloquea IP/Cuenta por 30 minutos. | **EPIC-09** |
| **HNF-15** | Data Isolation | Multi-tenancy real. | **Dado** que es un SaaS multi-empresa, **Cuando** un admin consulta, **Entonces** el esquema garantiza que no vea datos de otros clientes. | **EPIC-09** |
| **HNF-16** | Backups diarios | Respaldo de datos. | **Dado** que la info es crítica, **Cuando** es la ventana de mantenimiento, **Entonces** genera backup automático en nube segregada. | **EPIC-09** |
| **HNF-17** | Log de auditoría | Trazabilidad admin. | **Dado** que un admin cambia configuración, **Cuando** se ejecuta, **Entonces** registra quién, cuándo y qué cambió en log oculto. | **EPIC-06** |
| **HNF-18** | Mensajes de error | UX de fallos. | **Dado** que hay fallo de base de datos, **Cuando** la API falla, **Entonces** el frontend muestra mensaje amigable sin detalles técnicos. | **EPIC-10** |
| **HNF-19** | Rate Limiting | Protección de API. | **Dado** que un bot ataca la API, **Cuando** hay >100 req/min desde una IP, **Entonces** el Gateway bloquea con error 429. | **EPIC-09** |
| **HNF-20** | Velocidad Export | Procesamiento masivo. | **Dado** que se exportan 10,000 registros, **Cuando** se procesa, **Entonces** entrega el archivo en < 10 segundos. | **EPIC-08** |
| **HNF-21** | Complejidad clave | Validación de fortaleza. | **Dado** que se configura clave, **Cuando** es débil (1234), **Entonces** rechaza y exige 8 carac., número y símbolo. | **EPIC-09** |
| **HNF-22** | Soporte i18n | Internacionalización. | **Dado** que se desarrolla el código, **Cuando** se implementan textos, **Entonces** se envuelven en i18n para futuras traducciones. | **EPIC-11** |
| **HNF-23** | RTO | Recuperación desastres. | **Dado** que hay desastre total, **Cuando** se activa el DRP, **Entonces** el sistema opera en región secundaria en máximo 4 horas. | **EPIC-08** |
| **HNF-24** | Archivado datos | Cold Storage. | **Dado** que hay millones de registros, **Cuando** un log cumple 2 años, **Entonces** se mueve automáticamente a almacenamiento en frío. | **EPIC-06** |
| **HNF-25** | Consumo batería | Optimización móvil. | **Dado** que el dashboard corre 8h en tablet, **Cuando** se mide consumo, **Entonces** no debe causar drenaje excesivo ni calor. | **EPIC-08** |
| **HNF-26** | Seguridad OWASP | Sanitización de inputs. | **Dado** que hay ataque XSS/SQLi, **Cuando** se envían datos, **Entonces** el backend sanitiza y usa consultas parametrizadas. | **EPIC-09** |
| **HNF-27** | Sincronía NTP | Precisión temporal. | **Dado** que el log tiene valor legal, **Cuando** se registra evento, **Entonces** el servidor usa NTP para sincronía global exacta. | **EPIC-09** |
| **HNF-28** | Regla 3 clics | Arquitectura intuitiva. | **Dado** que se busca una función, **Cuando** se navega desde dashboard, **Entonces** se debe completar en máximo 3 clics. | **EPIC-10** |
| **HNF-29** | Design System | Consistencia UI. | **Dado** que hay nuevas pantallas, **Cuando** el usuario navega, **Entonces** los colores/espaciados deben ser uniformes. | **EPIC-10** |
| **HNF-30** | Health Checks | Monitoreo de salud. | **Dado** que falla un microservicio, **Cuando** el monitor consulta /health, **Entonces** detecta y notifica antes del reporte del cliente. | **EPIC-08** |

---

### Technical Stories

| ID | Título | Descripción | Criterios de Aceptación (Gherkin) |
| :--- | :--- | :--- | :--- |
| **TS-01** | Documentación OpenAPI | Implementar Swagger/OpenAPI para la documentación automática de la API. | El endpoint `/api/docs` debe mostrar todos los recursos, métodos y esquemas de respuesta actualizados. |
| **TS-02** | Estandarización de Respuestas | Crear un interceptor/formateador global para respuestas JSON consistentes. | Todas las respuestas deben seguir la estructura `{ "data": {}, "meta": {}, "errors": [] }`. |
| **TS-03** | Autenticación JWT | Implementar autenticación basada en JSON Web Tokens con rotación de Refresh Tokens. | El sistema debe emitir un `access_token` de corta duración y un `refresh_token` seguro en `HttpOnly cookie`. |
| **TS-04** | Paginación Global | Desarrollar un helper de paginación para endpoints de colecciones (Historial, Usuarios). | Los endpoints de lista deben aceptar parámetros `page` y `limit`, y devolver metadata de totalización. |
| **TS-05** | Middleware de Roles (RBAC) | Crear decoradores o middlewares para validar permisos por rol en los controladores. | Si un usuario con rol "Staff" intenta un `DELETE` en `/doors`, la API debe retornar un error `403 Forbidden`. |
| **TS-06** | Validación de DTOs | Implementar validación de esquemas de entrada (Data Transfer Objects) en cada request. | Cualquier payload que no cumpla con el tipo de dato o longitud debe ser rechazado con un error `400 Bad Request`. |
| **TS-07** | Manejo de Excepciones | Crear un Global Exception Filter para capturar errores y evitar fugas de stack trace. | En modo producción, los errores `500` no deben revelar detalles de la base de datos o líneas de código. |
| **TS-08** | CORS Policy | Configurar políticas de Cross-Origin Resource Sharing. | La API solo debe aceptar peticiones desde los dominios autorizados de la aplicación web y el simulador. |

---

### Definición de Epics (Módulos Generales)

| Epic ID | Nombre de la Epic | Descripción |
| :--- | :--- | :--- |
| **EPIC-01** | **Gestión de Identidad y Cuenta** | Todo lo relacionado con autenticación, seguridad de perfil y acceso inicial al sistema. |
| **EPIC-02** | **Administración de Personal (RRHH)** | Gestión del ciclo de vida del usuario: creación, asignación de roles, desactivación e invitaciones. |
| **EPIC-03** | **Configuración de Infraestructura y Reglas** | Definición de puertas físicas y las reglas de negocio (horarios, días, accesos temporales). |
| **EPIC-04** | **Centro de Monitoreo y Alertas** | El "corazón" operativo: dashboard en tiempo real, gestión de alertas e indicadores de estado. |
| **EPIC-05** | **Entorno de Simulación (Virtual Lock)** | Módulo para clientes sin hardware que permite probar la lógica de acceso digitalmente. |
| **EPIC-06** | **Auditoría, Reportes e Integridad** | Registro histórico, exportación de datos, analítica avanzada y protección de la inmutabilidad de logs. |
| **EPIC-07** | **Ecosistema Comercial y Suscripciones** | Manejo de tiers (Básico, Pro, Enterprise), límites de cuenta y gestión multi-sede. |
| **EPIC-08** | **Rendimiento, Disponibilidad y Escalabilidad** | Calidad del sistema en términos de velocidad, estabilidad frente a carga y recuperación ante fallos. |
| **EPIC-09** | **Capa de Seguridad y Ciberdefensa** | Normas técnicas de encriptación, protocolos de red, protección contra ataques y privacidad de datos. |
| **EPIC-10** | **Experiencia de Usuario (UX/UI)** | Consistencia visual, accesibilidad, diseño responsivo y usabilidad general. |
| **EPIC-11** | **Escalabilidad Global e i18n** | Preparación técnica del software para mercados internacionales y multi-idioma. |

## 3.2. Impact Mapping

<div align="center">
  <img src="/Resources/Chapter3/MapaImpacto.png" alt="Mapa de Impacto" width="700"/>
</div>
<br>

## 3.3. Product Backlog Priorizado

| # Orden | User Story Id | Título | Descripción | Story Points (1 / 2 / 3 / 5 / 8) |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **HU-01** | Inicio de sesión estándar | Como administrador, deseo ingresar con correo y clave para acceder al panel de control. | 8 |
| 2 | **HU-03** | Creación de usuarios | Como admin de RRHH, deseo registrar empleados con correo único para gestionar el acceso al personal. | 8 |
| 3 | **HU-04** | Asignación de roles | Como administrador, deseo asignar roles específicos para automatizar los permisos de cada usuario. | 8 |
| 4 | **HU-08** | Dashboard Real-Time | Como monitor de seguridad, deseo ver los eventos en tiempo real para reaccionar ante incidencias sin recargar la web. | 8 |
| 5 | **HU-09** | Simulación exitosa | Como desarrollador, deseo simular accesos permitidos para validar el flujo del sistema sin hardware físico. | 8 |
| 6 | **HU-13** | Historial detallado | Como auditor, deseo ver una lista paginada de movimientos para fiscalizar quién entró y a qué hora. | 8 |
| 7 | **HU-19** | Desactivación rápida | Como administrador, deseo revocar accesos instantáneamente para proteger la red ante despidos o emergencias. | 8 |
| 8 | **HU-20** | Gestión de Puertas | Como administrador, deseo configurar puntos de acceso para organizar la infraestructura física del sistema. | 8 |
| 9 | **HU-26** | Cierre de sesión | Como usuario, deseo cerrar mi sesión para destruir el token de acceso y proteger mi cuenta. | 8 |
| 10 | **HNF-03** | Encriptación de claves | Como responsable de seguridad, deseo usar hashing bcrypt para que las claves nunca se guarden en texto plano. | 8 |
| 11 | **HNF-04** | Datos en tránsito | Como usuario, deseo que la comunicación sea vía HTTPS para proteger mis datos sensibles durante el envío. | 8 |
| 12 | **HNF-15** | Data Isolation | Como cliente corporativo, deseo un esquema multi-empresa para garantizar que nadie más vea mis datos. | 8 |
| 13 | **HNF-26** | Seguridad OWASP | Como desarrollador, deseo sanitizar todos los inputs para prevenir ataques de inyección SQL o XSS. | 8 |
| 14 | **TS-03** | Autenticación JWT | Como arquitecto, deseo implementar tokens JWT con rotación para asegurar una autenticación persistente y segura. | 8 |
| 15 | **TS-05** | Middleware de Roles | Como desarrollador, deseo crear decoradores RBAC para restringir el acceso a la API según el rol del usuario. | 8 |
| 16 | **TS-06** | Validación de DTOs | Como desarrollador, deseo validar los esquemas de entrada para rechazar peticiones mal formadas. | 8 |
| 17 | **TS-08** | CORS Policy | Como arquitecto, deseo configurar políticas CORS para que solo dominios autorizados consuman la API. | 8 |
| 18 | **HU-02** | Autenticación 2FA | Como usuario, deseo una verificación de segundo paso para añadir una capa extra de seguridad a mi cuenta. | 5 |
| 19 | **HU-05** | Acceso días laborales | Como administrador, deseo restringir el acceso por calendario para evitar ingresos no autorizados en días no laborables. | 5 |
| 20 | **HU-06** | Acceso franjas horarias | Como administrador, deseo limitar el acceso por horas para asegurar que el personal entre solo en su turno. | 5 |
| 21 | **HU-10** | Simulación denegada | Como desarrollador, deseo simular accesos fallidos para verificar que las reglas de negocio disparen las alertas correctas. | 5 |
| 22 | **HU-11** | Alerta intentos fallidos | Como monitor de seguridad, deseo detectar ataques de fuerza bruta para bloquear intrusos a tiempo. | 5 |
| 23 | **HU-21** | Acceso por puerta | Como administrador, deseo asignar permisos por puerta específica para controlar zonas restringidas. | 5 |
| 24 | **HU-23** | Reset de contraseña | Como usuario, deseo recuperar mi acceso mediante un enlace temporal para autogestionar mi cuenta. | 5 |
| 25 | **HU-29** | Alerta desconexión | Como administrador, deseo saber si una puerta pierde conexión para realizar mantenimiento preventivo inmediato. | 5 |
| 26 | **HNF-01** | Latencia Dashboard | Como usuario, deseo actualizaciones en menos de 1 segundo para tener una experiencia fluida y reactiva. | 5 |
| 27 | **HNF-05** | Disponibilidad | Como cliente, deseo un uptime del 99.9% para asegurar que el control de acceso nunca se detenga. | 5 |
| 28 | **HNF-06** | Diseño Responsivo | Como usuario móvil, deseo una interfaz adaptable para gestionar el sistema desde mi smartphone. | 5 |
| 29 | **HNF-07** | Inmutabilidad logs | Como auditor, deseo que los logs sean de solo lectura para garantizar la integridad de las pruebas legales. | 5 |
| 30 | **HNF-11** | Tolerancia fallos | Como administrador, deseo que el sistema sea modular para que un fallo en un servicio no tumbe toda la plataforma. | 5 |
| 31 | **HNF-14** | Anti-Brute Force | Como sistema de seguridad, deseo bloquear IPs tras 5 fallos para mitigar ataques automatizados. | 5 |
| 32 | **HNF-16** | Backups diarios | Como administrador de IT, deseo respaldos diarios automáticos para recuperar el sistema ante desastres. | 5 |
| 33 | **HNF-19** | Rate Limiting | Como desarrollador, deseo limitar las peticiones por minuto para proteger la API contra bots y abusos. | 5 |
| 34 | **HNF-21** | Complejidad clave | Como sistema, deseo exigir claves fuertes para reducir el riesgo de cuentas vulneradas. | 5 |
| 35 | **HNF-30** | Health Checks | Como equipo de DevOps, deseo monitorear la salud de los microservicios para detectar caídas antes que el usuario. | 5 |
| 36 | **TS-02** | Estandarización de Respuestas | Como desarrollador frontend, deseo una estructura JSON única para facilitar el consumo de datos. | 5 |
| 37 | **TS-04** | Paginación Global | Como desarrollador, deseo implementar paginación en las listas para optimizar el rendimiento de la red. | 5 |
| 38 | **TS-07** | Manejo de Excepciones | Como usuario, deseo ver mensajes de error amigables para entender qué falló sin ver detalles técnicos. | 5 |
| 39 | **HU-07** | Accesos temporales | Como recepcionista, deseo crear permisos con caducidad para gestionar visitas de forma automática. | 3 |
| 40 | **HU-12** | Alerta fuera de horario | Como vigilante, deseo recibir notificaciones destacadas para identificar intentos de acceso sospechosos. | 3 |
| 41 | **HU-14** | Filtros de historial | Como auditor, deseo filtrar por fecha y estado para encontrar registros específicos rápidamente. | 3 |
| 42 | **HU-15** | Límites Plan Básico | Como dueño del producto, deseo restringir el número de usuarios para incentivar el upgrade a planes premium. | 3 |
| 43 | **HU-16** | Upgrade Profesional | Como cliente, deseo pagar por el Plan Pro para desbloquear funciones avanzadas y eliminar límites. | 3 |
| 44 | **HU-17** | Gestión multi-sede | Como gerente, deseo cambiar entre sedes independientes para centralizar la operación de mi empresa. | 3 |
| 45 | **HU-22** | Alerta uso indebido | Como administrador, deseo etiquetar intentos sin autorización para prevenir espionaje interno. | 3 |
| 46 | **HU-24** | Exportación de datos | Como administrativo, deseo descargar reportes en CSV para realizar análisis externos o presentaciones. | 3 |
| 47 | **HU-25** | Cierre de alertas | Como operador, deseo marcar alertas como resueltas para mantener el panel de monitoreo limpio. | 3 |
| 48 | **HU-30** | Notificación crítica | Como dueño de negocio, deseo recibir emails automáticos en emergencias para estar informado 24/7. | 3 |
| 49 | **HNF-02** | Rendimiento carga | Como usuario, deseo que la página sea interactiva en menos de 2 segundos para no perder tiempo esperando. | 3 |
| 50 | **HNF-08** | Escalabilidad | Como sistema, deseo soportar 500 peticiones simultáneas para garantizar estabilidad en horas pico. | 3 |
| 51 | **HNF-09** | Timeout sesión | Como administrador de seguridad, deseo que las sesiones inactivas expiren para evitar accesos indebidos en PCs desatendidas. | 3 |
| 52 | **HNF-10** | Compatibilidad | Como usuario, deseo usar cualquier navegador moderno para acceder al sistema sin errores visuales. | 3 |
| 53 | **HNF-12** | Velocidad 2FA/Email | Como usuario, deseo recibir correos en menos de 5 segundos para no interrumpir mi flujo de trabajo. | 3 |
| 54 | **HNF-17** | Log de auditoría | Como administrador principal, deseo registrar cambios de configuración para saber quién modificó las reglas del sistema. | 3 |
| 55 | **HNF-23** | RTO (Recuperación) | Como administrador de sistemas, deseo recuperar la operación en máximo 4 horas tras un desastre total. | 3 |
| 56 | **HNF-27** | Sincronía NTP | Como sistema legal, deseo usar servidores NTP para que todos los registros tengan una hora exacta y válida. | 3 |
| 57 | **TS-01** | Documentación OpenAPI | Como desarrollador, deseo una documentación Swagger automática para facilitar la integración de nuevos módulos. | 3 |
| 58 | **HU-18** | Reportes avanzados | Como gerente, deseo gráficas de horas pico para optimizar el personal en mi establecimiento. | 2 |
| 59 | **HU-27** | Invitación masiva | Como admin de RRHH, deseo enviar links únicos a múltiples correos para agilizar el onboarding de empleados. | 2 |
| 60 | **HU-28** | Edición de perfil | Como usuario, deseo actualizar mis datos de contacto y foto para mantener mi perfil al día. | 2 |
| 61 | **HNF-13** | Accesibilidad WCAG | Como usuario con discapacidad, deseo una interfaz con alto contraste para navegar sin dificultades. | 2 |
| 62 | **HNF-18** | UX de fallos | Como usuario, deseo interfaces claras que me guíen cuando ocurre un error de conexión o datos. | 2 |
| 63 | **HNF-20** | Velocidad Export | Como administrativo, deseo procesar descargas masivas en menos de 10 segundos para ser más eficiente. | 2 |
| 64 | **HNF-29** | Design System | Como diseñador, deseo una UI consistente para que la experiencia de usuario sea uniforme en todas las pantallas. | 2 |
| 65 | **HNF-22** | Soporte i18n | Como administrador global, deseo que el sistema esté preparado para traducciones para expandir el negocio a otros países. | 1 |
| 66 | **HNF-24** | Archivado datos | Como administrador de IT, deseo mover logs antiguos a almacenamiento frío para reducir costos de base de datos. | 1 |
| 67 | **HNF-25** | Consumo batería | Como guardia con tablet, deseo que la app esté optimizada para no agotar la batería durante el turno. | 1 |
| 68 | **HNF-28** | Regla 3 clics | Como usuario, deseo llegar a cualquier función principal en máximo 3 clics para mejorar mi productividad. | 1 |

---

### Evidencias de Gestión en Jira

A continuación, se adjuntan las capturas del tablero de Jira utilizado para la gestión del Backlog y la estimación de Story Points del equipo de SmartLock.

<div align="center">
  <img src="/Resources/Chapter3/story_points.png" alt="Story Points" width="500"/><br>
  <i>Story Points</i><br><br>
  
  <img src="/Resources/Chapter3/formato.png" alt="Formato de HU" width="500"/><br>
  <i>Formato de Historias de Usuario</i><br><br>
  
  <img src="/Resources/Chapter3/organizacion.png" alt="Estructura de prioridad" width="500"/><br>
  <i>Estructura de Prioridad</i>
</div>
<br>

**Enlace al tablero de Jira:** [SmartLock - UPC Team Open Source](https://upc-team-open-source.atlassian.net/jira/software/projects/SMAR/boards/1?atlOrigin=eyJpIjoiNDFhNzk1OTIxMGU0NDc5ZjlmYjliMzlmYjU2MDVmOTIiLCJwIjoiaiJ9)

# Capítulo IV: Product Design

## 4.1. Style Guidelines.
Se describen las directrices que aseguran la uniformidad estética del proyecto.<br>

### 4.1.1. General Style Guidelines.
**Colors:**
<br>
Elegimos una paleta que grite **seguridad y tecnología**, pero sin cansar la vista (pensando en administradores que estarán pegados al dashboard monitoreando accesos).
<br>
* **Azul Oscuro (#1B263B):** Es nuestro color estrella. Da esa seriedad y confianza que necesitas cuando hablas de controlar quién entra a tu edificio u oficina.
* **Casi Negro (#0D1B2A):** Lo usamos para los textos importantes. No es negro puro porque eso agota la vista en sesiones largas, pero tiene el peso suficiente para que se lea claro.
* **Gris Neutro (#E0E1DD):** Este va de fondo en las secciones. Es limpio y hace que los demás elementos resalten sin esfuerzo.
* **Azul Eléctrico (#3E92CC):** Este es nuestro "call to action". Si hay algo que el usuario tiene que clickear sí o sí (como el botón de "Abrir Puerta" o "Guardar Configuración"), va en este color.

<img src="/Resources/Chapter4/Style-Guidelines/Paleta-de-colores/Paleta-de-colores.PNG" alt="Paleta de Colores">

**Branding**<br>
El logo de **SmartLock** es directo al grano: un **candado**. Elegimos este isotipo porque es el símbolo universal de la seguridad física; no necesitamos complicarlo con más adornos para que el usuario entienda qué hacemos. Lo que lo hace moderno es su diseño minimalista y limpio. Acompañando al candado, la tipografía del nombre es sólida y de cortes precisos. Queríamos que la identidad visual transmitiera esa firmeza y robustez que se espera de un sistema de seguridad confiable, alejándonos de cualquier estética que pudiera parecer "frágil" o improvisada.

<img src="/Resources/Chapter4/Logo/SmartLock-Logo.png" alt="Logo SmartLock">

**Typography** <br>
Nos fuimos por **Inter**. ¿Por qué? Porque cuando tienes una lista gigante de registros de entrada y salida, necesitas una letra que se lea perfecto en pantallas de cualquier tamaño. Es una fuente *sans-serif* optimizada para entornos digitales.
* **Bold:** Para los títulos de sección y alertas que no puedes ignorar.
* **Semi-Bold:** Para encabezados de tablas o nombres de usuarios.
* **Regular:** Para el cuerpo de texto y los logs de acceso.
* *Referencia:* [Inter - Google Fonts](https://fonts.google.com/specimen/Inter)

**Spacing**<br>
Para que no todo esté tirado al azar, usamos la regla de los **8px**. Si vas a separar algo, que sea múltiplo de 8. En el código, **solo usamos `rem`** para que la interfaz sea escalable y se adapte bien si el usuario cambia el tamaño de fuente de su navegador.

| Categoría | Medida (rem / px) | Aplicación en el Diseño |
| :--- | :--- | :--- |
| **X-Small** | 0.25 rem / 4 px | Alineación de iconos y micro-ajustes de posición. |
| **Small** | 0.5 rem / 8 px | Espacio entre un texto y su campo de entrada (input). |
| **Medium** | 1.0 rem / 16 px | Relleno interno (padding) de botones y tarjetas. |
| **Large** | 1.5 rem / 24 px | Margen entre componentes de un mismo bloque funcional. |
| **X-Large** | 2.0 rem / 32 px | Distancia entre contenedores de información independientes. |
| **Section** | 4.0 rem / 64 px | El espacio grande entre bloques estructurales de la página. |

> **Nota técnica:** Queda prohibido usar píxeles (`px`) estáticos para márgenes o paddings. Todo debe ir en `rem` siguiendo la escala de arriba.

**Dimensions (Tono y Comunicación)**<br>
El estilo de comunicación de SmartLock es **directo y técnico**. Como ingenieros, no queremos meterle "floro" innecesario al usuario.
* Si alguien intenta entrar y no tiene permiso, el sistema dice **"Acceso Denegado"**, sin vueltas.
* Usamos términos que un jefe de seguridad entienda rápido (como "Trazabilidad", "Cifrado" o "Autenticación").
* La idea es que la plataforma sea una herramienta de trabajo estricta, libre de narrativa irrelevante, para que la toma de decisiones sea rápida.

---

### 4.1.2. Web Style Guidelines.

Aquí es donde aterrizamos todo para que la plataforma web se vea de nivel profesional:

1.  **Cero Adornos:** Si un botón o un icono no ayuda a monitorear o gestionar la seguridad, se quita. Queremos una interfaz limpia donde el control sea el protagonista.
2.  **Todo es Responsive:** El administrador puede estar en su oficina con un monitor gigante o en la entrada con su tablet. La estructura no debe romperse y los elementos deben ser fáciles de tocar/clickear en cualquier dispositivo.
3.  **Jerarquía Visual:** Usamos el contraste y los colores semánticos para que el ojo sepa qué es urgente.
* **Rojo:** Alertar brechas de seguridad o intentos fallidos.
* **Verde/Azul:** Accesos válidos y sistema operativo.
* **Amarillo:** Dar advertencias ante cualquier problema.

## 4.2. Information Architecture.
En SmartLock, la arquitectura de la información no es solo un menú de opciones; es el cerebro que permite que un administrador no entre en pánico cuando hay cientos de personas moviéndose por sus instalaciones. En el mundo de la seguridad digital, un segundo de duda puede ser un problema grave. Por eso, hemos diseñado una estructura donde la información crítica (como quién entró por la puerta principal hace un segundo) siempre está a la vista, eliminando cualquier "floro" visual que distraiga de lo importante: el control total y en tiempo real.

---

### 4.2.1. Organization Systems.
Para que SmartLock sea realmente eficiente tanto para el guardia en la puerta como para el administrador del sistema, hemos decidido combinar varios sistemas de organización:

### **Organización visual del contenido**
* **Jerárquica (Visual Hierarchy):** Elegimos este sistema porque en seguridad hay datos que "gritan" más fuerte que otros. En el Dashboard, los intentos de acceso fallidos o las alertas de puertas forzadas utilizan un tamaño y color prominente (rojo/bold). No es solo estética; es una estrategia para que el ojo del usuario sepa qué atender primero sin tener que leer toda la pantalla.
* **Organización secuencial (Step-by-step):** Registrar una nueva cerradura inteligente o dar de alta a un nuevo usuario puede ser tedioso. Lo dividimos en pasos claros (Identificación > Asignación de Permisos > Vinculación de Hardware) para evitar que el usuario se sienta abrumado y garantizar que no se salte ningún protocolo de seguridad.

### **Esquemas de categorización de contenido**
* **Por tópicos (Zonas de Acceso):** Organizamos la info por "Zonas" (ej. Piso 1, Almacén, Oficinas). Es la forma más lógica en la que un administrador piensa su espacio físico.
* **Según audiencia (Roles de Usuario):** El "Usuario Final" solo ve su llave digital y su historial personal. El "Administrador" ve todo el panel de control y analíticas. Esto "limpia" la interfaz de cada usuario, mostrándole solo lo que es relevante para su rol.
* **Cronológico:** Es vital para el Log de Eventos. Si pasa algo, necesitamos reconstruir la historia de forma lineal. Mostramos los ingresos por hora y fecha para que la trazabilidad sea impecable.
* **Alfabético:** Lo reservamos para el directorio de usuarios y empleados, donde la búsqueda por nombre de la A a la Z es la forma más rápida de encontrar a alguien.

---
### 4.2.2. Labeling Systems.

En el sistema de etiquetado de SmartLock, hemos huido del lenguaje genérico. Queremos que el usuario sienta que el software es una herramienta técnica y profesional:

* **Panel de Control:** En lugar de "Inicio", porque aquí es donde realmente se gestiona todo el hardware.
* **Bitácora de Accesos:** Suena más profesional que "Historial". Da la idea de un registro oficial y serio de cada movimiento para auditorías.
* **Credenciales Digitales:** Término usado para referirse a los permisos de acceso de los usuarios, reforzando la idea de seguridad y autenticación.
* **Puntos de Control:** En lugar de "Puertas", porque SmartLock puede controlar desde una puerta hasta un torniquete o una barrera vehicular.

---

### 4.2.3. SEO Tags and Meta Tags.
Queremos que SmartLock sea lo primero que aparezca cuando una empresa busque modernizar su seguridad.

### **Landing Page**
* **Título:** `<title>SmartLock | Control de Accesos Inteligente y Seguridad Digital</title>`
* **Descripción:** `<meta name="description" content="Moderniza la seguridad de tu edificio. SmartLock ofrece gestión de accesos en tiempo real, trazabilidad total y control desde la nube para oficinas y universidades."/>`
* **Keywords:** `<meta name="keywords" content="SmartLock, Control de accesos, Seguridad digital, Cerraduras inteligentes, Trazabilidad, SmartTecnologies, Software de seguridad Perú, ConTech."/>`
* **Autor:** `<meta name="author" content="SmartTecnologies" />`

### **Web Application**
* **Título:** `<title>Dashboard SmartLock - Gestión de Accesos</title>`
* **Descripción:** `<meta name="description" content="Panel de administración de SmartLock. Monitorea ingresos, gestiona usuarios y configura tus puntos de control en tiempo real."/>`

---

### 4.2.4. Searching Systems.
No queremos que el usuario "busque", queremos que "encuentre" rápido:

* **Búsqueda Predictiva:** A medida que el administrador escribe (ej. un DNI o nombre), el sistema sugiere usuarios registrados para ahorrar tiempo.
* **Filtros de Facetas:** El usuario puede refinar los registros por **Rango de fechas**, **Zona de acceso**, **Estado de ingreso** (Exitoso/Denegado) y **Tipo de usuario**, evitando la sobrecarga de información.
* **Búsqueda por Dispositivo:** Permite localizar rápidamente una cerradura o sensor específico dentro de toda la infraestructura mediante su ID técnico.

---
### 4.2.5. Navigation Systems.
La navegación en SmartLock está pensada para ser "invisible" y eficiente:

* **Menú Lateral Retráctil:** Prioriza el espacio de trabajo central para ver los mapas de calor y tablas de acceso, manteniendo los módulos principales a un solo clic.
* **Migas de Pan (Breadcrumbs):** Vital para no perderse cuando navegas por sedes (ej. Sedes > Lima Centro > Piso 3 > Laboratorio A), permitiendo al usuario ubicarse en todo momento.
* **Acciones Contextuales:** El sistema ofrece botones inteligentes según el estado del punto de control (ej. si una puerta detecta una intrusión, el botón principal será "Bloquear Acceso" o "Contactar Seguridad").

## 4.3. Landing Page UI Design.
En esta sección se detalla el proceso de diseño de la interfaz de usuario para la página de aterrizaje de **SmartLock**. El diseño se centra en la conversión de usuarios y la exposición clara de la propuesta de valor del sistema de control de acceso.

### 4.3.1. Landing Page Wireframe.
El wireframe de baja fidelidad define la estructura visual y la jerarquía de la información. Se ha priorizado una navegación intuitiva, destacando las funcionalidades principales y los beneficios de seguridad del sistema.

![Landing Page Wireframe](/Resources/Chapter4/LandingPage/Wireframe%20Landing%20Page.png)

* **Elementos clave:** Estructura de navegación, sección hero con llamado a la acción (CTA) y secciones de beneficios para el segmento de negocios.

### 4.3.2. Landing Page Mock-up.
El mock-up de alta fidelidad integra la identidad visual de la marca, incluyendo la paleta de colores, tipografía y elementos gráficos finales. Este diseño representa la apariencia exacta que tendrá la aplicación web una vez implementada.

![Landing Page Mock-up](/Resources/Chapter4/LandingPage/Mockup%20Landing%20Page.png)

* **Detalles estéticos:** Uso de contrastes para mejorar la legibilidad y elementos visuales que refuerzan la confianza y modernidad del sistema **SmartLock**.

## 4.4. Web Applications UX/UI Design.
Esta sección presenta y explica la propuesta visual y de interacción para las aplicaciones que constituyen la experiencia de usuario con los productos digitales de **SmartLock**.

### 4.4.1. Web Applications Wireframes.
Esta sección presenta los esquemas de baja fidelidad que definen la estructura de la aplicación web. Se ha priorizado la **Arquitectura de Información** mediante un sistema de navegación lateral (Sidebar) que organiza las funciones de gestión de usuarios, eventos y seguridad de forma jerárquica.
* **Principios de Diseño:** Se aplica el principio de proximidad para agrupar funciones relacionadas (como el perfil de usuario y notificaciones) y consistencia en la ubicación de los elementos de control.
* **Diseño Inclusivo:** Los wireframes consideran espacios adecuados para elementos interactivos y una disposición clara que facilita el uso de tecnologías de asistencia como lectores de pantalla.

---

#### A. Flujo de Acceso y Autenticación

### Inicio de Sesión

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Inicio sesion.png" width="800" alt="Inicio de Sesión Wireframe">
</p>

**Descripción:** Wireframe de la pantalla de acceso principal que define la estructura de los campos de autenticación, el botón de inicio de sesión y los elementos de recuperación de acceso.

---

### Registro de Sesión (Sign Up)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Registro Sesión.png" width="800" alt="Registro de Sesión Wireframe">
</p>

**Descripción:** Esquema del formulario de registro orientado al alta de nuevos administradores dentro de la plataforma, mostrando la distribución lógica de los campos requeridos.

---

### Autenticación de Dos Factores (2FA)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Autenticacion 2FA.png" width="800" alt="Autenticación 2FA Wireframe">
</p>

**Descripción:** Diseño estructural de la segunda capa de seguridad mediante verificación por código, enfocado en la simplicidad de interacción y validación segura del usuario.

---

#### B. Configuración de Infraestructura

### Creación de Sedes (Plan Principiante)

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/crear sedes -plan principiante.png" width="800" alt="Creación de Sedes Wireframe">
</p>

**Descripción:** Wireframe del proceso inicial de configuración de sedes, donde se organizan los campos necesarios para el despliegue y administración básica del sistema.

---

### Dashboard de Puntos de Control

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard - Puntos de Control.png" width="800" alt="Dashboard Puntos de Control Wireframe">
</p>

**Descripción:** Esquema de monitoreo de dispositivos físicos y puntos de acceso, utilizando una distribución visual en cuadrícula para facilitar el control operativo en tiempo real.

---

#### C. Dashboards de Gestión por Niveles

### Dashboard Corporativo

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard -corportivo.png" width="800" alt="Dashboard Corporativo Wireframe">
</p>

**Descripción:** Vista de alto nivel orientada a organizaciones empresariales, priorizando métricas globales, indicadores de seguridad y administración multisede.

---

### Dashboard Principiante

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard- gratuito.png" width="800" alt="Dashboard Principiante Wireframe">
</p>

**Descripción:** Versión simplificada del panel principal, diseñada para usuarios del plan gratuito, manteniendo consistencia visual y acceso a funciones esenciales.

---

#### D. Administración de Seguridad y Personal

### Dashboard de Usuarios

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard - usuarios.png" width="800" alt="Dashboard de Usuarios Wireframe">
</p>

**Descripción:** Distribución estructural del módulo de gestión de usuarios, incluyendo filtros, tabla de registros, búsqueda avanzada y administración de permisos.

---

### Gestión de Eventos

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard - eventos.png" width="800" alt="Gestión de Eventos Wireframe">
</p>

**Descripción:** Módulo orientado a la configuración de accesos temporales mediante eventos programados, permitiendo restricciones horarias y control de visitantes.

---

### Gestión de Credenciales

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard - Credenciales.png" width="800" alt="Gestión de Credenciales Wireframe">
</p>

**Descripción:** Organización funcional del sistema de emisión y control de credenciales digitales, permitiendo el seguimiento de accesos autorizados.

---

### Bitácora de Accesos

<p align="center">
  <img src="/Resources/Chapter4/Web-Application/Dashboard - Bitacora.png" width="800" alt="Bitácora de Accesos Wireframe">
</p>

**Descripción:** Estructura diseñada para la visualización de logs históricos de acceso, facilitando auditorías de seguridad y trazabilidad de eventos.

### 4.4.2. Web Applications Wireflow Diagrams.
*[Sección en desarrollo]*

### 4.4.3. Web Applications Mock-ups.
Esta sección presenta los mock-ups de alta fidelidad de la plataforma web de SmartLock. Estos diseños representan la apariencia visual final del sistema, incluyendo identidad visual, paleta de colores, tipografía, distribución de componentes y experiencia de usuario orientada a la implementación real del producto.

---

#### A. Flujo de Acceso y Seguridad

### Inicio de Sesión

![Inicio de Sesión Mockup](/Resources/Chapter4/Web-Application/Inicio Sesión-Mockup.png)

**Descripción:** Mock-up de la pantalla principal de acceso al sistema, donde se visualiza la interfaz final de autenticación con diseño visual completo, jerarquía de botones y elementos de recuperación de acceso.

---

### Registro de Sesión (Sign Up)

![Registro de Sesión Mockup](/Resources/Chapter4/Web-Application/Registro Sesión-Mockup.png)

**Descripción:** Representación visual del formulario de registro de nuevos administradores, mostrando el diseño definitivo de campos, validaciones visuales y estructura de navegación.

---

### Autenticación de Dos Factores (2FA)

![Autenticación 2FA Mockup](/Resources/Chapter4/Web-Application/Autentificación de 2 Factores-Mockup.png)

**Descripción:** Diseño final de la segunda capa de seguridad mediante código de verificación, enfocado en claridad visual, seguridad y facilidad de uso para el usuario.

---
#### B. Configuración de Infraestructura

### Dashboard Plan Principiante

![Dashboard Plan Principiante Mockup](/Resources/Chapter4/Web-Application/Dashboard- Plan Principiante-Mockup.png)

**Descripción:** Mock-up del panel principal para usuarios del plan principiante, presentando una interfaz simplificada con acceso rápido a funciones esenciales y monitoreo básico del sistema.

---
### 4.4.4. Web Applications User Flow Diagrams.
*[Sección en desarrollo]*

## 4.5. Web Applications Prototyping.
*[Sección en desarrollo]*

## 4.6. Domain-Driven Software Architecture.

### 4.6.1. Design-Level Event Storming.
En esta sección se detalla el diseño táctico del sistema, profundizando en la arquitectura y los componentes técnicos necesarios para implementar la solución. A diferencia del Big Picture, el DesignLevel Event Storming se enfoca en definir los límites de los agregados, los comandos que disparan cambios de estado y las políticas que gobiernan las reglas de negocio.

<p align="center">
  <img src="/Resources/Chapter4/eventStormin/design-level.jpeg" width="800" alt="Design Level Event Storming">
</p>

#### Authentication Context
Actúa como la puerta de entrada digital al ecosistema de SmartLock, gestionando los procesos de registro y acceso de los usuarios administrativos. Este componente se encarga de validar las credenciales de identidad y de implementar medidas de seguridad reforzadas, como la verificación en dos pasos (2FA), para garantizar que solo las personas legítimas ingresen al sistema. Además, supervisa la integridad de las sesiones activas, aplicando reglas automáticas que protegen la cuenta global ante cualquier cambio de seguridad o intento de acceso no autorizado.

<p align="center">
  <img src="/Resources/Chapter4/eventStormin/authentication-context.png" width="800" alt="Authentication Context">
</p>

#### Organization Context
Constituye el núcleo operativo del sistema, encargado de estructurar la jerarquía institucional y física de cada cliente. Este componente facilita la creación de entidades globales, la gestión de sedes o sitios específicos y el registro técnico de cada punto de acceso o puerta dentro de la plataforma. Al centralizar esta estructura, el sistema asegura que la administración de los espacios físicos sea coherente y escalable, sirviendo como la base informativa necesaria para que los demás módulos operen según la distribución administrativa de la organización.

<p align="center">
  <img src="/Resources/Chapter4/eventStormin/organization-context.png" width="800" alt="Organization Context">
</p>

#### Security Context
Centraliza la gestión de identidades y la integridad del sistema SmartLock, asegurando que solo el personal autorizado interactúe con la infraestructura física. Este componente se encarga de validar el acceso en tiempo real y coordinar las respuestas automáticas ante situaciones críticas o intentos de intrusión. Al aislar estas funciones, se garantiza una capa de protección robusta que salvaguarda tanto la información digital como la seguridad de los espacios físicos administrados.
<p align="center">
  <img src="/Resources/Chapter4/eventStormin/security-context.png" height="600" alt="Security Context">
</p>

#### Subscription Plan Context
Administra los planes comerciales y el modelo de facturación para cada organización dentro de la plataforma. Este componente es responsable de definir los niveles de servicio, gestionar los ciclos de pago y establecer los límites operativos, como el número permitido de puertas o usuarios según el plan adquirido.
<p align="center">
  <img src="/Resources/Chapter4/eventStormin/subscription-plan-context.png" width="750" alt="Subscription Plan Context">
</p>

#### User Context
Gestiona integralmente los perfiles y permisos de las personas que interactúan con la plataforma, distinguiendo claramente entre el personal administrativo y los usuarios de acceso físico. Este componente se encarga de dar de alta, actualizar o dar de baja a los miembros del sistema, asegurando que cada individuo cuente con las atribuciones necesarias según su rol dentro de la organización. Al centralizar esta administración, el sistema facilita un control preciso sobre quién puede operar el software y quién tiene permitido el ingreso a las instalaciones, manteniendo siempre un registro actualizado de todas las identidades activas.

<p align="center">
  <img src="/Resources/Chapter4/eventStormin/user-context.png" width="550" alt="User Context">
</p>

Descripción de los componentes identificados:
- **Comandos (Azul):** Representan las intenciones de los usuarios o sistemas externos para realizar una acción específica (ej. "Generar Código QR", "Validar Acceso"). 
- **Agregados (Amarillo):** Son las entidades o grupos de objetos que mantienen la consistencia de los datos y ejecutan la lógica de negocio ante un comando. 
- **Políticas (Lila):** Definen reacciones automáticas del sistema ante eventos específicos ("Siempre que ocurra el Evento X, ejecutar el Comando Y"). 
- **Modelos de Lectura (Verde):** Representan la información que el usuario visualiza en la interfaz para poder tomar una decisión y ejecutar un comando. 
- **Eventos de Dominio (Naranja):** Indican que algo relevante para el negocio ha sucedido exitosamente (ej. "Código QR Generado", "Acceso Denegado"). 

Este modelado permite al equipo de desarrollo tener una guía clara para la implementación de los servicios y la definición de la lógica en el código.

### 4.6.2. Software Architecture Context Diagram.

In this section, the team introduces the Software Architecture Context Diagram. This high-level overview illustrates the **SmartLock** software system as a central entity, surrounded by the key user personas and the external systems it interacts with to deliver its "Asset-Light" access control value proposition.

![Software Architecture Context Diagram](/Resources/Chapter4/umlfiles/contextDiagram.png)

**Explicación del diagrama:**

* **SmartLock System:** Es el núcleo de la plataforma que centraliza la lógica de generación de códigos QR dinámicos y la validación de reglas de acceso.
* **Usuarios:** El diagrama identifica al **Administrator** (configuración), **Security Staff** (validación móvil) y **Attendee** (usuario final) como los actores principales.
* **Sistemas Externos:** Se detalla la integración con **AWS SES** para la gestión de correos electrónicos y **Twilio API** para el envío de alertas críticas de seguridad vía SMS.

### 4.6.3. Software Architecture Container Diagrams.

In this section, the team presents the **Container Diagram** for SmartLock. This diagram expands the system's context to reveal the software containers that compose it (web applications, mobile applications, APIs, and databases). It illustrates the high-level distribution of responsibilities, exposes key technology decisions—such as Angular for the frontend, Java Spring Boot for the backend, and MySQL for persistence—and details how these containers communicate through the AWS cloud infrastructure.

![Software Architecture Container Diagram](/Resources/Chapter4/umlfiles/containerDiagram.png)

#### Diagram Explanation

The Container Diagram breaks down the internal architecture of SmartLock into the following key components:

* **Landing Page & Web Application (Frontend):** Developed using **Angular, TypeScript, and TailwindCSS**. The web application acts as a Single Page Application (SPA) that consumes the backend API. Both containers are hosted on **AWS S3** and distributed globally via **Amazon CloudFront** to ensure low latency and security via HTTPS.
* **Scanner Mobile App:** A specialized application for security staff, optimized for scanning QR codes and communicating with the server with minimal latency.
* **Core Backend API:** The system's main engine, developed in **Java using the Spring Boot framework**. It centralizes all domain-driven business logic (DDD), validates access attempts, and generates encrypted dynamic QR codes. It is deployed on **AWS Elastic Beanstalk** for automated load balancing and scaling.
* **Relational Database:** A **MySQL** database hosted on **Amazon RDS**, serving as the single source of truth. it ensures the immutability of access logs (audit trails) and the integrity of user profiles and access rules.
* **Communication:** The frontend and mobile app communicate asynchronously with the Backend API via **JSON over HTTPS**. The backend interacts with the database through **JDBC** and with third-party services (AWS SES and Twilio) via REST APIs.

### 4.6.4. Software Architecture Components Diagrams.

In this section, the team presents the **Component Diagram** for the Core Backend API container. This diagram zooms into the Java Spring Boot application to illustrate its internal structure based on Domain-Driven Design (DDD) and Layered Architecture. It shows how the system is divided into Controllers (Presentation), Services (Business Logic/Domain), and Repositories (Data Access), and how these components interact to execute the access control logic.

![Software Architecture Component Diagram](/Resources/Chapter4/umlfiles/componentDiagram.png)

#### Diagram Explanation

The Component Diagram breaks down the **Core Backend API** into the following functional layers:

* **Controllers (Presentation Layer):**
  * **Auth & Security Controller:** Exposes REST endpoints to handle user login, 2FA verification, and JSON Web Token (JWT) issuance.
  * **Access Validation Controller:** Receives API calls from the Scanner Mobile App to validate dynamic QR payloads in real-time.
  * **Space Manager Controller:** Provides endpoints for administrators (via the Web App) to perform CRUD operations on physical spaces and configure access schedules.

* **Services (Domain / Business Logic Layer):**
  * **Access Credential Service (Core Domain):** The heart of the system. It evaluates complex access policies, generates dynamic QR codes using cryptographic signatures, and determines whether an access attempt is granted or denied.
  * **Authentication Service:** Implements Role-Based Access Control (RBAC) and manages the lifecycle of credentials and tokens.
  * **Notification Publisher:** Uses the Spring ApplicationEventPublisher to asynchronously delegate alerts to prevent blocking the main execution thread during access validations.

* **Repositories (Infrastructure Layer):**
  * **Audit & Log Repository:** Uses Spring Data JPA to securely write immutable logs of every access attempt and security event into the database.
  * **Domain Data Repository:** Manage the persistence of user profiles, organizational data, doors, and policies.

* **Communication Flow:** The web and mobile applications send HTTP requests to the **Controllers**. These controllers delegate the business logic to the **Services**. The services evaluate the rules and use the **Repositories** to interact with the MySQL database via JDBC, or use the **Notification Publisher** to dispatch asynchronous emails and SMS via AWS SES and Twilio.

## 4.7. Software Object-Oriented Design.

En esta sección, el equipo presenta el diseño orientado a objetos del software, detallando la implementación interna y la estructura de componentes para cada *Bounded Context* de **SmartLock**. Los diagramas a continuación ilustran cómo se ha aplicado el enfoque de *Domain-Driven Design* (DDD) a nivel de código, definiendo claramente las responsabilidades, los límites de los agregados y los patrones de diseño utilizados tanto en la capa de presentación (Frontend) como en la lógica de negocio (Backend). Esta estructura garantiza un código modular, mantenible y altamente escalable.

### 4.7.1. Class Diagrams.

#### Diagrama de clases (Frontend)

<img src="/Resources/Chapter4/Diagram-Class/Frontend/Class-Diagram-Frontend-image.png" alt="Class Diagram Frontend">

El diagrama organiza el frontend de SmartLock en cinco *Bounded Contexts* (Authentication, Organization, User, Security y Subscription), lo que permite aislar la lógica de negocio y asegurar que cada módulo evolucione de forma independiente. Dentro de estos contextos, se implementan los 8 Agregados definidos, donde entidades raíz como *Security* y *Organization* encapsulan a *Door* y *Office* respectivamente; esto garantiza la integridad del sistema, ya que cualquier cambio de estado físico o estructural debe ser validado por su respectiva raíz de agregado antes de impactar la interfaz.

Bajo el enfoque DDD, la aplicación utiliza un *EventBus* en la capa Shared para comunicar eventos entre contextos de forma desacoplada y emplea el patrón *Assembler* para transformar los datos crudos de la API en objetos de dominio con comportamiento propio. Los *Stores* de la capa de aplicación gestionan estos agregados mediante Signals, permitiendo que la interfaz reaccione instantáneamente a cambios operativos —como la apertura de una puerta o la actualización de un perfil— sin comprometer la separación de responsabilidades ni la pureza del modelo de negocio.

#### Diagrama de clases (Backend)

<img src="/Resources/Chapter4/Diagram-Class/Backend/Class-Diagram-Backend-image.png" alt="Class Diagram Backend">

El backend de SmartLock ha sido estructurado estrictamente bajo los principios de *Domain-Driven Design* (DDD) utilizando el framework Spring Boot. La arquitectura se divide en 5 *Bounded Contexts* y 8 agregados principales, derivados del *Event Storming*, garantizando un alto nivel de cohesión y un bajo acoplamiento. Se emplean *Aggregate Roots* (como Security y Organization) para orquestar entidades secundarias (Door y Office), asegurando el cumplimiento de las reglas de negocio en la capa de dominio antes de ejecutar cualquier cambio de estado. 

Adicionalmente, se implementaron patrones de diseño estratégico como *Assembler* para la conversión de datos y aislamiento de la capa de presentación, el uso de *Records* de Java para garantizar la inmutabilidad de los DTOs, e interfaces dedicadas para los servicios y repositorios. Esta abstracción asegura un sistema altamente mantenible y preparado para escalar sin generar deuda técnica.

## 4.8. Database Design.

### 4.8.1. Database Diagrams.

<img src="/Resources/Chapter4/Data-Base-Diagram/Data-Base-Diagram-image.png" alt="Database Diagram">

El diagrama de base de datos para SmartLock se ha estructurado bajo un enfoque de normalización 3FN y *Domain-Driven Design* (DDD), organizando la información en *Bounded Contexts* que actúan como *Aggregate Roots* (como Users y Organization) para garantizar la integridad operativa y la escalabilidad mediante el uso de tipos de datos atómicos en MySQL. Desde la perspectiva de seguridad y persistencia, el diseño separa estrictamente las credenciales en la tabla *authentications* y los datos sensibles en *user_profiles* (con correos encriptados) para cumplir con las leyes de protección de datos, mientras que la tabla *access_logs* asegura una auditoría inmutable de cada evento físico. Finalmente, la arquitectura está totalmente optimizada para un ORM como Hibernate, facilitando el mapeo de relaciones uno-a-muchos y uno-a-uno mediante claves foráneas claras y tipos bigint, lo que permite un manejo eficiente de la carga perezosa (*Lazy Loading*) y una transición fluida del modelo relacional al código en Spring Boot.

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
| SMAR-33 | Encriptación | T-33-1 | Hash de claves | Programar la función para que las contraseñas se guarden encriptadas en la DB usando Bcrypt. | 4 | Juan | Done |
| SMAR-33 | Encriptación | T-33-2 | Pruebas de Login | Verificar que al loguearse, el sistema compare la clave escrita con la encriptada en la DB. | 3 | Juan | Done |
| SMAR-34 | Datos en tránsito | T-34-1 | Configuración HTTPS | Configurar el servidor para que la URL use certificados SSL. | 4 | Gabriel | Done |
| SMAR-34 | Datos en tránsito | T-34-2 | Redirección Segura | Hacer que si alguien entra por HTTP, la web lo redirija automáticamente a HTTPS. | 2 | Gabriel | Done |
| SMAR-45 | Data Isolation | T-45-1 | Campo de Empresa | Agregar la columna "Empresa_Id" en todas las tablas para separar los datos de cada cliente. | 6 | Imanol | Done |
| SMAR-45 | Data Isolation | T-45-2 | Filtro de Consultas | Programar la lógica para que un usuario solo pueda ver los registros de su "Empresa_Id". | 8 | Imanol | Done |
| SMAR-01 | Login estándar | T-01-1 | Maquetado de Login | Crear la página visual (HTML/CSS) con el formulario de correo y contraseña responsivo. | 5 | Johan | Done |
| SMAR-01 | Login estándar | T-01-2 | Conexión Backend | Programar el endpoint que recibe datos del formulario y valida si el usuario existe. | 6 | Johan | Done |
| SMAR-03 | Creación usuarios | T-03-1 | Formulario Registro | Diseñar la interfaz para que el Admin pueda ingresar datos de nuevos empleados. | 5 | Gabriel | Done |
| SMAR-03 | Creación usuarios | T-03-2 | Guardado Usuario | Crear función que inserta al nuevo usuario validando que el correo no esté repetido. | 5 | Gabriel | Done |
| SMAR-04 | Asignación roles | T-04-1 | Tabla de Roles | Crear en la base de datos los niveles (Admin, Staff, Monitor) y asignarlos. | 4 | Johan | Done |
| SMAR-04 | Asignación roles | T-04-2 | Control de Accesos | Programar que ciertas páginas o botones solo se activen si se tiene el rol adecuado. | 6 | Johan | Done |
| SMAR-23 | Reset de clave | T-23-1 | Envío de Correo | Integrar servicio de AWS para que el sistema envíe mail automático al pedir el reset. | 6 | Imanol | Done |
| SMAR-23 | Reset de clave | T-23-2 | Link Temporal | Crear página donde el usuario escriba su nueva clave usando enlace que expire en 1 hora. | 5 | Imanol | Done |
| SMAR-26 | Cierre de sesión | T-26-1 | Botón de Salir | Programar la acción que borre los datos de sesión guardados en el navegador. | 2 | Imanol | Done |
| SMAR-26 | Cierre de sesión | T-26-2 | Limpieza de Token | Asegurar que el servidor rechace el token anterior una vez que el usuario cerró sesión. | 4 | Imanol | Done |
| SMAR-44 | Anti-Brute Force | T-44-1 | Contador Fallos | Programar un contador que identifique si una persona falla su clave más de 5 veces. | 5 | Juan | Done |
| SMAR-44 | Anti-Brute Force | T-44-2 | Bloqueo por tiempo | Impedir el acceso a esa cuenta por 15 minutos tras los fallos detectados. | 4 | Juan | Done |
| SMAR-51 | Complejidad clave | T-51-1 | Reglas de Clave | Crear validaciones para clave segura (mínimo 8 letras, número y símbolo). | 3 | Gabriel | Done |
| SMAR-51 | Complejidad clave | T-51-2 | Mensajes de Error | Mostrar mensajes en rojo al usuario si su clave es muy débil mientras la escribe. | 3 | Gabriel | Done |
| SMAR-81 | Manejo Errores | T-81-1 | Pantalla de Error | Crear alerta amigable para cuando el servidor falle, sin mostrar código técnico. | 5 | Johan | Done |
| SMAR-81 | Manejo Errores | T-81-2 | Auditoría Interna | Configurar que el sistema guarde un archivo log con los errores reales para revisión. | 4 | Johan | Done |
| SMAR-82 | CORS Policy | T-82-1 | Permisos Dominio | Configurar el sistema para que solo acepte peticiones desde tu web oficial. | 3 | Gabriel | Done |
| SMAR-82 | CORS Policy | T-82-2 | Cabeceras Seguras | Definir qué acciones HTTP (GET, POST, DELETE) están permitidas. | 3 | Gabriel | Done |
| **TOTAL HORAS** | | | | | **105** | | |

## 5.3. Validation Interviews.
### 5.3.1. Diseño de Entrevistas.
### 5.3.2. Registro de Entrevistas.
### 5.3.3. Evaluaciones según heurísticas.

## 5.4. Video About-the-Product.

# Anexos

* **2.4. y 2.6.1. Event Storming (Big Picture & Design Level):** [Excalidraw](https://excalidraw.com/#json=vUgvQ_f8p5qxOvlqhFRzb,fcVt4lcEfKf0J_ePWUhZhw)
* **2.3. User Personas y Community:** [Figma Board](https://www.figma.com/board/okEnho158yZOcK5r6UzEgj/user-personal--Community-?node-id=0-1&t=y2q6BjfRkX2B6Mr1-1)
* **Landing Page y Web Application Design:** [Figma Design](https://www.figma.com/design/kVDoKtb6qnhzGb0kD1rCyR/Untitled?node-id=14-2537&t=k6bdmNtl5T5W5I9Q-1)
* **3.3. Gestión del Proyecto y Backlog:** [Jira Board](https://upc-team-open-source.atlassian.net/jira/software/projects/SMAR/boards/1?atlOrigin=eyJpIjoiNDFhNzk1OTIxMGU0NDc5ZjlmYjliMzlmYjU2MDVmOTIiLCJwIjoiaiJ9)

* Evidencia de herramienta utilizada : Jira :

* <img src="/Resources/Ending/Herramientas/story_points.png" alt="Story Points" width="500"> 

* <img src="/Resources/Ending/Herramientas/formato.png" alt="Formato de HU" width="500"/> 

* <img src="/Resources/Ending/Herramientas/organizacion.png" alt="Estructura de prioridad" width="500"/> 

* <img src="/Resources/Ending/Herramientas/Sprint.png" alt="Sprint" width="500"/> 

# Bibliografia
