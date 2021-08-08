# **Ejercicios SQL Desarrollo y Gestión de BD Crehana**

Ejercicios realizados en el curso de SQL Desarrollo y gestión de bases de datos presentado por Crehana.

## **Introducción**

Este repositorio contiene los archivos/ejercicios que realice durante el curso de SQL provisto por la plataforma Crehana. Cabe destacar, que si bien el repositorio es publico, el mismo solo tiene el propósito de mostrar las formas en las que solvente problemas/actividades propuestas por el curso.

## **Requisitos**

<li>
<strong>Docker</strong>: Es un proyecto de Código Abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software, proporcionando una capa adicional de abstracción y automatización de virtualización de aplicaciones en múltiples sistemas operativos.
<ol><strong>Opcional:</strong> preferiblemente correlo en un servidor linux (no tu desktop) para disfrutar de un mejor rendimiento</ol>
</li>
<li><strong>Visual Studio Code</strong>: Es un editor de código fuente desarrollado por Microsoft para Windows, Linux y macOS. Incluye soporte para la depuración, control integrado de Git, resaltado de sintaxis, finalización inteligente de código, fragmentos y refactorización de código.
<ol><strong>Opcional:</strong> si no quieres usar PgAdmin para realizar las consultas de tu base de datos, puedes probar la extensión de VSCode <a href="https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools">SQLTools</a></ol></li>
<li><strong>Postgres:</strong> Es un sistema de gestión de bases de datos relacional orientado a objetos y de código abierto, publicado bajo la licencia PostgreSQL, ​ similar a la BSD o la MIT.</li>

## **Instalación**

Utiliza el docker-compose.yml para desplegar en tu servidor con Docker el stack de contenedores. Este stack contiene dos contenedores:

- Postgres (la base de datos SQL)
- PgAdmin

En el archivo docker-compose.yml debes establecer las variables de:

- Usuario de la Base de Datos
- Contraseña del Usuario de la BD (Base de Datos)
- Correo Administrativo para PgAdmin
- Contraseña Administrativa para PgAdmin

Con estos requisitos básicos podrás correr el stack sin muchos problemas, preferiblemente si es tu primera vez usando un stack de docker-compose, no cambies otros de los aspectos del ambiente.

Para desplegar el stack, debes utilizar en tu terminal el comando `docker-compose up -d`, explicación del comando:

    1. docker-compose: es una herramienta para definir y correr aplicaciones docker de multiples contenedores
    2. up: levanta todos los servicios del ambiente descrito en el archivo docker-compose.yml
    3. -d: es una opción para el comando docker-compose que significa 'detached', es decir, que el stack correrá en el fondo, sin ocupar espacio en tu terminal.
