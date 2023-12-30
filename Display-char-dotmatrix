// The Project OF The Display OF The Specific Character ON The Dot Matrix .

// In This Program, We Want To Display The Specific Character ON The Dot Matrix .

// The Main Code OF The Project OF The Display OF The Specific Character ON The Dot Matrix . . INO . .




#include <MaxMatrix.h>                                                                                                                              // Library Required For This Project .


int DIN = 7;                                                                                                                                     // Basic Definition : Number 7 . :
int CLK = 6;                                                                                                                                    // Basic Definition : Number 6 . :
int CS = 5;                                                                                                                                    // Basic Definition : Number 5 . :
int MAXINUSE = 1;                                                                                                                             // Basic Definition : Number 1 . :


MaxMatrix M (DIN ,CS, CLK, MAXINUSE);


byte ThePoker [] = {8, 8,

                     0xff,
                     0x81,
                     0xa5,
                     0xa1,
                     0xa1,
                     0xa5,
                     0x81,
                     0xff,

                    };


byte TheSmile [] = {8, 8,

                     0xff,
                     0x81,
                     0xb5,
                     0xa1,
                     0xa1,
                     0xb5,
                     0x81,
                     0xff,

                    };


byte TheSad [] = {8, 8,

                   0xff,
                   0x81,
                   0xb5,
                   0x91,
                   0x91,
                   0xb5,
                   0x81,
                   0xff,

                  };


byte TheKiss [] = {8, 8,

                    0xff,
                    0x81,
                    0xb5,
                    0xb1,
                    0xb1,
                    0xb5,
                    0x81,
                    0xff,

                   };


void setup () {

  M.init ();                                                                                           // Starting The Dot Matrix .
  M.setIntensity (8);                                                                                 // Determining LEDs Light Intensity (0 To 15) . :
  
}


void loop () {

  M.writeSprite (0, 0, TheSmile);                                                             // Displaying A Specific Character With The Start Points 0 , AND & 0 . :
  delay (1000);                                                                              // Running The Delay Function (1 Second) . :
  M.clear ();                                                                               // Clear The Screen .

  M.writeSprite (0, 0, ThePoker);                                                         // Displaying A Specific Character With The Start Points 0 , AND & 0 . :
  delay (1000);                                                                          // Running The Delay Function (1 Second) . :
  M.clear ();                                                                           // Clear The Screen .

  M.writeSprite (0, 0, TheSad);                                                       // Displaying A Specific Character With The Start Points 0 , AND & 0 . :
  delay (1000);                                                                      // Running The Delay Function (1 Second) . :
  M.clear ();                                                                       // Clear The Screen .

  M.writeSprite (0, 0, TheKiss);                                                  // Displaying A Specific Character With The Start Points 0 , AND & 0 . :
  delay (1000);                                                                  // Running The Delay Function (1 Second) . :


  for (int i = 0; i < 8; i++) {
    M.shiftLeft (false, false);
    delay (300);                                                           // Running The Delay Function (0.3 Seconds) . :


  }


  M.clear ();                                                       // Clear The Screen .


}
