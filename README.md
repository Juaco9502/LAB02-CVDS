#Apache Maven
###Por: Juan Camilo Ortiz
##1. Cuál es su mayor utilidad
Apache Maven es una herramienta de gestión y comprensión de proyectos de software. Basado en el concepto de un modelo de objeto de proyecto (POM), Maven puede administrar la construcción, los informes y la documentación de un proyecto a partir de una información central.

##2. Fases de maven

- ***validate:*** Que valida que el proyecto es correcto y que está disponible toda la información necesaria
- ***compile:*** Que compila el código fuente del proyecto
- ***test:*** Que prueba el código compilado utilizando algún framework de pruebas unitarias. Estas pruebas no deben requerir que el código esté empaquetado o desplegado.
- ***package:*** Coge el código compilado y lo empaqueta en un formato distribuible. Por ejemplo, como un JAR.
- ***verify:*** Ejecuta comprobaciones de pruebas de integración para asegurarse que se cumplen los criterios de calidad.
- ***install:*** Instala el paquete en el repositorio local (el directorio ${user.home}/.m2) para que se pueda usar como dependencia en otros proyectos localmente.
- ***deploy:*** Copia el paquete final a un repositorio remoto para compartirlo con otros desarrolladores. Hay que tener en cuenta que este despliegue no se refiere en general al despliegue de la aplicación en un servidor web, sino a dejarlo disponible en un repositorio para que lo usen otros desarrolladores

##3. Ciclo de vida de la construcción

En Maven se definen tres ciclos de vida por defecto y normalmente nunca te vas a ver en la necesidad de definir ninguno adicional. Los tres ciclos de vida de Maven son:
- El ciclo de vida default, que gestiona la construcción y despliegue del proyecto.
- El ciclo de vida clean, que gestiona la limpieza del directorio del proyecto. Es decir, se encarga de eliminar todos los archivos generados en el proceso de construcción y despliegue.
- El ciclo de vida site, que gestiona la creación de la documentación del proyecto.

##4. Para qué sirven los plugins

Un Plugin es un fragmento o componente de código hecho para ampliar las funciones de un programa o de una herramienta. En el ámbito del marketing digital, sobre todo dentro del marketing de contenidos, es algo que se usa con mucha frecuencia dentro de entornos como WordPress, ya que sirven a la hora de contar con añadidos que hagan mucho más cómoda y completa la experiencia de uso.

##5. Qué es y para qué sirve el repositorio central de maven

Es un repositorio proporcionado por la comunidad de Maven. Contiene una gran cantidad de bibliotecas de uso común.
Cuando Maven no encuentra ninguna dependencia en el repositorio local, comienza a buscar en el repositorio central utilizando la siguiente URL: https://repo1.maven.org/maven2/
Los conceptos clave del repositorio central son los siguientes:
- Este repositorio es administrado por la comunidad Maven.
- No es necesario que se configure.
- Requiere acceso a internet para ser buscado.