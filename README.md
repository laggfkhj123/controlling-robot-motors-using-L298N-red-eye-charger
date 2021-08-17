# controlling-robot-motors-using-L298N-red-eye-charger
Controlling Robot Motors Using L298N
Used equipments
Arduino.
L298N Motor Driver.
2 motors.
11.1 V & 2200mAH Battery.
Implementation Steps
Connect the Arduino and L298N ports as following:

Arduino	L298N
13	Enaple A
12	IN1
11	IN2
10	IN3
9	IN4
8	Enaple b
Connect the two motors in L298N ports out1,out2,out3,out41.

Connect the LIPO battery in L298N.

The final step is Writing the code:

int Enable_button_1=13 ,Turn_right_1=12,Turn_left_1=11,Enable_button_2=10 ,Turn_right_2=9,Turn_left_2=8;
void setup() {
 pinMode(13,OUTPUT);
 pinMode(12,OUTPUT);
 pinMode(11,OUTPUT);
 pinMode(10,OUTPUT);
 pinMode(9,OUTPUT);
 pinMode(8,OUTPUT);
}

void loop() {

digitalWrite(Enable_button_1,HIGH);
digitalWrite(Turn_right_1,LOW);
digitalWrite(Turn_left_1,HIGH);


digitalWrite(Enable_button_2,HIGH);
digitalWrite(Turn_right_2,LOW);
digitalWrite(Turn_left_2,HIGH);

} 
