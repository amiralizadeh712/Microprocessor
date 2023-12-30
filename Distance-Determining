// The Project OF Determining The Distance OF Objects By Utilizing The Ultrasonic Module .

// In this program, We want to determine the distance of the Objects by utilizing the Ultrasonic Module and then display it on the LCD Screen .

// The Main Code OF The Project OF Determining The Distance OF Objects By Utilizing The Ultrasonic Module . . INO . .




#include <LiquidCrystal.h>                                                                                                              // Library Required for this Project.
const int rs = 12, en = 11, d4 = 5, d5 = 4, d6 = 3, d7 = 2;                                                                            // Definition of Different Bases .
int Time, Distance, Trigger = 9, Echo = 10;                                                                                           // Basic Definition : Numbers 9 , and 10 . :
LiquidCrystal LCD (rs, en, d4, d5, d6, d7);                                                                                          // Definition of Different Bases .


void setup () {


  pinMode (Trigger, OUTPUT);                                                                                                   // Introducing The OUTPUT Pin .
  pinMode (Echo, INPUT);                                                                                                      // Introducing The INPUT Pin .
  Serial.begin (9600);                                                                                                       // Introducing The Series .
  LCD.begin (16, 2);                                                                                                        // Introducing LCD Resolution .


}


void loop () {


  digitalWrite (Trigger, LOW);
  delayMicroseconds (2);                                                                                           // Running The Delay Function (2 Microseconds) . :
  digitalWrite (Trigger, HIGH);
  delayMicroseconds (10);                                                                                        // Running The Delay Function (10 Microseconds) . :
  digitalWrite (Trigger, LOW);
  Time = pulseIn (Echo, HIGH);
  Distance = Time * 0.034 / 2;                                                                                // Set Value to Distance.
  Serial.print (" Distance : ");                                                                             // Show The Desired Message .
  Serial.println (Distance);                                                                                // Show The Desired Message .
  LCD.setCursor (0, 0);                                                                                    // To run Regularly and Display The OUTPUT Below .
  LCD.print (" Distance : ");                                                                             // Show The Desired Message .
  LCD.print (Distance);                                                                                  // Show The Desired Message .


}
