<div align="center">
    <h1 style="text-align: center;">EliteGG</h1>
</div>

![Mi logo](assets/logo.png)

<div align="center">
    <h2 style="text-align: center;">ÍNDICE</h2>
</div>

<div align="center">
    <h2 style="text-align: center;">INTRODUCCIÓN</h2>
</div>

<div>
    EliteGG es una plataforma de análisis y seguimiento de estadísticas para distintos videojuegos, principalmente League of Legends, diseñada para jugadores que quieren mejorar y llevar un control más organizado de su progreso.
Nuestro objetivo es crear una página similar a OP.GG, pero con una interfaz más clara, ordenada y con nuevas herramientas exclusivas para la comunidad. 
    <br><br>
    <details>
    <summary><strong>¿Porque esta idea?</strong></summary>
    <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">

Como usuarios habituales de este tipo de páginas, creemos que sería interesante crear una que sea nuestra. Además, el tema nos apasiona, ya que trata de un videojuego que se disfruta en el tiempo libre.<br>
Otra razón importante es poder desarrollar una página que resuelva los fallos de las webs existentes en este ámbito. Al ser usuarios recurrentes de estos servicios, se ha identificado varias áreas de mejora y funcionalidades que serán muy útiles e interesantes para la comunidad.
</details>
<details>
<summary><strong>¿Hasta donde quiero llegar con este proyecto?</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
El objetivo principal es crear una página que sea realmente util y consistente tanto a nivel tecnico como a nivel visual, para ello se ha analizado distintas páginas ya existentes y listado las funcionalidades que la pagina acabará conteniendo. Dichas funciones son:<br>
 1. Estadísticas personales detalladas: consultar historial de partidas, campeones más jugados y rendimiento por rol....<br>
 2. Comparación con otros jugadores: medir tu nivel frente a amigos o rivales y descubrir en qué aspectos puedes mejorar.<br>
 3. Calendario de eventos: Accede a un calendario con torneos, eventos y novedades del juego para no perderte nada. También puedes guardar algún equipo en concreto como favorito para recibir un correo cada vez que este tenga un partido.<br>
 4. Consejos personalizados: Sugerencias de mejora basadas en tu estilo de juego y datos de la comunidad, como por ejemplo sugerencias de objetos según el campeón que quieras jugar y en contra de cuales juegues. También te hara una plantilla donde podras elegir que campeones te gusta jugar para darte consejos de que campeón de aquellos que te gustan deberías elegir en contra de enemigos concretos.<br>
 5. La pagina también va a incluir videos de una corta duración haciendo una demostración de las habilidades de los personajes y de sus diferentes aspectos.<br>
</details>
<details>
 <summary><strong>¿A quién va dirigido este proyecto?</strong></summary>
 <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 El proyecto está dirigido a la comunidad de League of Legends, un factor que nos beneficia mucho en términos de visibilidad. Al ser un juego para todos los públicos, el único "requisito" para usar nuestra plataforma es jugar al juego. Aunque mas adelante, si es posible, se incluiran más videojuegos ya que así el alcance podrá ser mayor y así abarcar otras comunidades.
</details>
<details>
 <summary><strong>Módulos del ciclo que tengan que ver con el proyecto</strong></summary>
  <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 En el proyecto se incluirán varios módulos del curso:<br>
1. Aplicaciones web: Este módulo es fundamental, ya que necesitamos desarrollar una página web funcional y atractiva. Para ello, utilizaremos lenguajes de programación como HTML y CSS.<br>
2. Seguridad: La seguridad es un aspecto crucial. Implementaremos medidas para proteger nuestros servidores y la información de los usuarios (como sus nombres y contraseñas) contra posibles ataques o robos de datos.<br>
3. Sistemas operativos en red: Este módulo se aplicará directamente en el uso de máquinas virtuales (MV) para nuestros servidores, lo cual es esencial para el despliegue del proyecto.<br>
4. Servicios en red: Este módulo será imprescindible, ya que utilizaremos herramientas esenciales como DNS para el funcionamiento de nuestra plataforma.<br>
</details>
<details>
<summary><strong>Materiales necesarios:</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<strong>Fisicos:<br></strong>
1. Ordenadores<br>
<strong>Lógicos:<br></strong>
1. Virtual Box (VM) <br>
2. Canva<br>
3. IA (Gemini)<br>
4. Visual Studio Code<br>
5. Vercel<br>
6. Trello<br>
7. Github<br>
</details>
<details>
<summary><strong>Recursos (Bibliografía, webgrafía, vídeos, cursos o demás multimedia)</strong></summary>
    <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
    https://www.youtube.com/watch?v=jkzq9j5yeT8&list=PL3vL1pnMCbUERqllcwhcvEJbKum-M9zT5
https://gist.github.com/dasdo/9ff71c5c0efa037441b6
https://www.youtube.com/watch?v=niPExbK8lSw&t=518s
 </div>

</details>
    <div align="center">
    <h2 style="text-align: center;">BRIEFING DE IDEAS</h2>
</div>

<div align="center">
    <h2 style="text-align: center;">ARQUITECTURA DEL SOFTWARE</h2>
</div>
<div align="center">
    <h2 style="text-align: center;">TECNOLOGÍAS A UTILIZAR</h2>
</div>
<div align="center">
    <h2 style="text-align: center;">RED</h2>
</div>
<div align="center">
    <h2 style="text-align: center;">PLANIFICACIÓN DE BASE DATOS</h2>
</div>

<details>
<summary><strong>Identificaciones de entidades principales</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<div>
<strong>-¿Qué elementos importantes hay en tu web que necesitan almacenarse?<br></strong>
Usuarios y contraseñas, plan de eventos de los partidos oficiales, imagenes personajes, imágenes objetos, videos de las skins y habilidades (muchos videos), imagenes de cada juego para la primera página, y las recomendaciones que te da segun tu personaje

<strong>-¿Qué tema de información almacena?<br></strong>
Usuarios (con contraseñas), fechas, imagenes, videos.
</div>
<strong>-¿Por qué necesitas guardarla en la base de datos?</strong>
<div align="center">
  <img src="assets/tabla1.png" alt="tabla1">
</div>

<div>
*Los metadatos son los datos extendidos sobre un primer dato, en esta tabla improvisada hemos puesto de ejemplo un campeón (Jinx) que en este caso sería el dato.
Todo lo que muestra la tabla serían los metadatos de este campeón.
</div>
<div align="center">
  <img src="assets/Tablajinx.png" alt="Tablajinx">
</div>
</details>

<details>
<summary><strong>Datos que se deben guardar de cada entidad (atributos)</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
Para cada entidad identificada en el punto anterior, describe qué información concreta se necesita guardar.
Por ejemplo, si una entidad es “Usuario”:<br>
1.Nombre<br>
2.Apellidos<br>
3.Correo electrónico<br>
4.Contraseña<br>
5.Fecha de registro<br>
<strong>-Indica el tipo de dato esperado (texto, número, fecha, etc.) y la definición que consideras que corresponde (varchar, int, decimal...)</strong><br>
<div align="center">
  <img src="assets/Tabla3.png" alt="Tabla3">
</div>
    <strong>*Booleano:</strong> Los datos booleanos son datos que se usan para conceptos positivos y negativos:<br>
Si/No<br>
Verdadero/Falso<br>
Afirmativo/negativo<br>
<div align="center">
  <img src="assets/Evento.png" alt="Evento">
</div>

<div align="center">
  <img src="assets/Tablacampeon.png" alt="Tablacampeon">
</div>

<div align="center">
  <img src="assets/Objetos.png" alt="Objetos">
</div>
</details>
<details>
<summary><strong>Relaciones entre tablas</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
    <div>

        
<strong>1.USUARIOS y CAMPEÓN/PERSONAJE (Estadísticas y Progreso)</strong><br>
Esta es la relación central para el análisis de estadísticas personales.<br>

<strong>2.USUARIOS y EVENTO/PARTIDO OFICIAL (Notificaciones y Favoritos)</strong><br>
Esta relación permite al sistema enviar las notificaciones por correo de los partidos favoritos.<br>

<strong>3.CAMPEÓN/PERSONAJE y OBJETOS (Consejos Personalizados)</strong><br>
Esta relación es fundamental para la funcionalidad de sugerencia de objetos e ítems contra campeones enemigos.<br>

<strong>4.CAMPEÓN/PERSONAJE u OBJETOS y ELEMENTOS MULTIMEDIA (Recursos)</strong><br>
Esta relación vincula los archivos de medios (imágenes, vídeos de skins, videos de habilidades) con la entidad a la que pertenecen.<br>
</div>
</details>

<details>
<summary><strong>Ejemplo de datos</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<div>
    -Incluye un ejemplo de cada entidad con datos ficticios pero realistas.<br>
  <div align="center">
  <img src="assets/USejemplo.png" alt="USejemplo">
  </div>  

<div align="center">
  <img src="assets/EVejemplo.png" alt="EVejemplo">
  </div>  

<div align="center">
  <img src="assets/OBejemplo.png" alt="OBejemplo">
  </div>
  
</div>
</details>
