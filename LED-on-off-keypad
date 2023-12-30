// The Project OF Turning ON AND OFF The LED With The Help OF A Keypad .

// In this program, We want to turn on an LED when Code : One (1) comes in and turn off The LED when Code : Two (2) comes in .

// The Main Code OF The Project OF Turning ON AND OFF The LED With The Help OF A Keypad . . INO . .




#include <Keypad.h>                                                                                                                                                          // Library Required for this Project .


int LED = 12;
const byte ROWS = 4;                                                                                                                                                     // The four Rows .
const byte COLS = 4;                                                                                                                                                    // The Four Columns .


// Define The Symbols on The Buttons of The Keypads .


char HexaKeys [ROWS] [COLS] = {

    
  {'1','2','3','A'},
  {'4','5','6','B'},
  {'7','8','9','C'},
  {'*','0','#','D'}

  
};


byte RowPins [ROWS] = {9, 8, 7, 6};                                                                                                                    // Connect to The Row Pinouts of The Keypad .
byte ColPins [COLS] = {5, 4, 3, 2};                                                                                                                   // Connect to The Column Pinouts of The Keypad .


// Initialize an Instance of Class NewKeypad .


Keypad customKeypad = Keypad ( makeKeymap (hexaKeys), RowPins, ColPins, ROWS, COLS); 

void setup () {


  pinMode (LED, OUTPUT);                                                                                                                    // Introducing The OUTPUT pin .
  Serial.begin (9600);                                                                                                                     // Introducing The Series .


}


void loop () {


  int TheButton = int (customKeypad.getKey () ) -48;


  switch (TheButton) {


  case 1:
    digitalWrite (LED,HIGH);                                                                                                   // Turn on The LED .
    break;                                                                                                                    // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .
    
  case 2:
    digitalWrite (LED,LOW);                                                                                                // Turn off The LED .
    break;                                                                                                                // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .


  }


}
