# training-security-notes-webapp

Proyecto de ejemplo para formación sobre seguridad en aplicaciones web.

Basado en: [https://www.adictosaltrabajo.com/2012/07/30/spring-mvc-api-rest-oauth-2/](https://www.adictosaltrabajo.com/2012/07/30/spring-mvc-api-rest-oauth-2/)

#### Entorno

- Java 1.8
- Maven 3.5
- Tomcat 7

#### Compilación

`mvn clean install  -Dmaven.test.skip=true`

#### Ejecución

`mvn tomcat7:run -X -Dmaven.tomcat.port=9080`
 
## Aplicación web Small Notes

Aplicación web sin securizar que accede a la API de la aplicación Small Notes. El usuario conectado está mockeado para este estado inicial sin seguridad.

#### Prueba
	
Probar la aplicación sin seguridad accediendo a: `http://localhost:9080/smallNotesExternalWebApp/home`

## Ejercicio

Preparar la aplicación web mediante configuración **Spring Security** aplicando **OAuth2** para el acceso a la API securizada Small Notes.

#### Acciones
	
- Añadir los filtros de securidad en `web.xml`.
- Modificar el RestTemplate en spring context para acceder a una API securizada OAuth2.

Finalmente probar el acceso a la API securizada con OAuth2.

Esta API está en:

[https://github.com/mazingergonzalez/training-security-notes-api](https://github.com/mazingergonzalez/training-security-notes-api)


