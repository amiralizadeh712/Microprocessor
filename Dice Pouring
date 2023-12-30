// The Dice Pouring Project .

// In this program, We want to Display Numbers Randomly .

// The Main Code OF The Dice Pouring Project . . INO . .




#include "SevSeg.h"                                                                                                                                                     // Library required for this Project .


SevSeg sevseg;                                                                                                                                                        // Instantiate a seven segment controller object .
const int ButtonPin = 10;
int ButtonState = 0;


void setup ()

{

byte NumDigits = 1;
byte DigitPins [] = {};
byte SegmentPins [] = {3, 2, 8, 7, 6, 4, 5, 9};
bool ResistorsONSegments = true;                                                                                                                             // ' False ' Means Resistors Are ON Digit Pins .
sevseg.begin (COMMON_ANODE, NumDigits, DigitPins, SegmentPins, ResistorsONSegments);
sevseg.setBrightness (90);
pinMode (ButtonPin, INPUT);                                                                                                                               // Introducing The INPUT Pin .

}


void loop ()

{

  ButtonState = digitalRead (ButtonPin);


  if (ButtonState == HIGH)

  {

    sevseg.setNumber (random (1, 7) );
    sevseg.refreshDisplay ();

  }

  
}
