<div align="center">
    <h1 style="text-align: center;">ELITEGG</h1>
</div>

![Mi logo](assets/logo.png)

<div align="center">

# 📖 Índice del Proyecto EliteGG

</div>

> Navega rápidamente por las diferentes secciones del documento.

- 🧭 **[Introducción](#introducción)**
- 🗄️ **[Informe Backend de DB](#informe-de-backend-de-db)**
- 🏗️ **[Arquitectura del Software](#arquitectura-del-software)**
- ⚙️ **[Tecnologías a Utilizar](#tecnologías-a-utilizar)**
- 🌐 **[Red](#red)**
- 💻 **[Web](#web)**
- 🖥️ **[Servicios](#servicios)**
- 🛡️ **[Plan de Contingencia](#plan-de-contingencia)**
- 📊 **[Conclusiones](#conclusiones)**
- 📚 **[Bibliografía](#bibliografia)**

<div align="center">
    <h2 id="introducción" style="text-align: center;">🧭INTRODUCCIÓN</h2>
</div>

<div>
    EliteGG es una plataforma de análisis y seguimiento de estadísticas para distintos videojuegos, principalmente League of Legends, diseñada para jugadores que quieren mejorar y llevar un control más organizado de su progreso.
El objetivo es crear una página similar a OP.GG, pero con una interfaz más clara, ordenada y con nuevas herramientas exclusivas para la comunidad. Los fundadores de este proyecto son:
    <br><br>
    <details>
    <summary><strong>¿POR QUÉ ESTA IDEA?</strong></summary>
    <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">

Como usuarios habituales de este tipo de páginas, creemos que sería interesante crear una que sea nuestra. Además, el tema nos apasiona, ya que trata de un videojuego que se disfruta en el tiempo libre.<br>
Otra razón importante es poder desarrollar una página que resuelva los fallos de las webs existentes en este ámbito. Al ser usuarios recurrentes de estos servicios, se ha identificado varias áreas de mejora y funcionalidades que serán muy útiles e interesantes para la comunidad.
</details>
<details>
<summary><strong>¿HASTA DÓNDE QUIERO LLEGAR CON ESTE PROYECTO?</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
El objetivo principal es crear una página que sea realmente útil y consistente tanto a nivel técnico como a nivel visual, para ello se ha analizado distintas páginas ya existentes y listado las funcionalidades que la página acabará conteniendo. Dichas funciones son:<br>
<li><strong>Estadísticas personales detalladas:</strong> consultar historial de partidas, campeones más jugados y rendimiento por rol...<br></li>
<li><strong>Comparación con otros jugadores:</strong> medir tu nivel frente a amigos o rivales y descubrir en qué aspectos puedes mejorar.<br></li>
<li><strong>Calendario de eventos:</strong> Accede a un calendario con torneos, eventos y novedades del juego para no perderte nada. También puedes guardar algún equipo en concreto como favorito para recibir un correo cada vez que este tenga un partido.<br></li>
<li><strong>Consejos personalizados:</strong> Sugerencias de mejora basadas en tu estilo de juego y datos de la comunidad, como por ejemplo sugerencias de objetos según el campeón que quieras jugar y en contra de cuáles juegues. También te hará una plantilla donde podrás elegir qué campeones te gusta jugar para darte consejos de qué campeón de aquellos que te gustan deberías elegir en contra de enemigos concretos.<br></li>
<li><strong>La página también va a incluir videos de una corta duración haciendo una demostración de las habilidades de los personajes y de sus diferentes aspectos.</strong><br></li>
</details>
<details>
 <summary><strong>¿A QUIÉN VA DIRIGIDO ESTE PROYECTO?</strong></summary>
 <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
El proyecto está dirigido a la comunidad de League of Legends, un factor que nos beneficia mucho en términos de visibilidad. Al ser un juego para todos los públicos, el único "requisito" para usar nuestra plataforma es jugar al juego. Aunque más adelante, si es posible, se incluirán más videojuegos, ya que así el alcance podrá ser mayor y así abarcar otras comunidades.
</details>
<details>
 <summary><strong>MÓDULOS DEL CICLO QUE TENGAN QUE VER CON EL PROYECTO</strong></summary>
  <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 En el proyecto se incluirán varios módulos del curso:<br>
<li>Aplicaciones web: Este módulo es fundamental, ya que necesitamos desarrollar una página web funcional y atractiva. Para ello, utilizaremos lenguajes de programación como HTML y CSS.<br></li>
<li>Seguridad: La seguridad es un aspecto crucial. Implementaremos medidas para proteger nuestros servidores y la información de los usuarios (como sus nombres y contraseñas) contra posibles ataques o robos de datos.<br></li>
<li>Sistemas operativos en red: Este módulo se aplicará directamente en el uso de máquinas virtuales (MV) para nuestros servidores, lo cual es esencial para el despliegue del proyecto.<br></li>
<li>Servicios en red: Este módulo será imprescindible, ya que utilizaremos herramientas esenciales como DNS para el funcionamiento de nuestra plataforma.<br></li>
</details>
<details>
<summary><strong>MATERIALES NECESARIOS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<strong>FÍSICOS<br></strong>
<li>Ordenadores<br></li>                                                         
<strong>LÓGICOS<br></strong>
<li>Virtual Box (VM) <br></li>
<li>Canva<br></li>
<li>Chatgpt<br></li>
<li>Deepseek<br></li>
<li>IA (Gemini)<br></li>
<li>Visual Studio Code<br></li>
<li>Vercel<br></li>
<li>Trello<br></li>
<li>Github<br></li>
<li>Corrector<br></li>
<li>Servicio DHCP en un servidor Windows diferente<br></li>
<li>Servidor DNS primario<br></li>
<li>Firewall: pfSense o Sophos<br></li>
<li>Backup: Truenas y/o rsync<br></li>
<li>Plan de contingencia<br></li>
</details>
    <div align="center">
    <h2 id="informe-de-backend-de-db" style="text-align: center;">🗄️INFORME DE BACKEND DE DB</h2>
</div>
<details>
<summary><strong>IDENTIFICACIONES DE ENTIDADES PRINCIPALES</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<div>
<strong>¿Qué elementos importantes hay en tu web que necesitan almacenarse?<br></strong>
Usuarios y contraseñas, plan de eventos de los partidos oficiales, imágenes personajes, imágenes objetos, videos de las skins y habilidades (muchos videos), imágenes de cada juego para la primera página, y las recomendaciones que te da según tu personaje.
<br><br>
<strong>¿Qué tema de información almacena?<br></strong>
Usuarios (con contraseñas), fechas, imágenes, videos.
</div>
<br><br>
<strong>¿Por qué necesitas guardarla en la base de datos?</strong><br>
 Aquí tenemos una tabla donde se explica de manera resumida la razón por la cual hay que guardar cada tipo de dato.
    <br><br>
<div align="center">
  <img src="assets/tabla1.png" alt="tabla1">
</div>

<div>
<strong>*Los metadatos son los datos extendidos sobre un primer dato, en esta tabla improvisada hemos puesto de ejemplo un campeón (Jinx) que en este caso sería el dato.
Todo lo que muestra la tabla serían los metadatos de este campeón.<br></strong>
 Aquí tenemos un ejemplo de lo que serían los metadatos en un personaje aleatorio de nuestra página, en este caso jinx.
    <br><br>
</div>
<div align="center">
  <img src="assets/Tablajinx.png" alt="Tablajinx">
</div>
</details>

<details>
<summary><strong>DATOS QUE SE DEBEN GUARDAR DE CADA ENTIDAD (ATRIBUTOS)</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
Para cada entidad identificada en el punto anterior, describe qué información concreta se necesita guardar.
Por ejemplo, si una entidad es “Usuario”:<br>
<li>Nombre</li>
<li>Apellidos</li>
<li>Correo electrónico</li>
<li>Contraseña</li>
<li>Fecha de registro</li>
    <br><br>
<strong>Indica el tipo de dato esperado (texto, número, fecha, etc.) y la definición que consideras que corresponde (varchar, int, decimal...)</strong><br>
<div align="center">
  <img src="assets/Tabla3.png" alt="Tabla3">
</div>
    <strong>*Booleano:</strong> Los datos booleanos son datos que se usan para conceptos positivos y negativos<br>
Si/No<br>
Verdadero/Falso<br>
Afirmativo/negativo<br>
<div align="center">
  <img src="assets/EV.png" alt="EV">
</div>

<div align="center">
  <img src="assets/Tablacampeon.png" alt="Tablacampeon">
</div>

<div align="center">
  <img src="assets/Objetos.png" alt="Objetos">
</div>
</details>
<details>
<summary><strong>RELACIONES ENTRE TABLAS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
    <div>

        
<strong><li>USUARIOS y CAMPEÓN/PERSONAJE (Estadísticas y Progreso)</li></strong>
Esta es la relación central para el análisis de estadísticas personales.<br>

<strong><li>USUARIOS y EVENTO/PARTIDO OFICIAL (Notificaciones y Favoritos)</li></strong>
Esta relación permite al sistema enviar las notificaciones por correo de los partidos favoritos.<br>

<strong><li>CAMPEÓN/PERSONAJE y OBJETOS (Consejos Personalizados)</li></strong>
Esta relación es fundamental para la funcionalidad de sugerencia de objetos e ítems contra campeones enemigos.<br>

<strong><li>CAMPEÓN/PERSONAJE u OBJETOS y ELEMENTOS MULTIMEDIA (Recursos)</li></strong>
Esta relación vincula los archivos de medios (imágenes, vídeos de skins, videos de habilidades) con la entidad a la que pertenecen.<br>
</div>
</details>

<details>
<summary><strong>EJEMPLOS DE DATOS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
<div>
    Incluye un ejemplo de cada entidad con datos ficticios pero realistas.<br>
    <br><br>
  <div align="center">
  <img src="assets/USejemplo.png" alt="USejemplo">
  </div>  

<div align="center">
  <img src="assets/EVejemplo.png" alt="EVejemplo">
  </div>  

<div align="center">
  <img src="assets/OBejemplo.png" alt="OBejemplo">
  </div>

 </details>
  <details>
<summary><strong>LISTA DE DATOS DB</strong></summary>
  <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
  <details>
   <summary><strong>USUARIOS</strong></summary>
   <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
   <li>Riot ID</li>
   <li>Contraseña</li>
   <li>Correo</li>
   <li>Teléfono</li>
   <li>Fecha de registro</li>
  </details>
  <details>
<summary><strong>CAMPEONES</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
   <li>ID Campeón</li>
   <li>Nombre del campeón</li>
   <li>Apodo</li>
   <li>Rol principal</li>
   <li>Clase</li>
   <li>Lore del campeón</li>
   <li>Estadísticas del campeón nvl 1</li>
   <li>Imagen del campeón</li>
   <li>Habilidades</li>
   <li>Combos</li>
   <li>Skins</li>
   <li>Precio</li>
  </details>
   <details>
    <summary><strong>BUILDS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
    <li>ID Build</li>
    <li>Runas</li>
    <li>Items</li>
   </details>
  <details>
    <summary><strong>ITEMS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
   <li>ID de Item</li>
   <li>Nombre de items</li>
   <li>Precio de Items</li>
   <li>Venta de Item</li>
   <li>Estadísticas de item</li>
   <li>Imagen de Item</li>
   <li>Activación</li>
   <li>Pasiva</li>
   <li>Lore de Item</li>
   <li>Rama de Creación</li> 
  </details>
   <details>
       <summary><strong>RUNAS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
    <li>ID Runa</li>
    <li>Runa Padre</li>
    <li>Runa Secundaria</li>
    <li>Estadísticas adicionales</li>
   </details>
   <details>
       <summary><strong>E-SPORTS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">    
    <li>Equipos</li>
    <li>Ligas</li>
    <li>Jugadores</li>
   </details>
     <details>
       <summary><strong>EQUIPOS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">   
    <li>ID Equipo</li>
    <li>Nombre del Equipo</li>
    <li>Foto del Equipo</li>
    <li>Jugadores del equipo</li>
    <li>Logros del equipo</li>
    <li>Historia del equipo</li>
    <li>Redes sociales del equipo</li>
    <li>Calendario de equipo</li>
     </details>
        <details>
       <summary><strong>JUGADORES</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">   
    <li>ID Jugador</li>
    <li>Nombre del equipo</li>
    <li>Foto del jugador</li>
    <li>Rol del jugador</li>
    <li>Trayectoria del jugador</li>
    <li>Premios del jugador</li>
    <li>Redes sociales del jugador</li>
    <li>Campeón preferido (provisional)</li>
        </details>
         <details>
       <summary><strong>LIGAS</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;"> 
    <li>ID liga</li>
    <li>Nombre de la liga</li>
    <li>Foto de la liga</li>
    <li>Equipos</li>
    <li>Región</li>
         </details>
        </details> 
   </details>

<details>
<summary><strong>RELACIONES DB</strong></summary>
 <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;"> 
 Aqui se podra observar las relaciones que habrá entre las distintas tablas de la base de datos, junto a las claves foráneas y Claves Primarias de cada una de ellas. Esta está creada utilizando la plataforma MYSQL Workbench.
    <div align="center">
          <img src="assets/DiagramaDB.png" alt="DiagramaDB">
    </div>
</details>
</div>
</details>

<div align="center">
    <h2 id="arquitectura-del-software" style="text-align: center;">🏗️ARQUITECTURA DEL SOFTWARE</h2>
</div>
<details>
 <summary><strong>OBJETIVOS</strong></summary>
  <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 Estos són en formato lista los objetivos que tenemos con nuestra página:<br>
 <li>Desarrollar un sistema de registro/login seguro (intentaremos vincular el RIOT ID de los usuarios para poder verificar con más certeza quien accede a la página).</li>
   <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Mostrar el historial de partidas, los campeones más jugados y el rendimiento por rol del usuario autenticado en una interfaz clara.</li>
    <div align="center">
          <img src="assets/PerfilJ.png" alt="PerfilJ">
    </div>
   <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Implementar la funcionalidad de Combos rápidos y explicación de las habilidades del mismo basada en el campeón que le gusta al usuario.</li>
   <div align="center">
  <img src="assets/Habilidades.png" alt="Habilidades">
             </div>
  <div align="center">
  <img src="assets/Combos.png" alt="Combos">
             </div>
   <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Integrar un calendario de eventos oficiales de LoL con la capacidad de que los usuarios marquen equipos favoritos para recibir notificaciones por correo.</li>
       <div align="center">
  <img src="assets/E-sports.png" alt="E-sports">
</div>
   <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Botón de PvP, sirve para poder seleccionar 2 cuentas diferentes y comparar diferentes aspectos de ambos jugadores mostrados en pantalla.</li>
       <div align="center">
  <img src="assets/PvP.png" alt="PvP">
</div>
    <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Base de datos donde almacenemos los campeones actuales del juego con sus historias resumidas para los curiosos que les guste mirar más allá del juego.</li>
  <div align="center">
  <img src="assets/Galeria.png" alt="Galeria">
</div>
     <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 Ranking de los mejores jugadores que se actualiza de manera automática, pudiendo entrar a los perfiles de esos jugadores TOP.
 <div align="center">
  <img src="assets/Ranking.png" alt="Ranking">
</div>
</details>
<details>
 <summary><strong>RESPONSABLES DE TAREAS</strong></summary>
 <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 Cada miembro del equipo de trabajo se encargará de diferentes aspectos del proyecto, intentando aportar cada uno en el aspecto que más destaca.
 <div align="center">
  <img src="assets/Tareas.png" alt="Tareas">
</div>
</details>
<details>
 <summary><strong>DATOS QUE SE VAN A SOLICITAR</strong></summary>
  <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <strong>-Datos solicitados al usuario</strong>
<li>Riot ID (El cual ya está vinculado a un correo electrónico).</li>
<li>Nombre de usuario</li>
<li>Contraseña</li>
<li>Teléfono móvil</li>
<li>Correo electrónico</li>
<strong>-Tipos de usuarios</strong>
<li>Usuario sin cuenta: Este usuario solo tendrá acceso a la galería de campeones y sus derivados, pero no podrá ni guardar configuraciones ni equipos seleccionados ni recibir notificaciones de manera automática.</li>
<li>Usuario ya registrado: Este usuario ya puede tener tanto equipos favoritos, cuentas y campeones, además de tener la opción de tener notificaciones automáticas.</li>
<li>Administradores: Cuenta que solo tendremos los propietarios de la página para poder modificar pequeñas cosas de la base de datos.</li>
<strong>-Tipos de datos</strong>
 <div align="center">
  <img src="assets/Tablausuarios.png" alt="Tablausuarios">
</div>
 <div align="center">
  <img src="assets/Campeonesh.png" alt="Campeonesh">
</div>
  <div align="center">
  <img src="assets/Campeonesh2.png" alt="Campeonesh2">
</div>
 <div align="center">
  <img src="assets/Skinx.png" alt="Skinx">
</div>
  <div align="center">
  <img src="assets/Itemx.png" alt="Itemx">
</div>
  <div align="center">
  <img src="assets/Runax.png" alt="Runax">
</div>
   <div align="center">
  <img src="assets/Equipox.png" alt="Equipox">
</div>
    <div align="center">
  <img src="assets/Jugadorex.png" alt="Jugadorex">
</div>
 <div align="center">
  <img src="assets/Eventox.png" alt="Eventox">
</div>
 <strong>DEFINICIONES DE LO QUE QUEREMOS USAR:</strong>
 <li><strong>Varchar (X):</strong> Este tipo de dato está hecho para carácter variables, lo que habrá entre  los paréntesis será el número máximo de bits que podremos usar, por ejemplo, si lo que tengo que sacar es un “hola” solo usará 4 bits, sin desperdiciar el resto.</li>
 <li><strong>ENUM:</strong> ENUM se utiliza para un campo donde solo se permite uno de un conjunto predefinido de valores.
Todo valor que no esté dentro de esa lista predefinida, se devolverá.</li>
 <li><strong>Text:</strong> Formato de texto libre. </li>
 <li><strong>Int o Bigint:</strong> Números enteros sin decimales.</li>
 <li><strong>DATETIME:</strong> Para registrar un momento exacto, incluyendo tanto la fecha como la hora.</li>
 <li><strong>JSON (JavaScript Object Notation):</strong> Se usa para almacenar datos complejos y semi-estructurados, como listas anidadas o pares clave-valor.</li>
</details>
<div align="center">
    <h2 id="tecnologías-a-utilizar" style="text-align: center;">⚙️TECNOLOGÍAS A UTILIZAR</h2>
</div>
El proyecto usará diferentes programas para poder ser funcional, las detallaremos en formato lista:
<br><br>
<details>
 <summary><strong>PROGRAMAS</strong></summary>
 <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <details>
 <summary><strong>DNS</strong></summary>
 Traduce el nombre de dominio a la dirección IP del servidor donde se aloja la web, permitiendo a los usuarios encontrar la plataforma.
</details>
<details>
 <summary><strong>DHCP</strong></summary>
No es esencial para la web pública, pero se usaría internamente en la red de desarrollo o producción para asignar IPs automáticas a los servidores y máquinas virtuales.
</details>
<details>
 <summary><strong>MYSQL</strong></summary>
Es un sistema de gestión de bases de datos relacionales, para almacenar datos estructurados de Campeones, Objetos y Usuarios. Ademas instalaremos phpmyadmin para tener una interfaz grafica.
</details>
<details>
 <summary><strong>PIHOLE</strong></summary>
Se usaría en la red de desarrollo para bloquear publicidad y rastreadores a nivel de red para un entorno de trabajo más limpio.
</details>
<details>
 <summary><strong>Github</strong></summary>
Plataforma de control de versiones obligatoria donde se almacenará el código fuente del proyecto, gestionando ramas y la colaboración del equipo. Ademas el codigo de nuestra web se encontrara dentro de un repositorio de github el cual estara ligado a nuestro nginx.
</details>
<details>
 <summary><strong>Firewall</strong></summary>
Software de seguridad de red que protege el servidor, filtrando el tráfico malicioso y asegurando que solo los puertos necesarios (80, 443, 8080) estén accesibles.
</details>
<details>
 <summary><strong>NGINX</strong></summary>
Gestiona y distribuye eficientemente las peticiones HTTP y sirve el contenido estático.
</details>
 <details>
  <summary><strong>ExpressJS</strong></summary>
  Procesa y ejecuta el código dinámico de las aplicaciones para enviárselo a Nginx. Usamos este programa en lugar del PHP debido a que el codigo de la web esta compuesto por un formato tipo TSX.
</details>
</details>
<details>
 <summary><strong>SO QUE VAMOS A UTILIZAR</strong></summary>
<hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
 <li>Plataforma de Virtualización = Proxmox</li>
 <li>Servidor de Backup = Debian</li>
 <li>Servidores DNS = Debian</li>
 <li>Servidor de Aplicación/Web/DB = Debian</li>
 <li>Dhcp + Router = Debian (interfaz gráfica) + IP tables</li>
 <li>Máquinas de Desarrollo = Windows 11</li>
 
</details>
<div align="center">
    <h2 id="red" style="text-align: center;">🌐RED</h2>
</div>
<details>
    <summary><strong>DIAGRAMA DE LA RED</strong></summary>

 <p>La red se divide en <strong>dos zonas</strong> separadas por un <strong>Router/Firewall</strong> que actúa como puerta de control.</p>
 
<img width="1142" height="642" alt="image" src="https://github.com/user-attachments/assets/201cd82b-7cdd-43ea-86e9-bcd0e55b1ef0" />
<br>

<div align="center">
    <table style="width: 100%; border-collapse: collapse; background: #f5f5f5;">
        <tr style="background-color: #333; color: white;">
            <th style="padding: 12px; border: 1px solid #444;">Zona</th>
            <th style="padding: 12px; border: 1px solid #444;">Elemento</th>
            <th style="padding: 12px; border: 1px solid #444;">Función</th>
        </tr>
         <tr>
            <td rowspan="3" style="padding: 12px; border: 1px solid #444; vertical-align: middle; text-align: center;"><strong>ZONA EXTERNA<br>(Desarrollo)</strong></td>
            <td style="padding: 12px; border: 1px solid #444;"><strong>Máquina de virtualización</strong><br><code>192.168.135.69</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Servidor con Proxmox que aloja todas las máquinas virtuales del proyecto.</td>
         </tr>
         <tr>
            <td style="padding: 12px; border: 1px solid #444;"><strong>Máquinas de desarrollo</strong><br><code>192.168.135.X</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Ordenadores de los programadores para trabajar en la web.</td>
         </tr>
         <tr>
            <td style="padding: 12px; border: 1px solid #444;"><strong>Servidor de Backups</strong></td>
            <td style="padding: 12px; border: 1px solid #444;">Almacena copias de seguridad automáticas de toda la infraestructura.</td>
         </tr>
        <tr style="background-color: #e9ecef;">
            <td rowspan="4" style="padding: 12px; border: 1px solid #444; vertical-align: middle; text-align: center;"><strong>ZONA INTERNA<br>(Producción - <code>10.10.10.X</code>)</strong></td>
            <td style="padding: 12px; border: 1px solid #444;"><strong>Router</strong><br><code>10.10.10.1</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Puerta de entrada. Con IPTables gestiona el tráfico, protege la red interna y redirige las peticiones al servidor web.</td>
         </tr>
        <tr style="background-color: #e9ecef;">
            <td style="padding: 12px; border: 1px solid #444;"><strong>DNS (Pi-hole)</strong><br><code>10.10.10.5</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Traduce nombres a direcciones IP y bloquea anuncios/malware.</td>
         </tr>
        <tr style="background-color: #e9ecef;">
            <td style="padding: 12px; border: 1px solid #444;"><strong>Web (Nginx)</strong><br><code>10.10.10.6</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Servidor que muestra la página web a los usuarios.</td>
         </tr>
        <tr style="background-color: #e9ecef;">
            <td style="padding: 12px; border: 1px solid #444;"><strong>Database (MySQL)</strong><br><code>10.10.10.9</code></td>
            <td style="padding: 12px; border: 1px solid #444;">Almacena todos los datos de usuarios, campeones y estadísticas.</td>
         </tr>
         <tr>
            <td style="padding: 12px; border: 1px solid #444;"><strong>APIs externas</strong></td>
            <td colspan="2" style="padding: 12px; border: 1px solid #444;">Fuentes externas de datos, como la API de Riot Games.</td>
         </tr>
     </table>
</div>

<br>

<div align="center">
    <h4>📌 FLUJO BÁSICO</h4>
</div>

<p align="center">Usuario accede a la web → Router redirige a Servidor Web → Web consulta a Base de Datos → Web devuelve la información al usuario.<br>
<strong>Todo protegido por el Router y el DNS.</strong></p>
  <div align="center">
  

</div>

</details>
<div align="center">
    <h2 id="web" style="text-align: center;">💻WEB</h2>
</div>
Aqui tendremos la planificación a nivel tanto visual como interactivo de lo que será nuestra web.
<details>
    <summary><strong>MOCKUP</strong></summary>
    <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
Aquí se podrá observar las bases a nivel visual de lo que será la página web de EliteGG. Para empezar la paleta principal de colores que compone la página son el negro, blanco, morado y amarillo, esto para dar una sensación de estilo neon ya que la página está dirigida al gaming. Seguido esto tenemos cada apartado de la página.
    <br><br>
    <details>
    <summary><strong>Home page</strong></summary>
     <hr style="margin-top: 10px; margin-bottom: 0px; border: none; height: 1px; visibility: hidden;">
      En nuestra Home page se encuentra primeramente una barra superior que contiene distintos objetos, comenzando por nuestro logo en un formato más pequeño y en la parte izquierda de la barra, segu
