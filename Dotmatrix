// The Dot Matrix Test Project .

// In This Program, We Want To Test The Dot Matrix .

// The Main Code OF The The Dot Matrix Test Project . . INO . .




#include <MaxMatrix.h>                                                                                                     // Library Required For This Project .


int DIN = 7;                                                                                                            // Basic Definition : Number 7 . :
int CLK = 6;                                                                                                           // Basic Definition : Number 6 . :
int CS = 5;                                                                                                           // Basic Definition : Number 5 . :
int MAXINUSE = 1;                                                                                                    // Basic Definition : Number 1 . :


byte buffer [20];
char Text [] = "A";


MaxMatrix M (DIN ,CS, CLK, MAXINUSE);


void setup () {

  M.init ();                                                                                                // Starting The Dot Matrix .
  M.setIntensity (8);                                                                                      // Determining LEDs Light Intensity (0 To 15) . :
  
}


void loop () {

  M.setDot (0, 7, true);                                                                          // Turning ON The LED IN (0 , 7) Cordinate .
  delay (1000);                                                                                  // Running The Delay Function (1 Second) . :

  M.setDot (7, 0, true);                                                                       // Turning ON The LED IN (7 , 0) Cordinate .
  delay (1000);                                                                               // Running The Delay Function (1 Second) . :

  M.setColumn (3, B11110000);                                                               // Turning ON A Group OF LEDs IN 3 Column .
  delay (1000);                                                                            // Running The Delay Function (1 Second) . :

  M.setColumn (4, B00001111);                                                            // Turning ON A Group OF LEDs IN 4 Column .
  delay (1000);                                                                         // Running The Delay Function (1 Second) . :

  M.clear ();                                                                         // Clear The Screen .
  delay (1000);                                                                      // Running The Delay Function (1 Second) . :
  
}
