# Proyecto Sthor
<img src="./assets/logotipo.png">

Es un proyecto de software gratuito creado para la gestion de almacenes.


## Licencia de Software

<img width="100px" src="./assets/coffeeware-badge.png">

Leer <a href="./LICENSE.md">licencia</a>

## Caracteristicas generales del sistema

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
* Incluye informacion de Proveedores, Receptores y Usuarios.

## Arquitectura de Software

<img width="600px" src="assets/arquitectura.png">

## Descarga de Sthor

Sthor es distribuido en formato zip <a href="src/sthor.zip" download>aqui</a> .

## Plataforma de desarrollo .Net Core 

Antes de continuar verificar que se tiene instalado .Net Core 2.2 en <a href="https://dotnet.microsoft.com/download">microsoft/download</a>

```sh
# verficar version instalada
root@debian/stror: dotnet --version
2.2.203

# Desde la ruta de descarga abrir la terminal :
# Ejcutar como un proceso
root@debian/sthor: dotnet server.dll 

# O si deseas Ejecutar con el gestor de modulos PM2 usa
root@debian/sthor: pm2 start "dotnet server.dll" --name sthor_1 

# verificar el aplicativo
root@debian: curl localhost:8080
```


## Documentacion

La documentacion de la API utilizada para la construccion del sistema esta detallada <a href="apidoc-sthor/index.html">aqui</a>  
Se utiliza swagger para documentar y se disponibiliza un manual de usuario <a href="src/manual.pdf" download>aqui</a>.

## Comentarios? Preguntas? Preocupaciones?
canal en discord : https://discord.gg/AaNK56A
<br>
email : alanwalter45@gmail.com