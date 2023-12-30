// The MQ — 9 Gas Sensor Measurement Project .

// In this program, We want to show The Measurement of The MQ — 9 Gas Sensor .

// The Main Code OF The MQ — 9 Gas Sensor Measurement Project . . INO . .




const int TheLED = 2;                                                                                                                           // The Basic Definition : The Number Is : 2 . :
const int TheDO = 8;                                                                                                                           // The Basic Definition : The Number Is : 8 . :




void setup () {

  Serial.begin (9600);                                                                                                                  // Init Serial At 9600 Baud Rate . OR . Introducing The Series .
  pinMode (TheLED , OUTPUT);                                                                                                           // The LED Pin Is OUTPUT . OR . Introducing The OUTPUT Pin .
  pinMode (TheDO , INPUT);                                                                                                            // The DO Pin Is INPUT . OR . Introducing The INPUT Pin .

}


void loop () {

  int TheAlarm = 0;
  float TheSensorVolt;
  float TheRSGas;
  float TheRatio;
                                                                                                                         . . // . . — Replace The Name " The R0 " With The Value OF The R0 IN The Demo OF First Test — . . // . .
  float TheR0 = 0.91;
 
  int TheSensorValue = analogRead (A0);
  TheSensorVolt = ( (float) TheSensorValue / 1024) * 5.0;
  TheRSGas = (5.0 - TheSensorVolt) / TheSensorVolt;                                                                     // Depend ON RL ON Your Module .


  TheRatio = TheRSGas / TheR0;                                                                                       // The Ratio = The RS / The R0 .


                                                                                                                  // ------------------------------------------------------------ //


  Serial.print (" * * * * The Sensor Volt = ! * * * * ");                                                      // Show The Desired Message .
  Serial.println (TheSensorVolt);                                                                             // Show The Desired Message .
  Serial.print (" * * * * The RS Ratio = ! * * * * ");                                                       // Show The Desired Message .
  Serial.println (TheRSGas);                                                                                // Show The Desired Message .
  Serial.print (" * * * * The RS / The R0 = ! * * * * ");                                                  // Show The Desired Message .
  Serial.println (TheRatio);                                                                              // Show The Desired Message .


  Serial.print (" * * * * \ The N \ The N * * * * ");                                                  // Show The Desired Message .


  TheAlarm = digitalRead (TheDO);
  if (TheAlarm == 1) digitalWrite (TheLED, HIGH);                                                  // Turn ON The LED .
  else if (TheAlarm == 0) digitalWrite (TheLED, LOW);                                             // Turn OFF The LED .


  delay (1000);                                                                                // Running The Delay Function (1 Second) . :


}
