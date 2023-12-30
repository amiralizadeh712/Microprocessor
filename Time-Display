// The Time Display Project .

// In this program, We want to Show Time .

// The Main Code OF The Time Display Project . . INO . .




#include <LiquidCrystal.h>                                                                                                                                            // Library required for this Project .


const int rs = 12, en = 11, d4 = 5, d5 = 4, d6 = 3, d7 = 2;                                                                                                        // Definition of Different Bases .
LiquidCrystal LCD (rs, en, d4, d5, d6, d7);                                                                                                                       // Definition of Different Bases .


unsigned long LastTime = 0;                                                                                                                                     // The Last Time In Milliseconds .
unsigned long InterVal = 1000;                                                                                                                                  // The Time Interval In Milliseconds . (1 Second Here . ) .


void setup ()

{
  
 LCD.begin (16, 2);                                                                                                                                       // Introducing LCD Resolution .
 
}


void loop ()

{
  
  unsigned long CurrentTime = millis ();                                                                                                             // The Current Amount OF Time .
  

  if (CurrentTime - LastTime >= InterVal)
  
  {
    
    LastTime = CurrentTime;                                                                                                                     // Updated The Last Time .
    int Seconds = (CurrentTime / 1000) % 60;                                                                                                   // Calculating Seconds .
    int Minutes = (CurrentTime / (1000 * 60) ) % 60;                                                                                          // Calculating Minutes .
    int Hours = (CurrentTime / (1000 * 60 * 60) ) % 24;                                                                                      // Calculating Hours .


    LCD.setCursor (0, 0);                                                                                                                  // To run regularly and display the OUTPUT below .


    if (Hours < 10)

    {
      
      LCD.print ('0');                                                                                                                // Show the Desired Message .
      
    }

    
    LCD.print (Hours);                                                                                                             // Show the Desired Message .
    LCD.print (':');                                                                                                              // Show the Desired Message .

    
    if (Minutes < 10)

    {

      LCD.print ('0')                                                                                                           // Show the Desired Message .

    }


    LCD.print (Minutes);                                                                                                     // Show the Desired Message .
    LCD.print (':');                                                                                                        // Show the Desired Message .


    if (Seconds < 10)
    
    {
      
      LCD.print ('0');                                                                                                // Show the Desired Message .
      
    }

    
    LCD.print (Seconds);                                                                                          // Show the Desired Message .
    
    
  }


}
