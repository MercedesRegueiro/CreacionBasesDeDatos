<h1>Proyectos de Investigación</h1>
El enunciado del ejercicio podrás encontrarlo en el siguiente enlace de davidgchaves: <a href="https://github.com/davidgchaves/first-steps-with-git-and-github-wirtz-asir1-and-dam1/tree/master/exercicios-ddl/1-proxectos-de-investigacion">Enunciado Proyecto de Investigacion</a><br/>
<h2>Crear Base de Datos</h2>
Para crear la base de datos debemos escribir lo siguiente: <b>CREATE DATABASE <i>nombreBD</i>;</b>
<img src="../imagenes/1_CrearBD.PNG"/>
Una vez hecho esto deberemos indicar que queremos hacer operaciones con esa base de datos por lo que deberemos usar lo siguiente: <b>USE <i>nombreBD</i>;</b>
<img src="../imagenes/2_UsarBD.PNG"/>


<h2>Crear Tablas</h2>
<b>NOTA:</b> A mi me parece más cómodo primero crear las tablas con las PRIMARY KEY y una vez creadas las tablas poner todas las claves foraneas.<br/<
Lo primero es crear las tablas. Para ello se utiliza lo siguiente: <b>CREATE TABLE <i>nombreTabla</i> (campo1 tipo, campo2 tipo, ...);</b> 
<img src="../imagenes/3_CrearTablaBD.PNG"/>
Dato: Para poner la PRIMARY KEY se escribe lo siguiente dentro del CREATE TABLE (Ver imagen anterior): <b>CONSTRAINT <i>nuevoNombre</i> PRIMARY KEY (<i>nombreCampo</i>)</b><br/>
Una vez creada la tabla podemos comprobar que se ha creado correctamente y ver sus propiedades. Para ello usamos: <b>DESCRIBE <i>nombreTabla</i>;</b>
<img src="../imagenes/4_ComprobarTablaBD.PNG"/>

<h3>Creación y Comprobacion de las Tablas del Ejercicio</h3>
Antes de hacer las claves foráneas, hay que crear las tablas que faltan. <br/>
En el siguiente enlace podreis ver la creacion de las tablas restantes del ejercicio: <a href="https://github.com/MercedesRegueiro/CreacionBasesDeDatos/tree/master/1_ProyectosInvestigacion/TablasEjercicio1">Crear Tablas Restantes</a>


<h2>Poner Claves Foráneas</h2>
Para poner las claves foráneas debemos escribir lo siguiente:<b>ALTER TABLE <i>nombreTabla</i> ADD CONSTRAINT <i>nuevoNombre</i> FOREIGN KEY (<i>nombreCampo</i>) REFERENCES <i>nombreTabla2</i>(<i>nombreCampo2</i>) ON DELETE <i>Tipo</i> ON UPDATE <i>Tipo</i>;</b><br/>
<img src="../imagenes/ForaneasUbicacion.PNG"/>
