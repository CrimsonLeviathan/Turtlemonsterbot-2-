#include <Servo.h>

Servo myservo;  // create servo object to control a servo
// twelve servo objects can be created on most boardsk

int pos = 0;    // variable to store the servo position

void setup() {
  myservo.attach(9);  // attaches the servo on pin 9 to the servo object
   pinMode(12, OUTPUT);
   pinMode(11,OUTPUT);
   }

void loop() {
  for (pos = 0; pos <= 70; pos += 3) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);
  // waits 15ms for the servo to reach the position
  }
  for (pos = 70; pos >= 0; pos -= 3) { // goes from 180 degrees to 0 degrees
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
  }
      digitalWrite(12,HIGH);
    digitalWrite(11,HIGH);
    delay(1000);
    digitalWrite(12,LOW);
    digitalWrite(11,LOW);
    delay(1000);
    digitalWrite(12,HIGH);
    delay(100);
    digitalWrite(11,HIGH);
    delay(1000);
    digitalWrite(12,LOW);
    digitalWrite(11,LOW);
    delay(100);
    {
  for (pos = 0; pos <= 70; pos += 3) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);
  // waits 15ms for the servo to reach the position
  }
  for (pos = 70; pos >= 0; pos -= 3)  // goes from 180 degrees to 0 degrees
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
    }
    digitalWrite(12,HIGH);
    digitalWrite(11,HIGH);
    delay(100);
    digitalWrite(12,LOW);
    digitalWrite(11,LOW);
    delay(100);
    digitalWrite(12,HIGH);
    digitalWrite(11,HIGH);
    delay(100);
    digitalWrite(12,LOW);
    digitalWrite(11,LOW);
    delay(1000);
  }
