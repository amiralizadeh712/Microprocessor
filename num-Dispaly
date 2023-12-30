// The Numbers Display Project .

// In this program, We want to Display Numbers .

// The Main Code OF The Numbers Display Project . . INO . .




#include "SevSeg.h"                                                                                                                                                          // Library required for this Project .


void setup ()

{

byte NumDigits = 1;
byte DigitPins [] = {};
byte SegmentPins [] = {3, 2, 8, 7, 6, 4, 5, 9};
bool ResistorsONSegments = true;                                                                                                                                      // ' False ' Means Resistors Are ON Digit Pins .
sevseg.begin (COMMON_ANODE, NumDigits, DigitPins, SegmentPins, ResistorsONSegments);
sevseg.setBrightness (90);

}


void loop ()

{

  for (int i = 0; i < 10; i++)

  {

    sevseg.setNumber (i);
    sevseg.refreshDisplay ();
    delay (2000);                                                                                                                                             // Running the Delay Function (2 Seconds) . :

  }

  
}
