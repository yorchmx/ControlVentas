1. Generar resumen ejecutivo que cuente con los siguientes elementos en el archivo README.md dentro del repositorio:

a. Descripción, problema identificado, solución, arquitectura
Descripción:


Problema identificado:

Los empleados de banquetes del Club France al realizar eventos, venden boletos y la relación de ventas la hacen en Excel y las hacen en varios archivos, por lo cual aveces propicia que se duplique la información. 

Solución:

Se plantea desarrollar una aplicación web la cual por medio de un formulario permita almacenar en una base de datos MySql o PostgreSQL la información de las ventas para el evento.

Arquitectura:

La arquitectuta de la aplicación es la siguiente:

- Cliente
- Petición HTTP
- Servidor
- Servidor BD

b. Tabla de contenidos (ToC) con enlaces o a la sección wiki dentro del repositorio o algún medio externo como ReadTheDocs.io

https://github.com/yorchmx/ControlVentas/wiki/Tabla-de-contenidos


2. Requerimientos:

a. Servidores de aplicación, web, bases de datos, etc.

- Glassfish
- MySql
- Conector JDBC

b. Paquetes adicionales.

-  Descargar las librerias del conector JDBC

c. Versión de Java, etc.

Java 8



3. Instalación:

a. ¿Cómo instalar el ambiente de desarrollo?

1. Realizar una base de datos en MySql llamada control_clientes
2. Crear una tabla llamada clientes
3. Ingresar las siguientes columnas: id_cliente, nombre, apellido, email, telefono, saldo

   
4. Descargar el fichero de este repositorio
https://github.com/yorchmx/ControlVentas.git

5. Cargar el proyecto en NetBeans
6. Hacer deploy


b. ¿Cómo ejecutar pruebas manualmente?


c. ¿Cómo implementar la solución en producción en un ambiente local o en la nube como Heroku?

En Heroku se tiene que dar de alta una nueva app y generar una base de datos en PostgreSQL, crear una base de datos y generar la tabla clientes con las columnas id_cliente, nombre, apellido, email, telefono, saldo.

Configurar el archivo pom.xml para el conector de base de datos Postgresql.
Configurar el archivo Conexion.java con el servidor de Heroku, el nombre de la base de datos y contraseña que genera Heroku.


4. Configuración:

a. Configuración del producto (archivos de configuración).
    
    Configurar el archivo pom.xml con las siguientes dependencias
    
     <dependencies>
        <dependency>
            <groupId>javax</groupId>
            <artifactId>javaee-api</artifactId>
            <version>${jakartaee}</version>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>mysql</groupId>
            <artifactId>mysql-connector-java</artifactId>
            <version>8.0.22</version>
        </dependency>
        <dependency>
            <groupId>org.apache.commons</groupId>
            <artifactId>commons-dbcp2</artifactId>
            <version>2.7.0</version>
        </dependency>
    </dependencies>
    
    
b. Configuración de los requerimientos.

5. Uso:

a. Sección de referencia para usuario final. Manual que se hará referencia para usuarios finales.
b. Sección de referencia para usuario administrador.

6. Contribución:

a. Guía de contribución para usuarios.
b. Debe contar con pasos específicos para clonar repositorio, crear un nuevo branch, enviar el pull request, esperar a hacer el merge.

7. Roadmap:

a. Requerimientos que se implementarán en un futuro.
