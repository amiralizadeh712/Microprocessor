// The Project OF The Master TX , AND & The Slave RX (The Master TX Is The Transmitter) (The Slave RX Is The Receiver) (The Master TX Code) .

// In this program, We want to show that we send and display messages .

// The Main Code OF The Project OF The Master TX , AND & The Slave RX (The Master TX Is The Transmitter) (The Slave RX Is The Receiver) (The Master TX Code) . . INO . .




#include <Wire.h>                                                                                                     // Library Required For This Project .




void setup () {

  Wire.begin ();                                                                                             // This Function Starts The Wire Library , AND & Adds The Module As Master OR Slave To The I2C Bass . OR Join I2C Bus (Address Is Optional For Controller Device) .

}


short Age = 0;


void loop () {

  Wire.beginTransmission (2);                                                                    // This Function Is Used To Start Communicating With The Address-Containing Slave .
  Wire.write (" Age Is = ");                                                                    // This Function Is Used To Send The Desired Data OR Message To The Slave .
  Wire.write (Age);                                                                            // This Function Is Used To Send The Desired Data OR Message To The Slave .
  Wire.endTransmission ();                                                                    // This Function Is Used To Finish Communicating .
  delay (1000);                                                                              // Running The Delay Function (1 Second) . :

}
