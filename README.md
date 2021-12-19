
# Kerala-IoT-Challenge

Foxlab Makerspace in association with GTech - Group of Technology Companies in Kerala is launching our prestigious program “Kerala IoT Challenge 2021”, with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. Kerala IoT Challenge is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.



## About Me
Hi everyone! I’m Richin, 3'rd year Electronics and Communication student from Sahrdaya college of engineering and technology,Kodakara.I’m here to get more exposure about the IoT world.And I also interested in Ethical hacking.
# Experiment 1 - Hello World LED Blinking
A basic Program similar to printing "Hello World " in any programming language. The Aim is to blink an LED using Arduino Uno Board.

Arduino Uno is an open-source microcontroller board developed by Arduino.cc. It has several advantages over the conventional microcontrollers. It comes with a pre-tested software and hardware libraries and has its own integrated development environment (IDE). Also it is less expensive & beginner friendly.

## Components Used

- Arduino Uno Board
- USB Cable
- LED (Any Color) x 1 Nos
- 220 OHM Resistor X 1 Nos
- Breadboard
- Jumper Wires (Male to Male ) X 2 Nos


## Circuit Diagram
![KL_IOT_EXP1(#)](https://user-images.githubusercontent.com/57257722/146680083-faabe266-4cc2-4637-8086-817f049a45f4.png)
## Code

Experiment 1 Code

```bash
  
int ledPin = 10; // define digital pin 10.
void setup()
{
pinMode(ledPin, OUTPUT);// define pin with LED connected as output.
}
void loop()
{
digitalWrite(ledPin, HIGH); // set the LED on.
delay(1000); // wait for a second.
digitalWrite(ledPin, LOW); // set the LED off.
delay(1000); // wait for a second
}

```
    
## Output

![KL_IOT_EXP1(2)](https://user-images.githubusercontent.com/57257722/146680038-8110fce6-607d-47fc-8482-1a0b1a9bb414.jpeg)
![KL_IOT_EXP1(1)](https://user-images.githubusercontent.com/57257722/146680046-cfaa3bfb-7ad0-4c77-81f0-4df0e469665b.jpeg)





## About Me
Hi everyone! I’m Richin, 3'rd year Electronics and Communication student from Sahrdaya college of engineering and technology,Kodakara.I’m here to get more exposure about the IoT world.And I also interested in Ethical hacking.
# Experiment 1 - Hello World LED Blinking
A basic Program similar to printing "Hello World " in any programming language. The Aim is to blink an LED using Arduino Uno Board.

Arduino Uno is an open-source microcontroller board developed by Arduino.cc. It has several advantages over the conventional microcontrollers. It comes with a pre-tested software and hardware libraries and has its own integrated development environment (IDE). Also it is less expensive & beginner friendly.

# Experiment 2 : Traffic Light
In the previous program, we have done the LED blinking experiment with one LED. Now, it’s time to up the stakes and do a bit more complicated experiment-traffic lights. Actually, these two experiments are similar. While in this traffic lights experiment, we use 3 LEDs with different colors rather than 1 LED.
## Components Required
- Arduino board *1
- USB cable *1
- Red M5 LED*1
- Yellow M5 LED*1
- Green M5 LED*1
- 220Ω resistor *3
## Circuit Diagram

![KL_IOT_EXP2(#)](https://user-images.githubusercontent.com/57257722/146680396-5d616c0a-4fbb-4e96-8170-069659e3755d.png)

## Code

```bash
int redled =10; // initialize digital pin 10.
int yellowled =7; // initialize digital pin 7.
int greenled =4; // initialize digital pin 4.
void setup()
{
pinMode(redled, OUTPUT);// set the pin with red LED as “output”
pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”
pinMode(greenled, OUTPUT); // set the pin with green LED as “output”
}
void loop()
{
digitalWrite(greenled, HIGH);//// turn on green LED
delay(5000);// wait 5 seconds
digitalWrite(greenled, LOW); // turn off green LED
for(int i=0;i<3;i++)// blinks for 3 times
{
delay(500);// wait 0.5 second
digitalWrite(yellowled, HIGH);// turn on yellow LED
delay(500);// wait 0.5 second
digitalWrite(yellowled, LOW);// turn off yellow LED
} 
delay(500);// wait 0.5 second
digitalWrite(redled, HIGH);// turn on red LED
delay(5000);// wait 5 seconds
digitalWrite(redled, LOW);// turn off red LED
}

```
## Output

In Traffic light the green LED blink about 5 second, then it is turnoff. Then the yellow LED blinks 3 times with a time interval of 0.5 second.Then the red LED blink about 5 seconds. This process continues
![KL_IOT_EXP2(1)](https://user-images.githubusercontent.com/57257722/146680543-ac23e8d6-4651-4f23-9204-1261cd43fb41.png)
![KL_IOT_EXP2(2)](https://user-images.githubusercontent.com/57257722/146680560-ee2a7d92-8dd3-402c-84a6-44572d8d2e11.png)

# Experiment 3 : LED Chasing Effect
We often see billboards composed of colorful LEDs. They are constantly changing to form various light effects. In this experiment, we compile a program to simulate LED chasing effect. The long lead of LED is the positive side; short lead is negative.
## Components Required

- Led *6
- Arduino board *1
- 220Ω resistor *6
- Breadboard *1
- USB cable*1
- Breadboard wire *13
## Circuit Diagram
![KL_IOT_EXP3(#)](https://user-images.githubusercontent.com/57257722/146680640-9516f09b-3cdf-4708-b6da-8a1bd76fa21d.jpeg)
## Code

```bash
int BASE = 2 ;  // the I/O pin for the first LED
int NUM = 6;   // number of LEDs
void setup()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     pinMode(i, OUTPUT);   // set I/O pins as output
   }
}
void loop()
{
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
     delay(200);        // delay
   }
   for (int i = BASE; i < BASE + NUM; i ++) 
   {
     digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
     delay(400);        // delay
   }  
}

```
## Output
![KL_IOT_EXP3(1)](https://user-images.githubusercontent.com/57257722/146680752-1758595a-279c-486f-8048-4e534f01f767.png)

![KL_IOT_EXP3(2)](https://user-images.githubusercontent.com/57257722/146680786-9434c6ec-2a11-4837-b85c-2bb590cc87a4.png)

