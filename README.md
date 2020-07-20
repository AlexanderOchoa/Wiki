# mi-proyecto

### Tabla de contenido
- [Descripción](#markdown-header-descripcion)  
- [Comunicación con otros proyectos](#markdown-header-comunicacion-con-otros-proyectos)
- [Pre-requisitos para correr la aplicación](#markdown-header-pre-requisitos-para-correr-la-aplicacion)  
- [Despliegue](#markdown-header-despliegue)  
- [Construido con](#markdown-header-construido-con)  
- [Uso de Git](#markdown-header-uso-de-git)  
- [Licencia](#markdown-header-licencia)

----------

### Descripción
El proyecto permite:

xxx

----------

### Comunicación con otros proyectos
* **mi-servicio-b**: Permite obtener datos de b

----------

### Pre-requisitos para correr la aplicación
- Descargar las fuentes de Bitbucket  
- Descargar las dependencias (Maven)  
- Tener conexión abierta con MongoDB
- Tener conexión abierta al servidor de archivos de configuración (Spring Config Server)
- Correr el proyecto

----------

### Despliegue
Existen dos formas de despliegue: manual y automático

----------

### Construido con
* ***Java 1.8 (spring boot 2.0.5.RELEASE)*** - Lenguaje base de toda la aplicación  
	* ***RestTemplate***: Clase de Spring para peticiones HTTP (Comunicación con servicios externos)
* ***Maven*** - Gestor de dependencias  
* ***MongoDB*** - Base de datos no relacional de la aplicación  
	* ***MongoTemplate***: Implementación de MongoDB para realizar operaciones contra la base de datos
* ***Spring Cloud*** - Configuración del proyecto  
	* ***Spring Config Server Client***: Permite obtener el archivo de configuración (.properties) del servidor centralizado
	* ***Hystrix***: Librería para tolerancia a fallos, manejo de errores en consumo de servicios externos

----------

### Uso de Git
**Ramas**

La estructura de ramas del proyecto sigue la siguiente distribución: ***master***, ***develop*** y ***features***
Cada *feature* representa un sprint y está definido por *feature/nombreSprint-funcionalidadPrincipal*

**Tags**

Cada vez que se fusiona un feature hacia develop se genera una tag (representa un punto estable de la aplicación) y está definido por *añoMesDía_horaMinutos*

**Commits**

Para el uso de comentarios se sigue la siguiente fórmula:

* ***feat***: Una nueva característica
ejemplo: feat (sprintX): nueva funcionalidad x

* **fix**: Se solucionó un bug
ejemplo: fix (sprintX): error al obtener datos de cliente

* **docs**: Se realizaron cambios en la documentación
ejemplo: docs (sprintX): manejo de versiones

* **style**: Se aplico formato, comas y puntos faltantes
ejemplo: style (sprintX): correccion de textos

* **refactor**: Refactorizacion del codigo
ejemplo: refactor (sprintX): mejora de codigo

* **test**: Se añadieron pruebas, refactorizacion de pruebas, sin cambios en el código
ejemplo: test (sprintX): administracion de clientes

* **chore**: Actualizacion de tareas de build, sin cambios en el código
ejemplo: chore (sprintX): cambios en el pipeline

----------

### Licencia
xxx
