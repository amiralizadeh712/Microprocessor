// The MQ — 9 Gas Sensor Calibration Project .

// In this program, We want to show The Calibration of The MQ — 9 Gas Sensor .

// The Main Code OF The MQ — 9 Gas Sensor Calibration Project . . INO . .




void setup () {

  Serial.begin (9600);                                                                                                                               // Init Serial At 9600 Baud Rate . OR . Introducing The Series .

}


void loop () {

  float TheSensorVolt;
  float TheRSAir;                                                                                                                            // The RS IN Clean Air .
  float TheR0;                                                                                                                              // The R0 IN 1000 PPM LPG .
  float TheSensorValue;


                                                                                                                                        // The Average .


    for (int x = 0 ; x < 100 ; x++)

  {

    TheSensorValue = TheSensorValue + analogRead (TheA0);

  }


  TheSensorValue = TheSensorValue / 100.0;


                                                                                                                      . . // . . ----------------------------------------------- . . // . .


  TheSensorVolt = (TheSensorValue / 1024) * 5.0;
  TheRSAir = (5.0 - TheSensorVolt) / TheSensorVolt;                                                                   // Depend ON RL ON Your Module .
  TheR0 = TheRSAir / 9.9;                                                                                            // According To The MQ — 9 Gas Sensor Datasheet Table .


  Serial.print (" * * * * The Sensor Volt = ! * * * * ");                                                        // Show The Desired Message .
  Serial.print (TheSensorVolt);                                                                                 // Show The Desired Message .
  Serial.println (" * * * * The V * * * * ");                                                                  // Show The Desired Message .


  Serial.print (" * * * * The R0 = ! * * * * ");                                                            // Show The Desired Message .
  Serial.println (TheR0);                                                                                  // Show The Desired Message .
  delay (1000);                                                                                           // Running The Delay Function (1 Second) . :


}
