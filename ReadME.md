
# 4 Digit 7 Segment LED Display

A Seven-segment display (SSD), or seven-segment indicator, is a form of electronic display device for displaying decimal numerals that is an alternative to the more complex dot matrix displays. Seven-segment displays are widely used in digital clocks, electronic meters, basic calculators, and other electronic devices that display numerical information.




## Components Used

### Hardware

1. Arduino UNO
2. 4 digit 7 Segment LED display
3. Wires & Breadboard
4. Power Supply 

### Software

1. VS Code (Arduino IDE Extension)

## Schematic 

<img src="https://firebasestorage.googleapis.com/v0/b/common-project-63634.appspot.com/o/4%20digit%207%20segment%20display%2Fschematic.jpg?alt=media&token=6ada8329-99b0-4071-a6da-773c97032268"></img>


## Code 

```javascript
/*
Author: Mohd Aman Ansari
embed
https://embed.org.in
===================================================================
Showing number 0-9 on a Common Anode 7-segment LED display
Displays the numbers 0-9 on the display, with one second inbetween.
    A
    ---
F |   | B
  | G |
   ---
E |   | C
  |   |
   ---
    D
   
 */
 
// Pin 2-8 is connected   to the 7 segments of the display.

int pinA = 2;
int pinB = 3;
int pinC   = 4;
int pinD = 5;
int pinE = 6;
int pinF = 7;
int pinG = 8;
int   D1 = 9;
int D2 = 10;
int D3 = 11;
int D4 = 12;

// the setup routine   runs once when you press reset:
void setup() {                
  // initialize   the digital pins as outputs.
  pinMode(pinA, OUTPUT);     
  pinMode(pinB,   OUTPUT);     
  pinMode(pinC, OUTPUT);     
  pinMode(pinD, OUTPUT);     
   pinMode(pinE, OUTPUT);     
  pinMode(pinF, OUTPUT);     
  pinMode(pinG,   OUTPUT);   
  pinMode(D1, OUTPUT);  
  pinMode(D2, OUTPUT);  
  pinMode(D3,   OUTPUT);  
  pinMode(D4, OUTPUT);  
}

// the loop routine runs over   and over again forever:
void loop() {
  digitalWrite(D1, HIGH);
  digitalWrite(D2,   LOW);
  digitalWrite(D3, LOW);
  digitalWrite(D4, LOW); 
  //0
  digitalWrite(pinA,   LOW);   
  digitalWrite(pinB, HIGH);   
  digitalWrite(pinC, LOW);   
   digitalWrite(pinD, LOW);   
  digitalWrite(pinE, HIGH);   
  digitalWrite(pinF,   LOW);   
  digitalWrite(pinG, LOW);   
  delay(1);               // wait for   a second
  
  digitalWrite(D1, LOW);
  digitalWrite(D2, HIGH);
  digitalWrite(D3,   LOW);
  digitalWrite(D4, LOW); 
  //1
  digitalWrite(pinA, LOW);   
   digitalWrite(pinB, LOW);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD,   HIGH);   
  digitalWrite(pinE, LOW);   
  digitalWrite(pinF, LOW);   
   digitalWrite(pinG, LOW);   
  delay(1);               // wait for a second
   
  digitalWrite(D1, LOW);
  digitalWrite(D2, LOW);
  digitalWrite(D3,   HIGH);
  digitalWrite(D4, LOW); 
  //2
  digitalWrite(pinA, HIGH);   
   digitalWrite(pinB, HIGH);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD,   HIGH);   
  digitalWrite(pinE, LOW);   
  digitalWrite(pinF, HIGH);   
   digitalWrite(pinG, LOW);     
  delay(1);               // wait for a second

   digitalWrite(D1, LOW);
  digitalWrite(D2, LOW);
  digitalWrite(D3, LOW);
   digitalWrite(D4, HIGH); 
  //3
  digitalWrite(pinA, LOW);   
  digitalWrite(pinB,   HIGH);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD, HIGH);   
   digitalWrite(pinE, LOW);   
  digitalWrite(pinF, LOW);   
  digitalWrite(pinG,   HIGH);     
  delay(1);               // wait for a second
/*  
  //4
   digitalWrite(pinA, HIGH);   
  digitalWrite(pinB, LOW);   
  digitalWrite(pinC,   LOW);   
  digitalWrite(pinD, HIGH);   
  digitalWrite(pinE, HIGH);   
   digitalWrite(pinF, LOW);   
  digitalWrite(pinG, LOW);     
  delay(1000);                // wait for a second
  
  //5
  digitalWrite(pinA, LOW);    
  digitalWrite(pinB, HIGH);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD,   LOW);   
  digitalWrite(pinE, HIGH);   
  digitalWrite(pinF, LOW);   
   digitalWrite(pinG, LOW);     
  delay(1000);               // wait for a second
   
  //6
  digitalWrite(pinA, LOW);   
  digitalWrite(pinB, HIGH);   
   digitalWrite(pinC, LOW);   
  digitalWrite(pinD, LOW);   
  digitalWrite(pinE,   LOW);   
  digitalWrite(pinF, LOW);   
  digitalWrite(pinG, LOW);     
   delay(1000);               // wait for a second
  
  //7
  digitalWrite(pinA,   LOW);   
  digitalWrite(pinB, LOW);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD,   HIGH);   
  digitalWrite(pinE, HIGH);   
  digitalWrite(pinF, HIGH);   
   digitalWrite(pinG, HIGH);     
  delay(1000);               // wait for a second
   
  //8
  digitalWrite(pinA, LOW);   
  digitalWrite(pinB, LOW);   
   digitalWrite(pinC, LOW);   
  digitalWrite(pinD, LOW);   
  digitalWrite(pinE,   LOW);   
  digitalWrite(pinF, LOW);   
  digitalWrite(pinG, LOW);     
   delay(1000);               // wait for a second

  //9
  digitalWrite(pinA,   LOW);   
  digitalWrite(pinB, LOW);   
  digitalWrite(pinC, LOW);   
  digitalWrite(pinD,   HIGH);   
  digitalWrite(pinE, HIGH);   
  digitalWrite(pinF, LOW);   
   digitalWrite(pinG, LOW);     
  delay(1000);               // wait for a second
   */
}
