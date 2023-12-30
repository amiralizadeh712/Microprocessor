// The Infrared Sensor Project .

// In this program, We want to show that if a motion is detected by an Infrared Sensor, The LED is turned on and if The motion is not detected, The LED is turned off .

// The Main Code OF The Infrared Sensor Project . . INO . .




int TheInfraredSensor = 3;                                                                                               // Connect The Infrared Sensor Module To Arduino Pin D9 . OR . The Basic Definition : The Number Is : 3 . :
int TheLED = 13;                                                                                                        // Connect The LED To Arduino Pin 13 . OR . The Basic Definition : The Number Is : 13 . :




void setup () {

Serial.begin (115200);                                                                                          // Init Serial At 115200 Baud Rate . OR . Introducing The Series .
Serial.println (" * * * * The Serial Is Working ! * * * * " );                                                 // Test To Check If * * * * The Serial Is Working ! * * * * OR NOT . OR . Show The Desired Message .
pinMode (TheInfraredSensor , INPUT);                                                                          // The Infrared Sensor Pin Is INPUT . OR . Introducing The INPUT Pin .
pinMode (TheLED , OUTPUT);                                                                                   // The LED Pin Is OUTPUT . OR . Introducing The OUTPUT Pin .
 
}


void loop () {

  int TheSensorStatus = digitalRead (TheInfraredSensor);                                              // Set The GPIO As INPUT .


  if (TheSensorStatus == 1)                                                                        // Check If The Pin HIGH OR NOT .

  {                                                                                              // If The Pin Is HIGH Turn OFF The Onboard The LED .

    digitalWrite (TheLED, LOW);                                                                // Turn OFF The LED .
    Serial.println (" * * * * The Motion Detected ! * * * * ");                               // Print * * * * The Motion Detected ! * * * * ON The Serial Monitor Window . OR . Show The Desired Message .

  }


  else {                                                                                // Else Turn ON The Onboard The LED .

    digitalWrite (TheLED , HIGH);                                                     // Turn ON The LED .
    Serial.println (" * * * * The Motion Ended ! * * * * ");                         // Print * * * * The Motion Ended ! * * * * ON The Serial Monitor Window . OR . Show The Desired Message .

  }
  

}
