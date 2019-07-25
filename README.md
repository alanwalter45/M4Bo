<img src="./assets/logotipo.png">

## Sistema generico para la gestion de almacenes.

## Idea general del proyecto

* Github page  : [sthor][1]

* Canal youtube : [youtube.com/alanwalter45/sthor][0]

## Licencia de software

<img width="100px" src="./assets/coffeeware-badge.png">

Leer licencia <a href="./LICENSE.md">aqui</a>.

## Caracteristicas generales

* Icono y Logotipo personalizables.
* Gestion de Almacen :
    * 10 Almacenes <code>(en el sistema)</code>.
    * 7 Usuarios <code>(en el sistema)</code>.
    * 6000 Logs / registros del sistema <code>(diariamente)</code>.
    * 5000 Articulos <code>(por almacen)</code>.
    * 3000 Proveedores <code>en el sistema</code>.
    * 3000 Receptores de articulos <code>(en el sistema)</code>.
* Alerta por colores segun cantidad en stock :
    * ROJO sin Stock.
    * AMARILLO tiene el stock minimo.
    * VERDE tiene stock suficiente.
    * Notificaciones via email segun color (ROJO, AMARILLO , VERDE).
* Paleta de 10 Articulos favoritos.
* Codigo de Barras para los articulos.
* Ubicacion de los articulos <code>rack/secciones doble fila</code>.
* Resguardo de articulos ajenos <code>documentos de pruebas</code>.
* Separar articulos por lotes <code>agrupar articulos</code>.
* Archivos de autenticidad <code>documentos digitales de la adquisicion de articulos</code>.
* Recordar completar entrega <code>cantidad imcompleta de articulos</code>.
* Recordar completar reposiciones <code>reponer articulos a receptores de articulos</code>.
* Control de acceso (seguridad) al almacen <code>planilla de asistencia</code>.
* Parametros del sistema configurable <code>(archivos de configuracion servidor y cliente)</code>.
    * Formatos : YML , JS , JSON
* Base de Datos SQLITE <code><code>(sin configuracion y portable)</code></code>.
* Frontend VUEJS <code>(capa de usuario)</code>.
* Autenticacion basada en Tokens (JWT).
* Operadores o Usuarios :
    * 1 Usuario por defecto <code>(Administrador)</code>.
    * 6 Usuarios gestionables por un usuario administrador.
    * Tipos de usuarios <code>(Administrador, Operador)</code>
    * Contrasenas modificables pero no recordables <code>(Hashes)</code>.
* Valores o Resultados :
    * Graficas Circulares.
    * Comparacion Mensual.
* Reportes :
    * PDF formato de impresion.
*Enportacion de datos :
    * XLSX - Excel.
    * TXT - Texto.
* Metodos de inventario:
    * PEPS (PRIMERO EN ENTRAR PRIMERO EN SALIR) FIFO.
    * UEPS (ULTIMO EN ENTRAR PRIMERO EN SALIR) LIFO.
    * PP (PRECIO PROMEDIO) PRO.
* Consultas en linea (1 periodo) :
    * Por Proveedor.
    * Por Articulo.
    * Por Almacen.
* Respaldo y restauracion de informacion (Backups).
* Logs de acciones realizadas <code>(registros del sistema)</code>.
* Idiomas Soportados
    * Espanol.
    * Ingles.
* Temas o Estilos 
    * Colores, fuentes , paneles
        * Light / Iluminado
        * Black / Oscuro


## Instalacion

Descarga la pataforma que necesites :

* <a href="src/sthor.zip" download>Windows</a> 64bit.

* <a href="src/sthor.zip" download>Linux</a> 64bit.


Descomprima el archivo y abra la terminal desde la ruta descomprimida

```sh
# ejecutar STHOR
root@debian:~/sthor$ ./sthor
# verificar el aplicativo usando el folder SHORTCUTS o con el comando CURL.
root@debian:~/sthor$ curl localhost:5000
```

Requisitos de sistema

```sh
# instalacion de PM2 https://www.npmjs.com/package/pm2
# verificar instalacion de PM2
root@debian:~/sthor$ pm2 --version # ...PM2 opcional
```

## Comentarios? Preguntas? Preocupaciones?
canal en discord : https://discord.gg/AaNK56A
<br>
email : alanwalter45@gmail.com

[0]:https://www.youtube.com/playlist?list=PLCGw6KEqh5zEhAPkQbcocWWxXfl_tbgD-
[1]:https://alanwalter45.github.io/sthor