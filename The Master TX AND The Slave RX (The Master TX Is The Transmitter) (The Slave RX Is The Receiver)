// The Project OF The Master TX , AND & The Slave RX (The Master TX Is The Transmitter) (The Slave RX Is The Receiver) (The Slave RX Code) .

// In this program, We want to show that we send and display messages .

// The Main Code OF The Project OF The Master TX , AND & The Slave RX (The Master TX Is The Transmitter) (The Slave RX Is The Receiver) (The Slave RX Code) . . INO . .




#include <Wire.h>                                                                                                // Library Required For This Project .




void setup () {


  Wire.begin (2);                                                                                      // This Function Starts The Wire Library , AND & Adds The Module As Master OR Slave To The I2C Bass .
  Wire.onReceive (receiveEvent);                                                                      // By Using This Function, We Store The Received Data OR Message .
  Serial.begin (9600);                                                                               // Introducing The Series . OR Start Serial For OUTPUT .

}


void loop () {

  delay (250);                                                                               // Running The Delay Function (0.25 Seconds) . :

}


void receiveEvent (int HowMany)

{


  while (Wire.available () > 1)                                                // The Slave May Send Less Than Requested .

  {

    char C = Wire.read ();                                                // Receive A Byte As Character .
    Serial.print (C);                                                    // Print The Character .

  }


}
