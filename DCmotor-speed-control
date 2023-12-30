// The Project OF The DC Motor Speed Control With POTENTIOMETER OR POT .

// In This Program, We Want To Show The DC Motor Speed Control With The POTENTIOMETER OR POT .

// The Main Code OF The Project OF The DC Motor Speed Control With POTENTIOMETER OR POT . . INO . .




int ENABLE = 10;                                                                                                                // Basic Definition : Number 10 . :
int IN1 = 9;                                                                                                                   // Basic Definition : Number 9 . :
int IN2 = 8;                                                                                                                  // Basic Definition : Number 8 . :
int PMWPIN = A0;                                                                                                             // Basic Definition : Number A0 . :
int C = 0;                                                                                                                  // Basic Definition : Number 0 . :


void setup () {
  
  pinMode (ENABLE , OUTPUT);                                                                                          // Introducing The OUTPUT Pin .
  pinMode (IN1 , OUTPUT);                                                                                            // Introducing The OUTPUT Pin .
  pinMode (IN2 , OUTPUT);                                                                                           // Introducing The OUTPUT Pin .
  pinMode (PMWPIN, INPUT);                                                                                         // Introducing The INPUT Pin .
  
}


void loop () {

  digitalWrite (IN1, HIGH);                                                                               // The Activation OF The IN1 OUTPUT .
  digitalWrite (IN2, LOW);                                                                               // The Inactivation OF The IN1 OUTPUT .
  C = analogRead (PMWPIN);
  C = map (C, 0, 1023, 0, 255);
  analogWrite (ENABLE, C);
  
}
