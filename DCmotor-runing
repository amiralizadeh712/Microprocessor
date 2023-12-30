// The Project OF Starting The DC Motor .

// In This Program, We Want To Show The DC Motor Launch .

// The Main Code OF The Project OF Starting The DC Motor . . INO . .




int ENABLE = 10;                                                                                                                                                         // Basic Definition : Number 10 . :
int IN1 = 9;                                                                                                                                                            // Basic Definition : Number 9 . :
int IN2 = 8;                                                                                                                                                           // Basic Definition : Number 8 . :


void setup () {

  pinMode (ENABLE, OUTPUT);                                                                                                                                       // Introducing The OUTPUT Pin .
  pinMode (IN1, OUTPUT);                                                                                                                                         // Introducing The OUTPUT Pin .
  pinMode (IN2, OUTPUT);                                                                                                                                        // Introducing The OUTPUT Pin .
  
}


void DemoONE ()

{

  digitalWrite (IN1, HIGH);                                                                                                                           // The Activation OF The IN1 OUTPUT .
  digitalWrite (IN2, LOW);                                                                                                                           // The Inactivation OF The IN2 OUTPUT .

  analogWrite (ENABLE, 200);

  delay (2000);                                                                                                                                 // Running The Delay Function (2 Seconds) . :

  digitalWrite (IN1, LOW);                                                                                                                    // The Inactivation OF The IN1 OUTPUT .
  digitalWrite (IN2, HIGH);                                                                                                                  // The Activation OF The IN2 OUTPUT .

  delay (2000);                                                                                                                            // Running The Delay Function (2 Seconds) . :

  digitalWrite (IN1, LOW);                                                                                                               // The Inactivation OF The IN1 OUTPUT .
  digitalWrite (IN2, LOW)                                                                                                               // The Inactivation OF The IN2 OUTPUT .

}


void DemoTwo ()

{


  digitalWrite (IN1, LOW);                                                                                                   // The Inactivation OF The IN1 OUTPUT .
  digitalWrite (IN2, HIGH);                                                                                                 // The Activation OF The IN2 OUTPUT .


  for (int i = 0; i < 256; i++)                                                                                          // The Determination OF The Acceleration From 0 To Maximum Speed .

  {

    analogWrite (ENABLE, i);
    delay (20);                                                                                                    // Running The Delay Function (0.02 Seconds) . :

  }


  for (int i = 255; i >= 0; --i)                                                                             // The Determination OF The Acceleration From Maximum Speed To 0

  {

    analogWrite (ENABLE, i);
    delay (20);                                                                                         // Running The Delay Function (0.02 Seconds) . :
    
  }


  digitalWrite (IN1, LOW);                                                                        // The Inactivation OF The IN1 OUTPUT .
  digitalWrite (IN2, LOW);                                                                       // The Inactivation OF The IN2 OUTPUT .


}


void loop () {

  DemoONE ();
  delay (1000);                                                                       // Running The Delay Function (1 Second) . :

  DemoTwo ();
  delay (1000);                                                                    // Running The Delay Function (1 Second) . :

}
