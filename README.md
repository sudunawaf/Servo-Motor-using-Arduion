# Servo-Motor-using-Arduion
#include <Servo.h>

Servo myservo;  
int pos = 0;    
now attach the servo on pin 11 to the servo object

void setup() {

  myservo.attach(11);  

}
we are going to use for loop to goes from 0 degrees to 180 degrees, by using "Write" we tell servo to go to position in variable 'pos'. using "delay" to waits 10ms for the servo to reach the position.

void loop() {

  for (pos = 0; pos <= 180; pos += 1) { 

    myservo.write(pos);              
    delay(10);                      
  }
using for loop to move from 180 degrees to 0 degrees, tell servo to go to position in variable 'pos'. waits 10ms for the servo to reach the position

for (pos = 180; pos >= 0; pos -= 1) { 
myservo.write(pos);              
delay(10);                       // waits 15ms for the servo to reach the position

}

}
