# 3-movements-for-robot-arm
Programming 3 movements for robot arm using 6 servo motors

 ## Components
 - 6 servo motors
 - 1 Arduino Uno R3
 - Breadbaourd
 - 20 wires
 
 
 ## C++ Code 
  the code that used in the circuit is:
  ```javascript
// C++ code
//
#include <Servo.h>

int dgree = 0;

Servo servo_13;

Servo servo_12;

Servo servo_11;

Servo servo_10;

Servo servo_9;

Servo servo_8;

int counter;

int counter2;

void setup()
{
  servo_13.attach(13, 500, 2500);

  servo_12.attach(12, 500, 2500);

  servo_11.attach(11, 500, 2500);

  servo_10.attach(10, 500, 2500);

  servo_9.attach(9, 500, 2500);

  servo_8.attach(8, 500, 2500);

}

void loop()
{
  servo_13.read();

  servo_12.read();

  servo_11.read();

  servo_10.read();

  servo_9.read();

  servo_8.read();

  for (counter = 0; counter < 1; ++counter) {
    delay(1000); // Wait for 1000 millisecond(s)
    servo_12.write(60);
    servo_11.write(60);
    servo_10.write(60);
    servo_9.write(60);
    servo_8.write(60);
    servo_13.write(60);
  }
  delay(2000); // Wait for 2000 millisecond(s)
  servo_13.write(120);
  servo_12.write(120);
  servo_11.write(120);
  servo_10.write(120);
  servo_9.write(120);
  servo_8.write(120);
  for (counter2 = 0; counter2 < 1; ++counter2) {
    delay(1000); // Wait for 1000 millisecond(s)
    servo_13.write(180);
    servo_12.write(180);
    servo_11.write(180);
    servo_10.write(180);
    servo_9.write(180);
    servo_8.write(180);
  }
}

```
## Program
The program that used to do the circuit and the code is TINKERCAD.
