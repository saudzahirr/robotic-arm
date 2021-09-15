

**Robotic Arm**

**Group Members:**

\1) Ch. Muhammad Shaheer Yasir. (CMS: 286021)

\2) Muhammad Saud Zahir.

\3) Muhammad Hamza.

(CMS: 294897)

(CMS: 290951)

**Introduction:**

A **Robotic arm** is a type of mechanical arm, usually programmable, with

similar functions to a human arm; the arm may be the sum total of the

mechanism or may be part of a more complex robot. The links of such a

manipulator are connected by joints allowing either rotational motion (such as

in an articulated robot) or translational (linear) displacement. They are mainly

used for **pick and place work**, application of sealant, assembly operations,

handling machine tools and arc welding. In this project we have used four

**Servo Motors** to show the movement of a robotic arm.

**Design Steps and Circuit Explanation:**

Our project consists of 3 main parts:

\1) Servo Motors (Robotic Arms).

\2) LCD for displaying the movement of Arms.

\3. Keypad for movement of Arms.





**Procedure:**

• Firstly, we started our working on the servo motor motion to explain the

movement of arms in different directions (like anti-clockwise for

upward).

• Then we moved to Keypad control for our servo motors.

• And lastly, we designed LCD interfacing for our locomotion and

movement units of arms.

**Explanation.**

**Design:**

\1) LCD LM016L.

\2) Potentiometer.

\3) Atmel 89C51.

\4) Keypad.

\5) Servo Motors.

\6) ULN2003A (7-Darlington Pairs).

\7) Quartz Crystal, Logic Probe and Push Button.

\8) Resistors (100 and 8.2kΩ) and Capacitors (1nF).

\9) Electrolytic Capacitor (10u, 16V, 30mA).





Our Robotic Arm model uses 3 **Atmel 89C51 Micro-controllers**, for Keypad,

LCD and Servo Motors, respectively. The basic principle of our project is that it

takes input from the keypad and the number of distance units to be moved.

Every key on **Keypad** defines a movement.

1 (UPWARD)

4 (REVERSE)

7 (GRIP CLOSE)

2 (DOWNWARD)

5 (LEFT)

8 (GRIP OPEN)

3 (FORWARD)

6 (RIGHT)

9 (STOP)

For instance, if ‘1’ is pressed the LCD displays ‘UPWARD.’

Then the user inputs the number of distance units required for

locomotion. Furthermore, for two axial motions (UPWARD &

DOWNWARD) one servo motor is used. When the arm is **moving**

**upward** the motor is **rotating anti-clockwise**. In reality, a robotic arm

uses gears to do locomotion. So, we have used this principle to show the

movement of arms (by the rotation of servo motors).

**Servo Motor 1.**

UPWARD:

FORWARD:

LEFT:

Anti-clockwise. DOWNWARD: Clockwise.

**Servo Motor 2.**

Anti-clockwise. REVERSE:

Clockwise.

Clockwise.

**Servo Motor 3.**

Anti-clockwise.

**Servo Motor 4.**

GRIP CLOSE: Anti-clockwise. GRIP OPEN: Clockwise.

RIGHT:





The **distance units** in our project is kept equal to the number of rotation

of servo motor.

So, if we have to move our arm about 10 units upward, the servo motor 1

will rotate anti-clockwise 10 times. The coding is done in Embedded C

using “reg51.h” library. The anti-clockwise and clockwise movement of

servo motors is created by using bits.

For example:

data1[] = {0000 0001, 0000 0010, 0000 0100, 0000 1000}

rotates servo motors anti-clockwise.

While,

data2[] = {0000 1000, 0000 0100, 0000 0010, 0000 0001}

rotates servo motors clockwise.

We have used **ULN2003A** (7-Darlington Pairs) before servo motors.

Typical usage of the ULN2003A is in driver circuits for relays, lamp and

LED displays, stepper motors, logic buffers and line drivers. We have

used this 16-pin IC to amplify the current from Atmel 89C51.

If we want to stop the motion of arm (servo motor) immediately the LCD

will display “**PRESS 9 TO STOP**”.





**Results and Achievements:**

**Problems Faced:**

• The Servo Motor did not stop after one complete cycle.

**Results Achieved:**

We have successfully created Robotic Arm using Atmel 89C51. The Servo

Motors work properly and show the locomotion as displayed on LCD.

**Recommended Future Work:**

The things that could have been added were:

• Using the cartesian coordinates (x, y, z) input from user to define the

locomotion of Robotic Arm.

• Saving the movement and the automatic locomotion.

