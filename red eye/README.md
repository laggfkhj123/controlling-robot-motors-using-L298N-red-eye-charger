Robot Eye
This is a circuit design to transform 9v power supply to 5v, to feed power for LED ; and controlled by Arduino
Implementation Steps
78L05 regulator, for step down the voltage to 5v.

two LED, to work as the eye of the robot.

resistor, to adjust current, the appropriate current for led is between 10mA -30mA, so I chose 11mA to save power.

9v battery.

transistor, to work as a switch.

Arduino, to control transistor.

code designed to off and on switch 60 times in a second to save power.

void setup() {
pinMode(11,OUTPUT);
}

void loop() {

digitalWrite(11,HIGH);
delay(8.33);
digitalWrite(11,LOW);
delay(8.33);

  
}
