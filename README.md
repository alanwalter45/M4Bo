
# Proyecto Sthor

<img src="./assets/favicon.ico">

## STHOR

Es un proyecto de software gratuito creado para la gestion de almacenes.

<img src="./assets/logotipo.png">

## Caracteristicas generales del sistema

* Icono y Logotipo personalizable.
* Gestion de Almacen :
    * 10 Almacenes <code>(sistema)</code>.
    * 7 Usuarios <code>(sistema)</code>.
    * 6000 logs / registros del sistema <code>(diario)</code>.
* Parametros del sistema configurable <code>(archivos de configuracion servidor y cliente)</code>.
    * Formatos : YML , JS , JSON
* Base de Datos SQLITE <code><code>(sin configuracion y portable)</code></code>.
* Frontend VUEJS <code>(capa de usuario)</code>.
* Autenticacion basada en Tokens (JWT).
* Operadores o Usuarios:
    * 1 Usuario por defecto <code>(Administrador)</code>.
    * 6 Usuarios gestionables por un usuario administrador.
    * Tipos de usuarios <code>(Administrador,Normal)</code>
    * Contrasenas modificables pero no recordables <code>(Hashes)</code>.
* Reportes :
    * PDF formato de impresion.
* Metodos de inventario:
    * PEPS (PRIMERO EN ENTRAR PRIMERO EN SALIR).
* Consultas en linea (1 periodo) :
    * Por Articulo.
* Logs de acciones realizadas <code>(registros del sistema)</code>.
* Idiomas Soportados
    * Espanol.
* 2 Temas o Estilos 
    * Colores, fuentes , paneles
        * Light o Iluminado
        * Black u Oscuro

## Arquitectura de Software

<img width="600px" src="assets/arquitectura.png">

## Descarga de Sthor

Sthor es un sistema para la gestion de almacenes , distribuido por el momento en formato zip <a href="src/sthor.zip" download>aqui</a> .

## Instalacion de .Net Core 

Antes de continuar verificar que se tiene instalado .Net Core 2.2 en <a href="https://dotnet.microsoft.com/download">microsoft/download</a>

```sh
# verficar version instalada
root@debian$ dotnet --version
2.2.203

# Desde la ruta de descarga abrir la terminal :
# Ejcutar como un proceso
root@debian/sthor0.1$ dotnet server.dll 

# O si deseas Ejecutar con el gestor de modulos PM2 usa
root@debian/sthorv0.1$ pm2 start "dotnet server.dll" --name tu_aplicacion 

# verificar el aplicativo
root@debian$ curl localhost:8080
```


## Interfaz de Programacion de Aplicaciones - API

La documentacion de la API utilizada para la construccion del sistema esta detallada <a href="apidoc-sthor/index.html">aqui</a>  y aunque se utiliza swagger para documentar se disponibiliza un manual de usuario <a href="src/manual.pdf" download>aqui</a>.

## Comentarios? Preguntas? Preocupaciones?
canal en discord : https://discord.gg/AaNK56A
<br>
email : alanwalter45@gmail.com