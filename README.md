Argentina programa 2daparte Proyecto integrador parte Backend - Guido Pilato - #YoProgramo

Se linkeó el backend y la bd para que permanezcan online. Se crean tablas correctamente y se añadió un usuario para login Se usó #Heroku y #Netbeans #Argentinaprograma

----

Podés encontrar la app completa en https://frontendguidopilato.web.app/

El Backend :
Podés encontrar el Backend en : https://backendguidopilato.herokuapp.com/

El Frontend :
Podés encontrar el frontend en : https://frontendguidopilato.web.app/

Github Backend
https://github.com/guidopilato/Proyectointegrador_GuidoPilato_BackEnd

Github Frontend
https://github.com/guidopilato/Proyectointegrador_GuidoPilato_FrontEnd

El Deploy está subido,
las distintas capas del proyecto integrador se encuentran disponibles en la nube,
utilizando HEROKU (para Back End Spring Boot) y Clever Cloud (para la Base de Datos MYSQL). 

**Diagrama Entidad - Relación** (DER) utilizado en la Base de Datos Relacional y que posteriormente se traduce en los Modelos o Entidades del Backend:

<div align="center">
<img src="https://github.com/guidopilato/Proyectointegrador_GuidoPilato_BackEnd/blob/master/MySQLWorkbench.png" width="400px">
</div>

------

## Instalación
- Si queres correr la aplicación en un entorno local tenes que tener en cuenta lo siguiente: 

1. Clonar el repositorio utilizando GIT o descargando el archivo ZIP:

    `git clone https://github.com/guidopilato/Proyectointegrador_GuidoPilato_BackEnd.git`

2. Instalar las dependencias de Maven utilizando nuestro IDE preferido o a través del comando:

    `mvn install`

3. Crear/Configurar el archivo _application.properties_ en src/main/resources/

```properties
# Ambiente de prueba (local)
spring.jpa.hibernate.ddl-auto = update
spring.datasource.url = jdbc:mysql://<host_DB>:<puerto_DB>/<nombre_DB>?useSSL=false&serverTimezone=UTC
spring.datasource.username = <usuario>
spring.datasource.password= <contraseña>
spring.jpa.database-platform = org.hibernate.dialect.MySQL8Dialect
#JWT
portfolio.jwtSecret = <clave_alfanumérica_JWT>
portfolio.jwtExpirationMs = <tiempo_expiración_JWT> 
```
NOTA: Reemplazar los valores borrando los <>.

4. Ejecutar la aplicación iniciando el archivo `GPApplication.Java` o bien ejecutando el siguiente comando:
    `mvn sprin-boot:run`
