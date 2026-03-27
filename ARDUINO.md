<div align="center">

# <img src="https://github.com/user-attachments/assets/189fe64c-3da7-48c4-b756-e1004be34eb6" width="60" style="vertical-align: middle;"> ARDUINO

### Plataforma de código abierto para la creación electrónica

</div>

---

## 📌 ¿Qué es Arduino?

Arduino es una plataforma de creación electrónica de código abierto que se compone de dos partes principales: la física y la digital. Su filosofía se basa en la simplicidad, la accesibilidad y la flexibilidad, lo que la convierte en la herramienta ideal tanto para artistas, diseñadores y aficionados como para profesionales y educadores.

<details>
<summary><strong>📱 Parte Física (Hardware)</strong></summary>

La parte física está compuesta por una placa de circuito impreso (PCB) que actúa como el cerebro del proyecto. Esta placa integra un microcontrolador que puedes programar para interactuar con el mundo exterior, conectando sensores, actuadores, motores y otros componentes electrónicos a sus pines de entrada y salida. Es un lienzo en blanco listo para ser modificado y manejado según tu creatividad.

<div align="center">
  <img src="assets/ardfisico.png" alt="Placa Arduino física" width="80%">
</div>

</details>

<details>
<summary><strong>💻 Parte Digital (Software)</strong></summary>

La parte digital es el entorno de desarrollo integrado (IDE) de Arduino. Es el lugar donde escribes el código, utilizando un lenguaje basado en C/C++ simplificado. Aquí es donde das vida a tu proyecto, creando una serie de instrucciones lógicas que le indican a la placa qué hacer, cómo reaccionar a los estímulos externos y cómo controlar los componentes conectados.

<div align="center">
  <img src="assets/IDEar.png" alt="IDE de Arduino" width="80%">
</div>

</details>

---

## 🌍 ¿Cuál es su origen?

Arduino nació en **2005** en el **Instituto de Diseño Interactivo de Ivrea, Italia**. Fue creado por un equipo de estudiantes y profesores, liderado por **Massimo Banzi**, con el objetivo de ofrecer a los estudiantes una herramienta de proyectos electrónica que fuera **sencilla, de bajo coste y rápida de aprender**, a diferencia de las complejas y costosas placas de desarrollo de la época.

<div align="center">
  <img src="assets/notch.png" alt="Origen de Arduino" width="60%">
</div>

Tras el cierre del instituto, el equipo decidió liberar el proyecto bajo licencias de **código abierto**. Esta decisión impulsó su fama mundial, creando una comunidad global de makers, ingenieros y artistas que continúan contribuyendo a su evolución.

---

## ⭐ Características más importantes

Arduino se distingue por ser una plataforma de **código abierto**, lo que significa que tanto su hardware como su software son libres y están disponibles para que cualquiera los estudie, modifique y distribuya. De esta filosofía se derivan sus dos factores más importantes:

| Característica | Descripción |
|----------------|-------------|
| 🎨 **Creatividad y Flexibilidad** | Su principal fortaleza es la capacidad de adaptarse a una infinidad de proyectos. Es ideal para principiantes gracias a un lenguaje de programación simple y una comunidad que ofrece una vasta cantidad de tutoriales y ejemplos. |
| 💰 **Bajo Coste y Accesibilidad** | Su bajo coste en comparación con otras plataformas de desarrollo lo hace accesible para escuelas, aficionados y proyectos personales, eliminando la barrera económica para la experimentación y el aprendizaje. |

---

## 📦 Modelos de Arduino

Existen diversos modelos de placas Arduino, cada una diseñada para satisfacer necesidades específicas. Los más populares incluyen:

| Modelo | Voltaje | Pines Digitales | Entradas Analógicas | Memoria Flash | Velocidad |
|--------|---------|-----------------|---------------------|---------------|-----------|
| **Arduino Uno** | 5V | 14 | 6 | 32KB | 16 MHz |
| **Arduino Mega** | 5V | 54 | 16 | 256KB | 16 MHz |
| **Arduino Nano** | 5V | 14 | 8 | 32KB | 16 MHz |
| **Arduino Leonardo** | 5V | 20 | 12 | 32KB | 16 MHz |
| **ESP32-S3 WROOM** | 3.3V | 36 | 18 | 512KB | 240 MHz |

<div align="center">
  <img src="assets/ardmodelo.png" alt="Modelos de Arduino" width="80%">
</div>

---

## 🛠️ ¿Para qué sirve?

Arduino es una herramienta versátil que sirve para crear una gran cantidad de proyectos electrónicos y de robótica. Es ampliamente utilizado en entornos educativos para enseñar programación, electrónica y pensamiento computacional.

### 🏠 Sistemas para casas inteligentes (Domótica)
Controla luces, persianas, electrodomésticos y sistemas de seguridad. Conecta sensores de temperatura, humedad, presencia y actuadores para crear un hogar automatizado y eficiente.

<div align="center">
  <img src="assets/casaar.png" alt="Domótica con Arduino" width="70%">
</div>

### 🏢 Automatización en edificios e industria
Controla sistemas de climatización, iluminación y accesos en edificios. En entornos industriales, sirve para monitorear maquinaria, controlar procesos y crear sistemas de adquisición de datos.

<div align="center">
  <img src="assets/edar.png" alt="Automatización industrial" width="70%">
</div>

---

## 💬 ¿Qué lenguaje utiliza?

Arduino se programa utilizando un lenguaje basado en **C/C++**, simplificado y adaptado para facilitar la interacción con los periféricos de la placa.

```cpp
pinMode(pin, modo);      // Configura un pin como INPUT o OUTPUT
digitalWrite(pin, valor); // Escribe HIGH o LOW en un pin digital
digitalRead(pin);         // Lee el estado de un pin digital
analogRead(pin);          // Lee un valor analógico (0-1023)
analogWrite(pin, valor);  // Escribe un valor PWM (0-255)
delay(ms);                // Pausa la ejecución por ms milisegundos
Serial.begin(velocidad);  // Inicia comunicación serie
Serial.print(dato);       // Envía datos por puerto serie
<div align="center"> <img src="assets/cplus.png" alt="Lenguaje C++" width="40%"> </div>
🖥️ ¿Qué es el IDE?
El Arduino IDE (Entorno de Desarrollo Integrado) es la aplicación oficial y gratuita que se utiliza para escribir, compilar y cargar el código a la placa Arduino. Proporciona una interfaz sencilla con un editor de texto, un área de mensajes, una consola de texto y una barra de herramientas con botones para las funciones más comunes.

<div align="center"> <img src="assets/IDEard.png" alt="Arduino IDE" width="80%"> </div>
🔧 PRÁCTICAS CON ARDUINO
💡 ACTIVIDAD 0: BLINK
Objetivo: Utilizar el ESP32-S3 WROOM para controlar el parpadeo de un LED integrado en la placa. Este es el "Hola Mundo" de la electrónica.

Lista de componentes:

<div align="center"> <img src="assets/compblink.png" alt="Componentes Blink"> </div><details> <summary><strong>🔍 LED azul que parpadea</strong></summary>
El código "Blink" hace que un LED (normalmente el integrado en la placa, conectado al pin 2 en el ESP32-S3) se encienda y apague de forma repetida. Esto sirve para confirmar que la placa y el software están funcionando correctamente.

</details><details> <summary><strong>📝 void setup() y void loop()</strong></summary>
void setup(): Se ejecuta una sola vez al iniciar la placa. Configura el estado inicial de los componentes.

void loop(): Se ejecuta de forma continua e infinita. Contiene las instrucciones que se repiten constantemente.

</details><details> <summary><strong>🏷️ #define LED_BUILTIN 2</strong></summary>
Define una constante. Reemplaza cualquier aparición de LED_BUILTIN por el número 2, haciendo el código más legible.

</details><details> <summary><strong>⏱️ delay(1000)</strong></summary>
Pausa la ejecución del programa durante el tiempo especificado en milisegundos (1000 ms = 1 segundo).

</details>
Código:

cpp
#define LED_BUILTIN 2

void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
}
🔴 ACTIVIDAD 1: LED EXTERNO
Objetivo: Controlar un LED externo usando la placa ESP32-S3 WROOM.

Lista de componentes:

<div align="center"> <img src="assets/compLED.png" alt="Componentes LED"> </div>
Esquema del circuito:

<div align="center"> <img src="assets/semaforo1.png" alt="Circuito LED 1" width="45%"> <img src="assets/semaforo2.png" alt="Circuito LED 2" width="45%"> </div>
Código:

cpp
#define LED_PIN 13

void setup() {
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_PIN, HIGH);
  delay(1000);
  digitalWrite(LED_PIN, LOW);
  delay(1000);
}
Resultado:

<div align="center"> <img src="assets/LEDfoto1.png" alt="LED encendido" width="45%"> <img src="assets/LEDfoto2.png" alt="LED apagado" width="45%"> </div>
<video src="https://github.com/user-attachments/assets/49e49177-718f-447d-90b8-2797805de5da" controls width="100%"></video>

🚦 ACTIVIDAD 2: SEMÁFORO
Objetivo: Simular un semáforo con tres LEDs (rojo, amarillo, verde).

Componentes necesarios:

<div align="center"> <img src="assets/componentesema.png" alt="Componentes semáforo"> </div>
Código:

cpp
#define RED_PIN 10
#define YELLOW_PIN 9
#define GREEN_PIN 8

void setup() {
  pinMode(RED_PIN, OUTPUT);
  pinMode(YELLOW_PIN, OUTPUT);
  pinMode(GREEN_PIN, OUTPUT);
}

void loop() {
  // Rojo
  digitalWrite(RED_PIN, HIGH);
  delay(5000);
  
  // Verde
  digitalWrite(RED_PIN, LOW);
  digitalWrite(GREEN_PIN, HIGH);
  delay(5000);
  
  // Amarillo
  digitalWrite(GREEN_PIN, LOW);
  digitalWrite(YELLOW_PIN, HIGH);
  delay(2000);
  
  digitalWrite(YELLOW_PIN, LOW);
}
Esquema del circuito:

<div align="center"> <img src="assets/esquemasem.png" alt="Esquema semáforo"> </div>
<video src="https://github.com/user-attachments/assets/5c37b494-c140-4cbd-9c3f-217365d051c2" controls width="100%"></video>

🔘 ACTIVIDAD 3: BOTÓN Y LED
Objetivo: Encender un LED mientras se presiona un botón.

Componentes necesarios:

<div align="center"> <img src="assets/componentesardact3.png" alt="Componentes botón"> </div>
Código:

cpp
#define LED_PIN 13
#define BUTTON_PIN 2

void setup() {
  pinMode(LED_PIN, OUTPUT);
  pinMode(BUTTON_PIN, INPUT);
}

void loop() {
  if (digitalRead(BUTTON_PIN) == HIGH) {
    digitalWrite(LED_PIN, HIGH);
  } else {
    digitalWrite(LED_PIN, LOW);
  }
}
Esquema del circuito:

<div align="center"> <img src="assets/esquemaact3ard.png" alt="Esquema botón"> </div>
<video src="https://github.com/user-attachments/assets/34f02e2f-5f67-45fd-9deb-352e842ec188" controls width="100%"></video>

💡 ACTIVIDAD 4: MINI LÁMPARA DE MESA
Objetivo: Crear un interruptor tipo lámpara (pulsar para encender/apagar).

Código:

cpp
#define LED_PIN 13
#define BUTTON_PIN 2

bool ledState = false;
bool lastButtonState = LOW;
unsigned long lastDebounceTime = 0;
const unsigned long debounceDelay = 50;

void setup() {
  pinMode(LED_PIN, OUTPUT);
  pinMode(BUTTON_PIN, INPUT);
}

void loop() {
  bool reading = digitalRead(BUTTON_PIN);
  
  if (reading != lastButtonState) {
    lastDebounceTime = millis();
  }
  
  if ((millis() - lastDebounceTime) > debounceDelay) {
    if (reading != ledState) {
      ledState = reading;
      if (ledState == HIGH) {
        digitalWrite(LED_PIN, !digitalRead(LED_PIN));
      }
    }
  }
  
  lastButtonState = reading;
}
Esquema del circuito:

<div align="center"> <img src="assets/ARDACT4.png" alt="Mini lámpara"> <img src="assets/esquemaact3ard.png" alt="Esquema lámpara"> </div>
<video src="https://github.com/user-attachments/assets/0b8667d9-59fc-4b6e-8603-20c494ff2526" controls width="100%"></video>

🌈 ACTIVIDAD 5: LED RGB
Objetivo: Controlar un LED RGB para generar diferentes colores usando PWM.

Componentes necesarios:

<div align="center"> <img src="assets/componentesact5.png" alt="Componentes RGB"> </div>
Comparativa LED normal vs LED RGB:

<div align="center"> <img src="assets/diferenciasledrgb.png" alt="Diferencias LED vs RGB"> </div>
Preguntas y respuestas:

<details> <summary><strong>❓ 1. Analizar y entender la diferencia entre un LED normal a un LED RGB</strong></summary>
Característica	LED Normal	LED RGB
Número de pines	2 (ánodo y cátodo)	4 (ánodo común o cátodo común + 3 colores)
Colores	Un solo color (rojo, verde, azul, etc.)	Múltiples colores combinando rojo, verde y azul
Control	Encendido/apagado simple	Control de intensidad por PWM para cada color
Aplicaciones	Indicadores básicos	Iluminación decorativa, efectos de color
Costo	Bajo	Moderado
</details><details> <summary><strong>❓ 2. ¿Qué ocurriría en caso de invertir los colores del LED RGB?</strong></summary>
El LED seguirá funcionando, pero los colores mostrados no coincidirán con lo programado. Si el código intenta mostrar rojo (activando el pin conectado al ánodo rojo), pero ese pin está conectado al ánodo verde del LED, veremos luz verde. Esto se debe a que la correspondencia física entre el pin de control y la pata del LED ha sido alterada.

</details><details> <summary><strong>❓ 3. ¿Qué sucede si comentamos la llamada a setColor()?</strong></summary>
Si comentamos la línea que llama a setColor(), el LED no cambiará de estado. El programa seguirá calculando nuevos valores para red, green y blue, pero nunca los enviará a los pines del LED. Por lo tanto, el LED permanecerá en su último estado o apagado.

</details>
Código básico (colores aleatorios):

cpp
#define RED_RGB 9
#define GREEN_RGB 10
#define BLUE_RGB 11

void setup() {
  pinMode(RED_RGB, OUTPUT);
  pinMode(GREEN_RGB, OUTPUT);
  pinMode(BLUE_RGB, OUTPUT);
}

void setColor(int red, int green, int blue) {
  analogWrite(RED_RGB, red);
  analogWrite(GREEN_RGB, green);
  analogWrite(BLUE_RGB, blue);
}

void loop() {
  setColor(random(0, 256), random(0, 256), random(0, 256));
  delay(1000);
}
Esquema del circuito:

<div align="center"> <img src="assets/ARDACT5.png" alt="Circuito RGB"> <img src="assets/circuitodiseñoact5.png" alt="Esquema RGB"> </div>
<video src="https://github.com/user-attachments/assets/d7e50a8a-eafa-423a-b32d-957b739f9aee" controls width="100%"></video>

Código con gradiente (transición suave):
<video src="https://github.com/user-attachments/assets/27c91968-7255-46bf-b115-0f35ceff82e2" controls width="100%"></video>

<details> <summary><strong>❓ Preguntas sobre el gradiente</strong></summary>
1. ¿Qué observa tras cargar y correr el código del programa?
El color cambia de forma suave y fluida, realizando una transición continua entre colores. En el código, esta transición se logra porque los valores RGB se modifican de manera incremental y lineal.

2. Explique qué es el tipo de dato long y su diferencia con el int
long es un tipo de dato entero que ocupa 4 bytes y puede almacenar números mucho más grandes que int (2 bytes). Se utiliza para valores como los códigos de color en formato hexadecimal.

3. Explique el funcionamiento de la función wheel
La función wheel toma un valor de posición (0-1530) y lo traduce a una combinación específica de valores RGB correspondiente a un punto en un círculo cromático.

4. ¿Para qué se utiliza la función ledcWrite()?
ledcWrite() es una función específica del ESP32 para generar señal PWM en un canal específico, controlando el brillo de cada color del LED RGB.

</details>
📊 ACTIVIDAD 6: BARRA DE LEDS
Objetivo: Controlar una barra de 10 LEDs de forma secuencial.

Componentes necesarios:

<div align="center"> <img src="https://github.com/user-attachments/assets/dff35936-e52d-4d51-bc86-b110242286b6" alt="Componentes barra" width="60%"> </div>
Pines utilizados: 0, 2, 15, 34, 35, 32, 33, 25, 26, 27

Código base:

cpp
int ledPins[] = {0, 2, 15, 34, 35, 32, 33, 25, 26, 27};
int numLeds = 10;

void setup() {
  for (int i = 0; i < numLeds; i++) {
    pinMode(ledPins[i], OUTPUT);
  }
}

void loop() {
  for (int i = 0; i < numLeds; i++) {
    digitalWrite(ledPins[i], HIGH);
    delay(100);
    digitalWrite(ledPins[i], LOW);
  }
  
  for (int i = numLeds - 1; i >= 0; i--) {
    digitalWrite(ledPins[i], HIGH);
    delay(100);
    digitalWrite(ledPins[i], LOW);
  }
}
Código con inicio en el medio:

<div align="center"> <img src="https://github.com/user-attachments/assets/aaeac552-5316-45df-bdd4-0ff0316671c9" alt="Código inicio medio" width="80%"> </div>
Código con botón de avance:

<div align="center"> <img src="https://github.com/user-attachments/assets/d5c11915-8f38-4d21-8179-b976f52ece59" alt="Código con botón" width="80%"> </div>
<video src="https://github.com/user-attachments/assets/9b86fa40-f2c8-4c18-9ef7-e1f5b1ab03fb" controls width="100%"></video>

📡 ACTIVIDAD 7: COMUNICACIÓN SERIE
Proyecto 7.1: Comunicación Serie
Objetivo: Enviar y recibir datos entre Arduino y el ordenador.

Componentes necesarios:

<div align="center"> <img src="https://github.com/user-attachments/assets/fd8e00cd-7c35-4cf0-98f1-6df1c6f81409" alt="Comunicación serie"> </div>
Código:

cpp
void setup() {
  Serial.begin(115200);
  Serial.println("Sistema iniciado correctamente");
}

void loop() {
  static unsigned long lastTime = 0;
  
  if (millis() - lastTime >= 1000) {
    lastTime = millis();
    Serial.print("Tiempo transcurrido: ");
    Serial.print(millis() / 1000.0, 1);
    Serial.println(" s");
  }
  
  if (Serial.available() > 0) {
    char comando = Serial.read();
    Serial.print("Comando recibido: ");
    Serial.println(comando);
  }
}
Monitor Serie:

<div align="center"> <img src="https://github.com/user-attachments/assets/0a86607f-5be4-41df-b94d-432a28a66b99" alt="Monitor serie" width="80%"> <img src="https://github.com/user-attachments/assets/326b4274-3682-4340-957f-ccca54e1ae68" alt="Salida serie" width="60%"> </div><details> <summary><strong>❓ Preguntas sobre comunicación serie</strong></summary>
1. ¿Qué aparece en el monitor serie?
Aparece el texto programado, generalmente un mensaje que se repite en el loop(), como un contador de tiempo.

2. ¿Qué ocurre al pulsar BOOT+EN y solo EN?

BOOT+EN: Pone la placa en modo de descarga para cargar nuevo programa.

EN (Reset): Reinicia el microcontrolador, reiniciando la ejecución desde setup().

3. ¿Qué indica Serial.begin(115200);?
Inicia la comunicación serie a 115200 baudios. Debe coincidir con la velocidad seleccionada en el Monitor Serie.

4. ¿Qué significa "%.1f s\n"?
Es una cadena de formato para printf: % indica variable, .1f es decimal con un decimal, s es la letra literal, \n es salto de línea.

</details>
Proyecto 7.2: Pantalla LCD 1602 con I2C
Objetivo: Mostrar información en una pantalla LCD usando solo 4 cables.

Componentes necesarios:

<div align="center"> <img src="https://github.com/user-attachments/assets/9e261a64-466b-4d1d-a769-052f8d04ec9f" alt="LCD I2C"> </div>
Conexiones:

SCL: Señal de reloj sincronizada (protocolo I2C)

SDA: Línea de transmisión de datos bidireccional

VCC: Alimentación (5V)

GND: Conexión a tierra

Código con desplazamiento de texto:

<div align="center"> <img src="https://github.com/user-attachments/assets/dfa86304-f55f-4ef7-8fc6-480feb34eacd" alt="Código LCD desplazamiento" width="80%"> <img src="https://github.com/user-attachments/assets/51e32b1a-8f84-4ed3-9abf-789cdf6aee27" alt="LCD en acción" width="60%"> </div>
Proyecto 7.3: Higrotermógrafo (Sensor DHT11)
Objetivo: Medir temperatura y humedad y mostrarlos en la pantalla LCD.

Componentes necesarios:

<div align="center"> <img src="https://github.com/user-attachments/assets/22d986ab-f5ab-4ee3-ab0f-cfa45b894e61" alt="Sensor DHT11"> </div>
Código con conversión a Kelvin y Fahrenheit:

<div align="center"> <img src="https://github.com/user-attachments/assets/8c83d05d-8b0c-4a97-9eef-af15af589cd9" alt="Código DHT Kelvin Fahrenheit" width="80%"> </div>
📶 ACTIVIDAD 8: WIFI
Modo Station (Estación)
Objetivo: Conectar el ESP32 a una red WiFi existente (2.4GHz exclusivamente).

<div align="center"> <img src="https://github.com/user-attachments/assets/58f48420-a8b5-4f97-92b1-5d8a140f90df" alt="Modo Station"> </div><details> <summary><strong>❓ Preguntas sobre WiFi</strong></summary>
¿A qué red te has podido conectar?
El ESP32-S3 se conecta exclusivamente a redes de 2.4 GHz. Su hardware no soporta la banda de 5 GHz.

¿Son necesarias las tres librerías?
No. Para el modo Station básico solo se necesita WiFi.h, que ya incluye las funciones fundamentales.

¿En qué casos se usan WiFiClient.h y WiFiClientSecure.h?

WiFiClient.h: Para comunicación estándar con otros dispositivos o servidores.

WiFiClientSecure.h: Para comunicaciones cifradas y seguras (HTTPS, SSL/TLS).

¿Es posible seleccionar el canal de comunicación?
Sí, es posible para evitar saturación de canales y optimizar la calidad de la conexión.

</details>
Modo Access Point (Punto de Acceso)
Objetivo: Crear una red WiFi propia con el ESP32.

<div align="center"> <img src="https://github.com/user-attachments/assets/70fcf3f4-29c4-42e6-857f-315bf2a1908e" alt="Código AP" width="80%"> </div><details> <summary><strong>❓ Preguntas sobre Modo AP</strong></summary>
¿Cuál es el uso de softAPConfig?
Permite establecer una configuración de red específica y manual para el punto de acceso que crea el ESP32.

¿Cómo conocer la cantidad de dispositivos conectados?
Mediante WiFi.softAPgetStationNum(), que devuelve un entero con el número de clientes vinculados.

¿Qué método permite visualizar la IP del AP?
WiFi.softAPIP() devuelve la dirección IP que el ESP32 tiene dentro de la red que él mismo ha creado.

¿Qué permite la opción c_str()?
Convierte un objeto String en una cadena de caracteres estilo C (char*), útil para funciones que requieren este formato.

</details>
Modo AP + Station
Objetivo: Actuar como cliente y punto de acceso simultáneamente.

<div align="center"> <img src="https://github.com/user-attachments/assets/d37aa673-0eae-4675-ba4d-4f444b42da7f" alt="Modo AP+Station" width="80%"> </div>
Servidor Web en el ESP32
Objetivo: Crear una página web alojada en el ESP32.

<div align="center"> <img src="https://github.com/user-attachments/assets/d12ee6e1-c8cd-4985-8da1-7f8e3103e3b1" alt="Servidor web ESP32" width="80%"> </div><details> <summary><strong>❓ Preguntas sobre servidor web</strong></summary>
Explica los parámetros de server.send():

Parámetro	Ejemplo	Significado
Código HTTP	200 / 404	200 = OK (éxito), 404 = Not Found (no encontrado)
Tipo de contenido	"text/html" / "text/plain"	Indica si es HTML (renderizable) o texto plano
Cuerpo del mensaje	SendHTML() / "No hay respuesta"	Contenido real que se muestra en el navegador
</details>
⚔️ PROYECTO FINAL: ACERO IMPURO
<div align="center"> <img src="assets/logoacero.png" alt="Logo Acero Impuro" width="200"> </div>
🏆 Introducción
Elite Arduino Battle es un proyecto de robótica competitiva desarrollado por el equipo "La Elite". Consiste en el diseño, programación y ensamblaje de dos vehículos autónomos o controlados por Arduino, equipados con sistemas de ataque y defensa para combate en arena.

El objetivo fundamental es la supervivencia: cada coche protege un punto débil (globo) mientras intenta perforar el del adversario mediante un arma frontal personalizada.

Fundadores del proyecto: Equipo La Elite

❓ ¿Por qué esta idea?
Como entusiastas de la tecnología, buscábamos un proyecto que combinara la programación lógica con la ingeniería física. La idea de los "Coches de Combate" nos permite experimentar con la movilidad, el diseño de estructuras en 3D y la estrategia en tiempo real.

Además, este proyecto nos apasiona porque traslada la competitividad de los videojuegos al mundo real, permitiéndonos ver físicamente el resultado de nuestro código y diseño mecánico.

🎯 ¿Hasta dónde queremos llegar?
Objetivo	Descripción
Control Total	Dominar el manejo de motores y sensores mediante código limpio y eficiente
Diseño e Impresión 3D	Crear piezas personalizadas para el soporte de armas y blindaje, optimizando peso y resistencia
Autonomía y Respuesta	Conseguir que el sistema de ataque sea funcional y el chasis soporte el impacto
Aprendizaje Técnico	Documentar todo el proceso para servir de base a futuros proyectos de robótica
📚 Objetivos de Aprendizaje
Hardware: Conexión de controladores de motores (L298N), sensores y alimentación externa

Software: Programación en C++ (IDE de Arduino) y gestión de bibliotecas de movimiento

Fabricación Digital: Uso de software de modelado 3D e impresión para componentes físicos únicos

Resolución de Problemas: Diagnóstico de fallos en circuitos y depuración de errores lógicos

🔧 Requisitos Técnicos y Materiales
Físicos
2 Kits de Coche Arduino (Chasis, motores, ruedas)

Placas Arduino (Uno/Elegoo)

Controlador de motores L298N

Servomotores (para el movimiento del arma)

Módulo Bluetooth HC-05

Batería Li-ion (7.4V o 11.1V)

Globos (Punto débil)

Armas punzantes (Chinchetas, agujas o plástico afilado 3D)

Impresora 3D (para soportes personalizados)

Lógicos
Arduino IDE (Entorno de desarrollo)

Bibliotecas: Servo.h, SoftwareSerial.h, NewPing.h (opcional)

Tinkercad / Fusion 360 (Diseño 3D)

GitHub (Control de versiones)

📋 Metodología de Trabajo
<details> <summary><strong>Fases de Implementación</strong></summary>
Creación de los coches: Ensamblaje de la estructura base y conexión de motores y baterías

Desarrollo del Código: Implementación de la lógica de movimiento y pruebas de respuesta

Diseño de Armamento: Prototipado del objeto punzante y su mecanismo de accionamiento

Integración 3D: Impresión de soportes para fijar el arma y el globo al chasis

Pruebas de Combate: Testeo de colisiones y efectividad de perforación

</details>
💻 Código Base del Coche de Combate
cpp
#include <SoftwareSerial.h>
#include <Servo.h>

// Pines del controlador de motores L298N
#define ENA 5   // PWM motor A
#define ENB 6   // PWM motor B
#define IN1 7
#define IN2 8
#define IN3 9
#define IN4 10

// Pin del servomotor (arma)
#define SERVO_PIN 11

// Pines del módulo Bluetooth
#define BT_RX 2
#define BT_TX 3

SoftwareSerial bluetooth(BT_RX, BT_TX);
Servo arma;

int velocidad = 150;
char comando;

void setup() {
  // Configurar pines de motores
  pinMode(ENA, OUTPUT);
  pinMode(ENB, OUTPUT);
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);
  pinMode(IN3, OUTPUT);
  pinMode(IN4, OUTPUT);
  
  // Configurar servomotor
  arma.attach(SERVO_PIN);
  arma.write(0);  // Posición inicial (armada)
  
  // Iniciar comunicación
  Serial.begin(9600);
  bluetooth.begin(9600);
  
  Serial.println("Sistema de combate iniciado");
}

void loop() {
  if (bluetooth.available()) {
    comando = bluetooth.read();
    
    switch (comando) {
      case 'F': moverAdelante(); break;
      case 'B': moverAtras(); break;
      case 'L': girarIzquierda(); break;
      case 'R': girarDerecha(); break;
      case 'S': parar(); break;
      case 'A': atacar(); break;
    }
  }
}

void moverAdelante() {
  digitalWrite(IN1, HIGH); digitalWrite(IN2, LOW);
  digitalWrite(IN3, HIGH); digitalWrite(IN4, LOW);
  analogWrite(ENA, velocidad); analogWrite(ENB, velocidad);
}

void moverAtras() {
  digitalWrite(IN1, LOW); digitalWrite(IN2, HIGH);
  digitalWrite(IN3, LOW); digitalWrite(IN4, HIGH);
  analogWrite(ENA, velocidad); analogWrite(ENB, velocidad);
}

void girarIzquierda() {
  digitalWrite(IN1, LOW); digitalWrite(IN2, HIGH);
  digitalWrite(IN3, HIGH); digitalWrite(IN4, LOW);
  analogWrite(ENA, velocidad); analogWrite(ENB, velocidad);
}

void girarDerecha() {
  digitalWrite(IN1, HIGH); digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW); digitalWrite(IN4, HIGH);
  analogWrite(ENA, velocidad); analogWrite(ENB, velocidad);
}

void parar() {
  digitalWrite(IN1, LOW); digitalWrite(IN2, LOW);
  digitalWrite(IN3, LOW); digitalWrite(IN4, LOW);
  analogWrite(ENA, 0); analogWrite(ENB, 0);
}

void atacar() {
  arma.write(90);   // Extender arma
  delay(500);
  arma.write(0);    // Retraer arma
}
⚠️ Desafíos y Soluciones
Desafío	Estrategia / Solución Prevista
Elección del Chasis	Decidir entre kit pre-hecho por rapidez o diseño propio para mayor personalización
Mecanismo de Ataque	Evaluar si el arma será fija o móvil mediante un servomotor
Estabilidad del Punto Débil	Diseñar un soporte 3D que mantenga el globo rígido pero expuesto
Consumo de Energía	Uso de baterías Li-ion separadas para motores y placa Arduino
📖 Recursos y Documentación
<details> <summary><strong>Guías y Tutoriales</strong></summary>
Contamos con documentación técnica de alta calidad para el montaje base:

Documentación oficial: Keyestudio KS0470 Smart Car

En este enlace se encuentran los esquemas eléctricos y ejemplos de código necesarios para el movimiento inicial.

</details>
🏁 Fase Final: Coche Funcional Conseguido
El coche ya funciona con la APP móvil y con sus 4 direcciones/funciones completamente operativas y listas para el combate.

<video src="https://github.com/user-attachments/assets/e5bbce68-fe37-42ff-8248-b45136dbe03e" controls width="100%"></video>

<div align="center"> <img src="https://github.com/user-attachments/assets/f8f634c8-66e0-4ebc-a0ed-b66b418d404e" width="30%"> <img src="https://github.com/user-attachments/assets/a8d97b2d-622d-4182-9276-6df5d3daf131" width="30%"> <img src="https://github.com/user-attachments/assets/2a49c4ed-6ab8-4e30-9bfb-4af07cb21a8e" width="30%"> </div>
