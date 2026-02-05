# Robotics-Task
Study Arduino Basics a.Arduino Programming Structure b.How Arduino knowledge helps in learning ESP-IDF

Solution:
a.A interface used to write,upload Program written in C or C++ Programming Language to the Arduino Boards is known as Arduino Integrated Development Environment(IDE).
It contains two main specific Functions without those it cannot compile.Those are

1.void setup() :These functions runs only one time and is used to initialize variables, pin modes, and start using libraries.

2.void loop() : After setup function is finished loop function starts.It contains the important line of Program need to be implemented.It is used to actively control the Arduino board.
This is where the main logic lives.

As in the Arduino IDE mainly C or C++ language is used it contains same variable and datatypes(for example int for integer,boolean for true or false) or control flow statements(for example if,else).
Additionaly It also contains some built in commands like pinmode(pin,mode),digitalWrite(pin, value),digitalRead(pin),analogRead(pin),analogWrite(pin, value),etc. This commands are very important and used for interacting with the Hardware Pins.

b.ESP-IDF is the official, open-source software development framework provided by Espressif Systems for their ESP32 systems.Similar to the Arduino IDE it uses C/C++ Programming language to write,upload to the Hardware.Like Arduino it also has inbuilt commands(For example digitalWrite(pin, value) in Arduino is similar to gpio_set_level() in ESPIDF.If you will try to directly Learn ESP IDF you will feel it harder But if you have the knowledge of Arduino IDE it will be simpler to get into the ESP IDF.As Arduino circuits are not as complex as ESP32 circuits.

Explanation of Coding task of writing Arduino Program for having a button for ON or OFF led and also changing speed using delay:The LED is connected to pin 9 and brightness of LED is controlled by PWM to create blinking effect. A button on pin 2 is used as a switch, so if it is press it turns the blinking effect ON or OFF. The INPUT_PULLUP mode is used for the button, meaning it reads LOW when pressed. When enabled, the LED brightness increases and decreases automatically; when disabled, the LED remains OFF.
