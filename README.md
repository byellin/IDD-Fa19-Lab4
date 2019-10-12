# Paper Puppets

*A lab report by John Q. Student*

## In this Report

To submit your lab, clone [this repository](https://github.com/FAR-Lab/IDD-Fa18-Lab4). You'll need to describe your design, include a video of your paper display in operation, and upload any code you wrote to make it move.

## Part A. Actuating DC motors

**Link to a video of your vibration motor**

![DC Motor Video](https://github.com/byellin/IDD-Fa19-Lab4/blob/master/Vibration%20Motor.MOV)

## Part B. Actuating Servo motors

### Part 1. Connect the Servo to your breadboard

**a. Which color wires correspond to power, ground and signal?**

Red is power.
Purple is ground.
Orange is signal.

### Part 2. Connect the Servo to your Arduino

**a. Which Arduino pin should the signal line of the servo be attached to?**

The signal line of the servo is attached to pin 9 on the Arduino. 

**b. What aspects of the Servo code control angle or speed?**

This loop controls the angle of the servo motor. The increment position controls the speed of the motor. 

void loop() {
  for (pos = 0; pos <= 180; pos += 1) { // goes from 0 degrees to 180 degrees
    // in steps of 1 degree
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
  }
  for (pos = 180; pos >= 0; pos -= 1) { // goes from 180 degrees to 0 degrees
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
  }
}

## Part C. Integrating input and output

**Include a photo/movie of your raw circuit in action.**

https://github.com/byellin/IDD-Fa19-Lab4/blob/master/IMG_7247.JPG

## Part D. Paper puppet

**a. Make a video of your proto puppet.**

![Prototype of Puppet](https://github.com/byellin/IDD-Fa19-Lab4/blob/master/Puppet%20in%20Action.MOV)

## Part E. Make it your own

**a. Make a video of your final design.**

![Final Design](https://github.com/byellin/IDD-Fa19-Lab4/blob/master/Make%20it%20Your%20Own.MOV)
 
