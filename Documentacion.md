# Indice

#### __EvalúaMe: Intranet de Autoevaluación y Coevaluación Estudiantil__	1
* Escenario del proyecto	3
* Requisitos del proyecto y casos de uso general	3
* Casos de uso general	3
* Fases de desarrollo	4
* Versiones	5
__Backlog de Producto y Sprint para "EvalúaMe: Intranet de Autoevaluación y Coevaluación Estudiantil"__	6
#### SPRINT 0: Definición del Proyecto	6
* Historia: Requisitos, Casos de Uso y Diagrama de Casos de Uso	6
* Historia: Versiones y Planificación	6
* Historia: Casos de Uso Específicos y Diagramas de Flujo	6
#### SPRINT 1: Diseño de la Interfaz	6
* Historia: Bocetos	6
* Historia: Wireframes, Mockups y Guía de Estilos	6
#### SPRINT 2: Prototipos	7
* Historia: Entorno de Desarrollo	7
* Historia: Prototipos HTML	7
* Historia: Validaciones de Formularios	7
#### SPRINT 3: Implementación de la SPA (Single Page Application)	7
* Historia: Configuración del Entorno basado en NodeJS	7
* Historia: Organización de Archivos y Vistas	7
* Historia: Creación de Componentes	7
* Historia: Navegación por las Vistas	7
* Historia: Validación de Formularios en Tiempo Real	7
* Historia: Autenticación de Usuarios	8
* Historia: Personalización de la Interfaz según el Rol	8
* Historia: Simulación con Datos Ficticios	8
* Historia: Administración de Usuarios y Proyectos	8
#### SPRINT 4: Backend	8
* Historia: Diseño de la Base de Datos	8
* Historia: Implementación en Supabase	8
* Historia: Uso de la API de JavaScript de Supabase	8
* Historia: Implementación de un ORM en JavaScript	8
#### SPRINT 5: Integración del Frontend y Backend	9
* Historia: Registro e Inicio de Sesión	9
* Historia: Gestión de Sesiones y Roles	9
* Historia: Edición de Perfil	9
* Historia: Publicación y Gestión de Proyectos	9
* Historia: Administración de Usuarios	9
#### SPRINT 6: Revisión y Despliegue en Producción de la Versión 1.0	9
* Historia: Pruebas de Usuario	9
* Historia: Corrección y Mejora	9
* Historia: Despliegue en Producción	9
### VERSIÓN 2.0: Implementación de las Coevaluaciones entre Estudiantes	11
#### SPRINT 1: Diseño y Planificación de la Funcionalidad de Coevaluación	11
* Historia: Definición de Casos de Uso y Diagramas de Flujo para Coevaluaciones	11
* Historia: Actualización de la Interfaz de Usuario	11
* Historia: Actualización de la Guía de Estilos	11
#### SPRINT 2: Desarrollo de la Funcionalidad de Coevaluación	11
* Historia: Visualización de Proyectos de Compañeros	11
* Historia: Formulario de Coevaluación	11
* Historia: Validaciones y Reglas de Negocio	11
* Historia: Actualización del Backend para Soportar Coevaluaciones	11
#### SPRINT 3: Integración y Pruebas	11
* Historia: Integración del Frontend y Backend para Coevaluaciones	12
* Historia: Notificaciones y Feedback	12
* Historia: Pruebas de Usabilidad y Correcciones	12
* Historia: Despliegue de la Versión 2.0	12
### VERSIÓN 3.0: Implementación de un Sistema Avanzado de Evaluación Basado en Rúbricas y Criterios Personalizados	12
#### SPRINT 1: Definición y Configuración de Rúbricas	12
* Historia: Definición de Criterios de Evaluación	12
* Historia: Asignación de Rúbricas a Proyectos	12
* Historia: Diseño de la Interfaz para Rúbricas	12
#### SPRINT 2: Desarrollo del Sistema de Evaluación con Rúbricas	12
* Historia: Implementación de Formularios de Evaluación con Rúbricas	13
* Historia: Autoevaluación Basada en Rúbricas	13
* Historia: Actualización del Backend para Soportar Rúbricas	13
#### SPRINT 3: Análisis y Reportes	13
* Historia: Visualización de Resultados de Evaluación	13
* Historia: Reportes para el Profesor	13
* Historia: Feedback Automatizado	13
#### SPRINT 4: Integración Final y Mejora Continua	13
* Historia: Mejoras en la Experiencia de Usuario	13
* Historia: Pruebas de Usabilidad y Correcciones	13
* Historia: Despliegue de la Versión 3.0	13
* Resumen de Versiones y Funcionalidades	14

### Escenario del proyecto
El profesor Juan Martínez es docente en el Instituto Tecnológico ABC y está interesado en mejorar el proceso de evaluación de sus alumnos en las asignaturas de programación y desarrollo web. Actualmente, las evaluaciones se realizan de manera tradicional, lo que limita la retroalimentación y la participación activa de los estudiantes en su propio proceso de aprendizaje.
Con el objetivo de fomentar la autoevaluación y la coevaluación entre los estudiantes, el profesor desea implementar una intranet educativa. Esta plataforma permitirá a los alumnos publicar sus proyectos, realizar autoevaluaciones y recibir evaluaciones de sus compañeros. De esta manera, se busca promover un ambiente colaborativo y enriquecedor que mejore el desempeño académico y las habilidades críticas de los estudiantes.
Hasta ahora, el profesor ha utilizado herramientas básicas como correos electrónicos y documentos compartidos para recopilar y comentar los proyectos de los alumnos. Sin embargo, reconoce la necesidad de una solución más integrada y eficiente que facilite el proceso de evaluación y comunicación entre todos los participantes.
Como estudiante en prácticas, tu tarea es desarrollar una aplicación web que sirva como intranet para el profesor y sus alumnos. Esta plataforma permitirá la publicación de proyectos, la realización de autoevaluaciones y coevaluaciones, y la gestión de usuarios y roles dentro del sistema.
### Requisitos del proyecto y casos de uso general
Los casos de uso describen cómo los usuarios interactuarán con el sistema y qué funcionalidades estarán disponibles para cada rol.
### Casos de uso general
La aplicación web debe permitir a un usuario registrarse con su nombre, apellidos, correo electrónico y contraseña, y posteriormente iniciar y cerrar sesión. Un usuario registrado podrá ver un listado de proyectos publicados por otros estudiantes, editar su perfil y subir una imagen de avatar.
Si el usuario registrado tiene el rol de 'estudiante', podrá:
- Publicar sus propios proyectos con información como: título del proyecto, descripción, imágenes representativas, enlaces al código fuente o demos, estado del proyecto, etc.
- Editar o eliminar sus proyectos publicados.
- Realizar autoevaluaciones de sus proyectos basadas en criterios establecidos.
- Evaluar los proyectos de sus compañeros mediante coevaluaciones, proporcionando comentarios y valoraciones.
El profesor, con el rol de 'administrador', podrá:
- Gestionar los perfiles de todos los usuarios registrados en la plataforma (editar, borrar, asignar roles, etc.).
- Revisar y moderar los comentarios y evaluaciones realizadas por los estudiantes.
- Establecer los criterios y rúbricas de evaluación que se utilizarán en las autoevaluaciones y coevaluaciones.
- Acceder a reportes y estadísticas sobre el desempeño de los estudiantes y la interacción en la plataforma.
### Fases de desarrollo
Para organizar el desarrollo del proyecto y cumplir con los objetivos establecidos, seguiremos las siguientes fases:
1. __Definición del proyecto y requisitos básicos:__ Clarificar las expectativas de la aplicación y anotar cada funcionalidad considerando los diferentes roles de acceso.
2. __Definición de las versiones:__ Dividir el trabajo en versiones operativas, cada una ampliando las funcionalidades de la anterior.
3. __Planificación del proyecto:__ Utilizando la metodología Agile, dividir el proceso en historias y tareas para cada versión, asignar tiempos y representarlas mediante diagramas.
4. __Diseño de la interfaz:__
* Realizar un benchmarking para inspirarse en soluciones similares.
* Crear un modelo de usuarios.
* Diseñar prototipos de baja fidelidad (bocetos, wireframes).
* Desarrollar un mockup de alta fidelidad junto con una guía de estilos utilizando Figma.
* Realizar pruebas de usabilidad y ajustar los prototipos según los resultados.
5. __Programación del frontend (HTML/CSS/JS):__
* Maquetar los prototipos en código.
* Implementar la lógica de validación en el lado del cliente.
6. __Programación del backend:__
* Utilizar un Backend como Servicio (BaaS) como SUPABASE para:
  + Crear las bases de datos.
  + Diseñar consultas SQL y funciones en PostgreSQL.
* Programar un ORM en JavaScript para el mapeo de la base de datos.
7. __Integración de frontend y backend:__
- Desarrollar la aplicación SPA (Single Page Application) a partir de los prototipos.
- Implementar la lógica de acceso a la base de datos utilizando el ORM.
- Programar el resto de funcionalidades (gestión de sesiones, control de roles, etc.).
8. __Análisis de usabilidad II:__
- Realizar pruebas de usabilidad adicionales y solucionar posibles conflictos detectados.
9. __Testing y despliegue en producción:__
- Diseñar un sistema de testing para crear pruebas unitarias.
- Configurar un entorno DevOps para trabajar con Integración Continua y Despliegue Continuo (CI/CD).
- Desplegar en producción cada una de las versiones.
### Versiones
El desarrollo del proyecto se dividirá en las siguientes versiones basadas en las funcionalidades a implementar:
- __VERSIÓN 1.0:__ Implementación de la publicación de proyectos y autoevaluaciones.
- __VERSIÓN 2.0:__ Implementación de las coevaluaciones entre estudiantes.
- __VERSIÓN 3.0:__ Implementación de un sistema avanzado de evaluación basado en rúbricas y criterios personalizados establecidos por el profesor.



# Backlog de Producto y Sprint para "EvalúaMe: Intranet de Autoevaluación y Coevaluación Estudiantil"
Estas son las historias a planificar en la entrega de la versión 1 de nuestro proyecto, agrupadas por sprints:

## SPRINT 0: Definición del Proyecto
## Historia: Requisitos, Casos de Uso y Diagrama de Casos de Uso
__Como desarrollador__, quiero definir de manera general las especificaciones de la aplicación, incluyendo los requisitos y casos de uso, para comprender claramente las funcionalidades esperadas.
### Historia: Versiones y Planificación
Como desarrollador, quiero agrupar las especificaciones en versiones, definir las tareas necesarias y planificar todo el proceso de desarrollo del proyecto.
__Historia: Casos de Uso Específicos y Diagramas de Flujo__
__Como desarrollador__, quiero detallar las especificaciones y casos de uso para la versión 1.0, creando diagramas de flujo para visualizar los procesos.
Nota: Esta historia ya ha comenzado a trabajarse en apartados anteriores. Sin embargo, es importante incluirla para valorar el tiempo total invertido.

## SPRINT 1: Diseño de la Interfaz
#### Historia: Bocetos
__Como diseñador__, quiero dibujar los bocetos de todas las pantallas potenciales del proyecto y probar su funcionamiento para asegurar una experiencia de usuario intuitiva.
Historia: Wireframes, Mockups y Guía de Estilos
Como diseñador, quiero crear wireframes y mockups, además de elaborar una guía de estilos basada en los colores, tipografías y elementos visuales seleccionados.

## SPRINT 2: Prototipos
#### Historia: Entorno de Desarrollo
__Como desarrollador__, quiero instalar y configurar las herramientas necesarias para programar la aplicación, gestionar repositorios y establecer un entorno de Integración Continua y Despliegue Continuo (CI/CD).
####  Historia: Prototipos HTML
__Como maquetador web__, quiero crear las páginas HTML del proyecto a partir de los wireframes, aplicando la guía de estilos y utilizando Bootstrap 5.
#### Historia: Validaciones de Formularios
__Como programador__, quiero definir e implementar las validaciones de los formularios para asegurar la integridad de los datos ingresados por los usuarios.

## SPRINT 3: Implementación de la SPA (Single Page Application)
#### Historia: Configuración del Entorno basado en NodeJS
__Como programador__, quiero instalar y configurar todas las herramientas necesarias (NodeJS, Vite, etc.) para desarrollar una aplicación SPA en JavaScript.
#### Historia: Organización de Archivos y Vistas
__Como programador__, quiero configurar la estructura de carpetas para las vistas y crear archivos basados en componentes HTML de los prototipos.
####  Historia: Creación de Componentes
__Como programador__, quiero desarrollar los componentes para el encabezado, el enrutamiento de páginas y los menús de navegación.
#### Historia: Navegación por las Vistas
__Como usuario__, quiero poder navegar por todas las vistas de la aplicación, independientemente de mi rol, para familiarizarme con la interfaz.
#### Historia: Validación de Formularios en Tiempo Real
__Como usuario__, quiero recibir retroalimentación inmediata en los formularios para corregir errores durante la entrada de datos.
#### Historia: Autenticación de Usuarios
__Como usuario registrado__, quiero que mis datos de sesión se recuerden al iniciar sesión (utilizando localStorage) para facilitar el acceso.
#### Historia: Personalización de la Interfaz según el Rol
__Como usuario logueado__, quiero que el encabezado y los menús se actualicen según mi rol, mostrando solo las opciones relevantes para mí.
#### Historia: Simulación con Datos Ficticios
__Como programador__, quiero simular el registro, inicio de sesión y visualización de datos utilizando archivos JSON de prueba.
#### Historia: Administración de Usuarios y Proyectos
__Como profesor (administrador)__, quiero poder gestionar los usuarios y proyectos (ver, editar, borrar) para mantener la plataforma actualizada.

## SPRINT 4: Backend
#### Historia: Diseño de la Base de Datos
__Como programador__, quiero diseñar la base de datos utilizando diagramas UML (Entidad-Relación) para estructurar adecuadamente la información.
#### Historia: Implementación en Supabase
__Como programador__, quiero implementar las tablas y funciones en Supabase, diseñando consultas y funciones PostgreSQL necesarias.
#### Historia: Uso de la API de JavaScript de Supabase
__Como programador__, quiero utilizar la API de JavaScript de Supabase para interactuar con la base de datos desde la aplicación.
#### Historia: Implementación de un ORM en JavaScript
__Como programador__, quiero desarrollar un ORM (Object-Relational Mapping) en JavaScript para facilitar el mapeo y manejo de datos de la base de datos.

## SPRINT 5: Integración del Frontend y Backend
Historia: Registro e Inicio de Sesión
__Como estudiante__, quiero poder registrarme y acceder al sistema para participar en las actividades de evaluación.
#### Historia: Gestión de Sesiones y Roles
__Como usuario registrado__, quiero que el sistema reconozca mi rol (estudiante o profesor) y adapte la interfaz y funcionalidades disponibles.
#### Historia: Edición de Perfil
__Como usuario registrado__, quiero poder ver y editar mi perfil, incluyendo la actualización de mi imagen de avatar.
#### Historia: Publicación y Gestión de Proyectos
__Como estudiante__, quiero poder publicar mis proyectos, ver detalles, editar y eliminar mis propios proyectos.
#### Historia: Administración de Usuarios
__Como profesor (administrador)__, quiero poder ver, editar y eliminar usuarios del sistema, así como asignar roles y permisos.

## SPRINT 6: Revisión y Despliegue en Producción de la Versión 1.0
#### Historia: Pruebas de Usuario
__Como diseñador__, quiero realizar pruebas de usabilidad con un grupo de usuarios para identificar áreas de mejora en la aplicación.
#### Historia: Corrección y Mejora
__Como programador__, quiero revisar y solucionar los problemas detectados durante las pruebas de usuario para optimizar la aplicación.
#### Historia: Despliegue en Producción
__Como programador__, quiero desplegar la aplicación en un entorno de producción para que esté accesible a todos los usuarios.

  ## Sprint 1 Diseño de la Interfaz

Historia de los bocetos: Nosotros dos hemos pensado en hacer una pagina web tipo foro de colegio para poder ver las publicaciones de los alumnos y sus opiniones.

Tenemos varias maquetas hechas en papel y boli para el borrador de nuestra pagina web. 

Aqui tenemos las fotos de los bocetos para nuestro foro de clase: 




