# PROYECTO STHOR

## STHOR

Es un proyecto de software gratuito creado para la gestion de almacenes, puede ser utilizado por cualquier entidad  en caso de adaptarse al producto y el uso del mismo no involucra un pago de licencia.


## Colores / Temas

* (Light) Blanco , Verde Olivo y Verde Oscuro.
* (Dark)  Negro , Blanco y Verde

## Instalacion de .Net Core 

Antes de continuar verificar que se tiene instalado .Net Core 2.2 en https://dotnet.microsoft.com/download

```sh
# verficar version instalada
root@debian$ dotnet --version
2.2.203
```


## Descarga Sthor

Windows y Linux
* http://github.com/alanwalter45/0.1/sthor.zip


```sh
# Desde la ruta de descarga abrir la terminal :
# Ejcutar como un proceso
root@debian/sthor0.1$ dotnet server.dll 

# O si deseas Ejecutar con el gestor de modulos PM2 usa
root@debian/sthorv0.1$ pm2 start "dotnet server.dll" --name tu_aplicacion 
```
```sh
# verificar el aplicativo
root@debian$ curl localhost:8080
```


## Interfaz Programable de Aplicaciones - API

La documentacion de la Interfaz Programable de Aplicaciones usado para este sistema esta detallada en http://github.com/alanwalter45/apidoc-sthor/index.html

aunque se usa swagger para la documentacion y esta es interactiva pero muy tecnica , asi que se disponibiliza un manual de usuario en http://github.com/alanwalter45/apidoc-sthor/manual.pdf

<br>

> copyright@2019
<a href="http://alanwalter45@gmail.com" target="_blank">
 @alanwalter45
 </a>