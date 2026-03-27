<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arduino - Documentación Oficial del Proyecto</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #e9edf2 100%);
            color: #2c3e50;
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
            overflow: hidden;
            padding: 40px;
        }

        h1 {
            color: #00979D;
            font-size: 2.5em;
            margin-bottom: 20px;
            text-align: center;
            border-bottom: 3px solid #00979D;
            display: inline-block;
            padding-bottom: 10px;
        }

        h2 {
            color: #2c3e50;
            font-size: 1.8em;
            margin: 30px 0 20px 0;
            padding-left: 15px;
            border-left: 5px solid #00979D;
        }

        h3 {
            color: #34495e;
            font-size: 1.4em;
            margin: 20px 0 15px 0;
        }

        .header-center {
            text-align: center;
            margin-bottom: 30px;
        }

        img {
            max-width: 100%;
            height: auto;
            border-radius: 12px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        img:hover {
            transform: scale(1.02);
        }

        details {
            background: #f8f9fa;
            border-radius: 12px;
            margin: 15px 0;
            padding: 15px;
            border-left: 4px solid #00979D;
            transition: all 0.3s ease;
        }

        details:hover {
            background: #f0f2f5;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
        }

        summary {
            font-weight: bold;
            font-size: 1.1em;
            cursor: pointer;
            color: #00979D;
            padding: 5px;
        }

        summary:hover {
            color: #007b83;
        }

        code {
            background: #2c3e50;
            color: #ecf0f1;
            padding: 2px 6px;
            border-radius: 5px;
            font-family: 'Courier New', monospace;
            font-size: 0.9em;
        }

        pre {
            background: #2c3e50;
            color: #ecf0f1;
            padding: 15px;
            border-radius: 8px;
            overflow-x: auto;
            margin: 15px 0;
            font-family: 'Courier New', monospace;
            font-size: 0.9em;
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            margin: 20px 0;
            border-radius: 12px;
            background: #000;
        }

        .video-container video, .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border-radius: 12px;
        }

        .component-list {
            background: #ecf0f1;
            padding: 20px;
            border-radius: 12px;
            margin: 15px 0;
            display: inline-block;
            width: auto;
        }

        .component-list img {
            margin: 10px;
            box-shadow: none;
        }

        hr {
            margin: 20px 0;
            border: none;
            height: 2px;
            background: linear-gradient(to right, #00979D, transparent);
        }

        .badge {
            background: #00979D;
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8em;
            display: inline-block;
            margin-right: 10px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        th, td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }

        th {
            background: #00979D;
            color: white;
            font-weight: bold;
        }

        tr:hover {
            background: #f5f5f5;
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }
            
            h1 {
                font-size: 1.8em;
            }
            
            h2 {
                font-size: 1.4em;
            }
        }

        .footer {
            text-align: center;
            margin-top: 50px;
            padding-top: 20px;
            border-top: 2px solid #ecf0f1;
            color: #7f8c8d;
        }

        .image-gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin: 20px 0;
        }

        .image-gallery img {
            flex: 1;
            min-width: 200px;
            max-width: 300px;
        }
    </style>
</head>
<body>
<div class="container">

    <!-- Header Principal -->
    <div class="header-center">
        <h1>⚡ ARDUINO</h1>
        <p style="font-size: 1.2em; color: #7f8c8d;">Plataforma de código abierto para la creación electrónica</p>
    </div>

    <div align="center">
        <img src="https://github.com/user-attachments/assets/189fe64c-3da7-48c4-b756-e1004be34eb6" alt="Arduino Robot" style="max-width: 200px;">
    </div>

    <!-- Sección: ¿Qué es Arduino? -->
    <h2>🔍 ¿Qué es Arduino?</h2>
    <p>Arduino es una plataforma de creación electrónica de código abierto que se compone de dos partes principales: la física y la digital. Su filosofía se basa en la simplicidad, la accesibilidad y la flexibilidad, lo que la convierte en la herramienta ideal tanto para artistas, diseñadores y aficionados como para profesionales y educadores.</p>

    <details>
        <summary><strong>📱 Parte Física (Hardware)</strong></summary>
        <p>La parte física está compuesta por una placa de circuito impreso (PCB) que actúa como el cerebro del proyecto. Esta placa integra un microcontrolador que puedes programar para interactuar con el mundo exterior, conectando sensores, actuadores, motores y otros componentes electrónicos a sus pines de entrada y salida. Es un lienzo en blanco listo para ser modificado y manejado según tu creatividad.</p>
        <div align="center">
            <img src="assets/ardfisico.png" alt="Placa Arduino física">
        </div>
    </details>

    <details>
        <summary><strong>💻 Parte Digital (Software)</strong></summary>
        <p>La parte digital es el entorno de desarrollo integrado (IDE) de Arduino. Es el lugar donde escribes el código, utilizando un lenguaje basado en C/C++ simplificado. Aquí es donde das vida a tu proyecto, creando una serie de instrucciones lógicas que le indican a la placa qué hacer, cómo reaccionar a los estímulos externos y cómo controlar los componentes conectados.</p>
        <div align="center">
            <img src="assets/IDEar.png" alt="IDE de Arduino">
        </div>
    </details>

    <!-- Origen -->
    <h2>🌍 ¿Cuál es su origen?</h2>
    <p>Arduino nació en 2005 en el Instituto de Diseño Interactivo de Ivrea, Italia. Fue creado por un equipo de estudiantes y profesores, liderado por Massimo Banzi, con el objetivo de ofrecer a los estudiantes una herramienta de proyectos electrónica que fuera sencilla, de bajo coste y rápida de aprender, a diferencia de las complejas y costosas placas de desarrollo de la época.</p>
    <div align="center">
        <img src="assets/notch.png" alt="Origen de Arduino">
    </div>
    <p>Tras el cierre del instituto, el equipo decidió liberar el proyecto bajo licencias de código abierto. Esta decisión impulsó su fama mundial, creando una comunidad global de makers, ingenieros y artistas que continúan contribuyendo a su evolución.</p>

    <!-- Características -->
    <h2>⭐ Características más importantes</h2>
    <p>Arduino se distingue por ser una plataforma de código abierto, lo que significa que tanto su hardware como su software son libres y están disponibles para que cualquiera los estudie, modifique y distribuya. De esta filosofía se derivan sus dos factores más importantes:</p>
    <ul>
        <li><strong>🎨 Creatividad y Flexibilidad:</strong> Su principal fortaleza es la capacidad de adaptarse a una infinidad de proyectos. Es ideal para principiantes gracias a un lenguaje de programación simple y una comunidad que ofrece una vasta cantidad de tutoriales y ejemplos.</li>
        <li><strong>💰 Bajo Coste y Accesibilidad:</strong> Su bajo coste en comparación con otras plataformas de desarrollo lo hace accesible para escuelas, aficionados y proyectos personales, eliminando la barrera económica para la experimentación y el aprendizaje.</li>
    </ul>

    <!-- Modelos -->
    <h2>📦 Modelos de Arduino</h2>
    <p>Existen diversos modelos de placas Arduino, cada una diseñada para satisfacer necesidades específicas. Los más populares incluyen el <strong>Arduino Uno</strong> (ideal para principiantes), el <strong>Arduino Mega</strong> (con más pines y memoria para proyectos complejos), el <strong>Arduino Nano</strong> (compacto y perfecto para proyectos embebidos) y el <strong>Arduino Leonardo</strong> (con capacidad para emular periféricos de computadora). Cada modelo varía en voltaje de operación (generalmente 5V o 3.3V), número de pines digitales y analógicos, capacidad de memoria (Flash, SRAM, EEPROM) y velocidad de reloj.</p>
    <div align="center">
        <img src="assets/ardmodelo.png" alt="Modelos de Arduino">
    </div>

    <!-- Para qué sirve -->
    <h2>🛠️ ¿Para qué sirve?</h2>
    <p>Arduino es una herramienta versátil que sirve para crear una gran cantidad de proyectos electrónicos y de robótica. Es ampliamente utilizado en entornos educativos para enseñar programación, electrónica y pensamiento computacional. Sus aplicaciones prácticas abarcan desde la automatización del hogar hasta la creación de prototipos de productos tecnológicos.</p>
    <ul>
        <li><strong>🏠 Sistemas para casas inteligentes (Domótica):</strong> Controla luces, persianas, electrodomésticos y sistemas de seguridad. Conecta sensores de temperatura, humedad, presencia y actuadores para crear un hogar automatizado y eficiente.</li>
        <div align="center">
            <img src="assets/casaar.png" alt="Domótica con Arduino">
        </div>
        <li><strong>🏢 Automatización en edificios e industria:</strong> Controla sistemas de climatización, iluminación y accesos en edificios. En entornos industriales, sirve para monitorear maquinaria, controlar procesos y crear sistemas de adquisición de datos.</li>
        <div align="center">
            <img src="assets/edar.png" alt="Automatización industrial">
        </div>
    </ul>

    <!-- Lenguaje -->
    <h2>💬 ¿Qué lenguaje utiliza?</h2>
    <p>Arduino se programa utilizando un lenguaje basado en <strong>C/C++</strong>, simplificado y adaptado para facilitar la interacción con los periféricos de la placa. Este lenguaje de programación incluye funciones específicas como <code>pinMode()</code>, <code>digitalWrite()</code> y <code>analogRead()</code>, que abstraen la complejidad de la programación de microcontroladores, haciendo la curva de aprendizaje mucho más accesible para los principiantes sin perder potencia para los usuarios más avanzados.</p>
    <div align="center">
        <img src="assets/cplus.png" alt="Lenguaje C++">
    </div>

    <!-- IDE -->
    <h2>🖥️ ¿Qué es el IDE?</h2>
    <p>El Arduino IDE (Entorno de Desarrollo Integrado) es la aplicación oficial y gratuita que se utiliza para escribir, compilar y cargar el código a la placa Arduino. Proporciona una interfaz sencilla con un editor de texto, un área de mensajes, una consola de texto y una barra de herramientas con botones para las funciones más comunes como verificar y cargar el programa.</p>
    <div align="center">
        <img src="assets/IDEard.png" alt="Arduino IDE">
    </div>

    <hr>

    <!-- PRÁCTICAS -->
    <h2>🔧 PRÁCTICAS CON ARDUINO</h2>

    <!-- Actividad 0 -->
    <h3>💡 ACTIVIDAD 0: BLINK</h3>
    <p><strong>Objetivo:</strong> Utilizar el ESP32-S3 WROOM para controlar el parpadeo de un LED integrado en la placa. Este es el "Hola Mundo" de la electrónica y sirve para verificar que la placa y el entorno de desarrollo funcionan correctamente.</p>
    <div align="center">
        <img src="assets/compblink.png" alt="Componentes Blink">
    </div>
    <details>
        <summary><strong>LED azul que parpadea</strong></summary>
        <p>El código "Blink" hace que un LED (normalmente el integrado en la placa, conectado al pin 2 en el ESP32-S3) se encienda y apague de forma repetida. Esto sirve para confirmar que la placa y el software están funcionando correctamente.</p>
    </details>
    <details>
        <summary><strong>void setup() y void loop()</strong></summary>
        <p><strong>void setup():</strong> Se ejecuta una sola vez al iniciar la placa. Configura el estado inicial de los componentes (pines, comunicación serie).<br>
        <strong>void loop():</strong> Se ejecuta de forma continua e infinita. Contiene las instrucciones que se repiten constantemente.</p>
    </details>
    <details>
        <summary><strong>#define LED_BUILTIN 2</strong></summary>
        <p>Define una constante. Reemplaza cualquier aparición de <code>LED_BUILTIN</code> por el número 2, haciendo el código más legible.</p>
    </details>
    <details>
        <summary><strong>delay(1000)</strong></summary>
        <p>Pausa la ejecución del programa durante el tiempo especificado en milisegundos (1000 ms = 1 segundo).</p>
    </details>

    <!-- Actividad 1 -->
    <h3>🔴 ACTIVIDAD 1: LED EXTERNO</h3>
    <p>Control de un LED externo usando la placa ESP32-S3 WROOM.</p>
    <div align="center">
        <img src="assets/compLED.png" alt="Componentes LED">
        <img src="assets/semaforo1.png" alt="Circuito LED 1">
        <img src="assets/semaforo2.png" alt="Circuito LED 2">
        <img src="assets/codigosemaforo.png" alt="Código LED">
        <img src="assets/LEDfoto1.png" alt="LED encendido">
        <img src="assets/LEDfoto2.png" alt="LED apagado">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/49e49177-718f-447d-90b8-2797805de5da" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 2 -->
    <h3>🚦 ACTIVIDAD 2: SEMÁFORO</h3>
    <p>Simulación de un semáforo con tres LEDs.</p>
    <div align="center">
        <img src="assets/componentesema.png" alt="Componentes semáforo">
        <img src="assets/codigosem.png" alt="Código semáforo">
        <img src="assets/esquemasem.png" alt="Esquema semáforo">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/5c37b494-c140-4cbd-9c3f-217365d051c2" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 3 -->
    <h3>🔘 ACTIVIDAD 3: BOTÓN Y LED</h3>
    <p>Control de un LED mediante un pulsador.</p>
    <div align="center">
        <img src="assets/componentesardact3.png" alt="Componentes botón">
        <img src="assets/codigoact3ard.png" alt="Código botón">
        <img src="assets/esquemaact3ard.png" alt="Esquema botón">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/34f02e2f-5f67-45fd-9deb-352e842ec188" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 4 -->
    <h3>💡 ACTIVIDAD 4: MINI LÁMPARA DE MESA</h3>
    <p>Interruptor tipo lámpara: una pulsación enciende, otra apaga.</p>
    <div align="center">
        <img src="assets/ARDACT4.png" alt="Mini lámpara">
        <img src="assets/esquemaact3ard.png" alt="Esquema lámpara">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/0b8667d9-59fc-4b6e-8603-20c494ff2526" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 5 RGB -->
    <h3>🌈 ACTIVIDAD 5: LED RGB</h3>
    <p>Control de colores con un LED RGB, uso de random() y gradientes.</p>
    <div align="center">
        <img src="assets/componentesact5.png" alt="Componentes RGB">
        <img src="assets/diferenciasledrgb.png" alt="Diferencias LED vs RGB">
        <img src="assets/ARDACT5.png" alt="Circuito RGB">
        <img src="assets/circuitodiseñoact5.png" alt="Esquema RGB">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/d7e50a8a-eafa-423a-b32d-957b739f9aee" type="video/mp4">
        </video>
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/27c91968-7255-46bf-b115-0f35ceff82e2" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 6 LED BAR -->
    <h3>📊 ACTIVIDAD 6: BARRA DE LEDS</h3>
    <p>Control de una barra de 10 LEDs con secuencias y botón.</p>
    <div align="center">
        <img src="https://github.com/user-attachments/assets/dff35936-e52d-4d51-bc86-b110242286b6" alt="Componentes barra">
        <img src="https://github.com/user-attachments/assets/aaeac552-5316-45df-bdd4-0ff0316671c9" alt="Código barra inicio medio">
        <img src="https://github.com/user-attachments/assets/d5c11915-8f38-4d21-8179-b976f52ece59" alt="Código barra con botón">
        <img src="https://github.com/user-attachments/assets/d88eb7b3-a452-4d7f-8632-8a720805d8e8" alt="Código final barra">
    </div>
    <div class="video-container">
        <video controls>
            <source src="https://github.com/user-attachments/assets/9b86fa40-f2c8-4c18-9ef7-e1f5b1ab03fb" type="video/mp4">
        </video>
    </div>

    <!-- Actividad 7 Comunicación Serie -->
    <h3>📡 ACTIVIDAD 7: COMUNICACIÓN SERIE</h3>
    <p>Uso del monitor serie y pantalla LCD I2C con sensor DHT11.</p>
    <div align="center">
        <img src="https://github.com/user-attachments/assets/fd8e00cd-7c35-4cf0-98f1-6df1c6f81409" alt="Comunicación serie">
        <img src="https://github.com/user-attachments/assets/0a86607f-5be4-41df-b94d-432a28a66b99" alt="Monitor serie">
        <img src="https://github.com/user-attachments/assets/6d69e45c-5e0f-4b43-a850-2677c1a62883" alt="Código serie">
        <img src="https://github.com/user-attachments/assets/326b4274-3682-4340-957f-ccca54e1ae68" alt="Salida serie">
        <img src="https://github.com/user-attachments/assets/9e261a64-466b-4d1d-a769-052f8d04ec9f" alt="LCD I2C">
        <img src="https://github.com/user-attachments/assets/dfa86304-f55f-4ef7-8fc6-480feb34eacd" alt="Código LCD desplazamiento">
        <img src="https://github.com/user-attachments/assets/51e32b1a-8f84-4ed3-9abf-789cdf6aee27" alt="LCD en acción">
        <img src="https://github.com/user-attachments/assets/22d986ab-f5ab-4ee3-ab0f-cfa45b894e61" alt="Sensor DHT11">
        <img src="https://github.com/user-attachments/assets/8c83d05d-8b0c-4a97-9eef-af15af589cd9" alt="Código DHT Kelvin Fahrenheit">
    </div>

    <!-- Actividad WiFi -->
    <h3>📶 ACTIVIDAD 8: WIFI</h3>
    <p>Modos Station, Access Point y servidor web en el ESP32.</p>
    <div align="center">
        <img src="https://github.com/user-attachments/assets/58f48420-a8b5-4f97-92b1-5d8a140f90df" alt="Modo Station">
        <img src="https://github.com/user-attachments/assets/70fcf3f4-29c4-42e6-857f-315bf2a1908e" alt="Código AP">
        <img src="https://github.com/user-attachments/assets/d37aa673-0eae-4675-ba4d-4f444b42da7f" alt="Modo AP+Station">
        <img src="https://github.com/user-attachments/assets/d12ee6e1-c8cd-4985-8da1-7f8e3103e3b1" alt="Servidor web ESP32">
    </div>

    <hr>

    <!-- PROYECTO FINAL: ACERO IMPURO -->
    <div class="header-center">
        <h1 style="border-bottom-color: #e67e22;">⚔️ ACERO IMPURO</h1>
    </div>
    <div align="center">
        <img src="assets/logoacero.png" alt="Logo Acero Impuro" style="max-width: 200px;">
    </div>

    <h2>🏆 INTRODUCCIÓN</h2>
    <p><strong>Elite Arduino Battle</strong> es un proyecto de robótica competitiva desarrollado por el equipo "La Elite". Consiste en el diseño, programación y ensamblaje de dos vehículos autónomos o controlados por Arduino, equipados con sistemas de ataque y defensa para combate en arena. El objetivo fundamental es la supervivencia: cada coche protege un punto débil (globo) mientras intenta perforar el del adversario mediante un arma frontal personalizada.</p>

    <details>
        <summary><strong>❓ ¿POR QUÉ ESTA IDEA?</strong></summary>
        <p>Como entusiastas de la tecnología, buscábamos un proyecto que combinara la programación lógica con la ingeniería física. La idea de los "Coches de Combate" nos permite experimentar con la movilidad, el diseño de estructuras en 3D y la estrategia en tiempo real. Además, traslada la competitividad de los videojuegos al mundo real, permitiéndonos ver físicamente el resultado de nuestro código y diseño mecánico.</p>
    </details>

    <details>
        <summary><strong>🎯 ¿HASTA DÓNDE QUEREMOS LLEGAR?</strong></summary>
        <ul>
            <li><strong>Control Total:</strong> Dominar el manejo de motores y sensores mediante código limpio y eficiente.</li>
            <li><strong>Diseño e Impresión 3D:</strong> Crear piezas personalizadas para el soporte de armas y blindaje, optimizando el peso y la resistencia.</li>
            <li><strong>Autonomía y Respuesta:</strong> Conseguir que el sistema de ataque sea funcional y que el chasis soporte el impacto sin desmontarse.</li>
            <li><strong>Aprendizaje Técnico:</strong> Documentar todo el proceso para que sirva de base a futuros proyectos de robótica más complejos.</li>
        </ul>
    </details>

    <details>
        <summary><strong>📚 OBJETIVOS DE APRENDIZAJE</strong></summary>
        <ul>
            <li><strong>Hardware:</strong> Conexión de controladores de motores (L298N), sensores y alimentación externa.</li>
            <li><strong>Software:</strong> Programación en C++ (IDE de Arduino) y gestión de bibliotecas de movimiento.</li>
            <li><strong>Fabricación Digital:</strong> Uso de software de modelado 3D e impresión para la creación de componentes físicos únicos.</li>
            <li><strong>Resolución de Problemas:</strong> Diagnóstico de fallos en circuitos y depuración de errores lógicos en el código.</li>
        </ul>
    </details>

    <details>
        <summary><strong>🔧 REQUISITOS TÉCNICOS Y MATERIALES</strong></summary>
        <p><strong>FÍSICOS</strong></p>
        <ul>
            <li>2 Kits de Coche Arduino (Chasis, motores, ruedas)</li>
            <li>Placas Arduino (Uno/Elegoo)</li>
            <li>Servomotores (para el movimiento del arma)</li>
            <li>Globos (Punto débil)</li>
            <li>Armas punzantes (Chinchetas, agujas o plástico afilado 3D)</li>
            <li>Material de oficina (Cartón, bridas, cinta americana)</li>
            <li>Impresora 3D (para soportes personalizados)</li>
        </ul>
        <p><strong>LÓGICOS</strong></p>
        <ul>
            <li>Arduino IDE (Entorno de desarrollo)</li>
            <li>Bibliotecas: <code>Servo.h</code>, <code>NewPing.h</code> (si se usan sensores)</li>
            <li>Tinkercad / Fusion 360 (Diseño 3D)</li>
            <li>Github (Control de versiones del código)</li>
        </ul>
    </details>

    <h2>📋 METODOLOGÍA DE TRABAJO</h2>
    <details>
        <summary><strong>FASES DE IMPLEMENTACIÓN</strong></summary>
        <ol>
            <li><strong>Creación de los coches:</strong> Ensamblaje de la estructura base y conexión de motores y baterías.</li>
            <li><strong>Desarrollo del Código:</strong> Implementación de la lógica de movimiento y pruebas de respuesta.</li>
            <li><strong>Diseño de Armamento:</strong> Prototipado del objeto punzante y su mecanismo de accionamiento.</li>
            <li><strong>Integración 3D:</strong> Impresión de soportes para fijar el arma y el globo de forma segura al chasis.</li>
            <li><strong>Pruebas de Combate:</strong> Testeo de colisiones y efectividad de perforación.</li>
        </ol>
    </details>

    <h2>📖 RECURSOS Y DOCUMENTACIÓN</h2>
    <details>
        <summary><strong>GUÍAS Y TUTORIALES</strong></summary>
        <p>Contamos con documentación técnica de alta calidad para el montaje base:</p>
        <ul>
            <li><strong>Documentación oficial:</strong> <a href="https://docs.keyestudio.com/projects/KS0470/en/latest/" target="_blank">Keyestudio KS0470 Smart Car</a></li>
            <li>En este enlace se encuentran los esquemas eléctricos y ejemplos de código necesarios para el movimiento inicial.</li>
        </ul>
    </details>

    <h2>⚠️ DESAFÍOS Y SOLUCIONES</h2>
    <details>
        <summary><strong>IDENTIFICACIÓN DE RIESGOS</strong></summary>
        <table>
            <tr><th>Desafío</th><th>Estrategia / Solución Prevista</th></tr>
            <tr><td>Elección del Chasis</td><td>Decidir entre kit pre-hecho por rapidez o diseño propio para mayor personalización.</td></tr>
            <tr><td>Mecanismo de Ataque</td><td>Evaluar si el arma será fija o móvil mediante un servomotor.</td></tr>
            <tr><td>Estabilidad del Punto Débil</td><td>Diseñar un soporte 3D que mantenga el globo rígido pero expuesto.</td></tr>
            <tr><td>Consumo de Energía</td><td>Uso de baterías Li-ion separadas para motores y placa Arduino.</td></tr>
        </table>
    </details>

    <h2>🌐 RED Y CONECTIVIDAD</h2>
    <details>
        <summary><strong>DIAGRAMA DE CONEXIÓN (HARDWARE)</strong></summary>
        <p>Esencial para entender el flujo de energía y datos entre los componentes.</p>
        <!-- Aquí se puede insertar un diagrama si se dispone de él -->
    </details>

    <h2>🏁 FASE FINAL</h2>
    <details>
        <summary><strong>🚗 COCHE FUNCIONAL CONSEGUIDO</strong></summary>
        <p>El coche ya funciona con la APP móvil y con sus 4 direcciones/funciones completamente operativas y listas para el combate.</p>
        <div class="video-container">
            <video controls>
                <source src="https://github.com/user-attachments/assets/e5bbce68-fe37-42ff-8248-b45136dbe03e" type="video/mp4">
            </video>
        </div>
        <div class="image-gallery">
            <img src="https://github.com/user-attachments/assets/f8f634c8-66e0-4ebc-a0ed-b66b418d404e" alt="Coche 1">
            <img src="https://github.com/user-attachments/assets/a8d97b2d-622d-4182-9276-6df5d3daf131" alt="Coche 2">
            <img src="https://github.com/user-attachments/assets/2a49c4ed-6ab8-4e30-9bfb-4af07cb21a8e" alt="Coche 3">
        </div>
    </details>

    <div class="footer">
        <p>📌 Documentación oficial del proyecto Arduino - La Elite</p>
        <p>© 2026 - Todos los derechos reservados</p>
    </div>

</div>
</body>
</html>
