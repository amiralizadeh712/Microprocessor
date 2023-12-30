// The Project OF The Calculator , With The Help OF A Keypad .

// In this program, We want to Show, How The Calculator, is Built with The Help of a Keypad .

// The Main Code OF The Project OF The Calculator , With The Help OF A Keypad . . INO . .




  # include <Keypad.h>                                                                                                                                                                 // Library Required for this Project .
  const byte ROWS = 4;                                                                                                                                                                // The Four Rows .
  const byte COLS = 4;                                                                                                                                                               // The Four Columns .

  float TheFirstNumber = 0;                                                                                                                                                        // Basic Definition : Number : 0 . :
  float TheSecondNumber = 0;                                                                                                                                                      // Basic Definition : Number : 0 . :
  float TheResult = 0;                                                                                                                                                           // Basic Definition : Number : 0 . :
  bool TheSection = false;
  int TheType = 0;                                                                                                                                                             // Basic Definition : Number : 0 . :

  char HexaKeys [ROWS] [COLS] = {

    
  {'1','2','3','A'},
  {'4','5','6','B'},
  {'7','8','9','C'},
  {'*','0','#','D'}

  
};


byte RowPins [ROWS] = {9, 8, 7, 6};                                                                                                                                   // Connect to The Row Pinouts of The Keypad .
byte ColPins [COLS] = {5, 4, 3, 2};                                                                                                                                  // Connect to The Column Pinouts of The Keypad .

Keypad CustomKeypad = Keypad (makeKeymap (HexaKeys), RowPins, ColPins, ROWS, COLS); 

void setup () {

  
Serial.begin (9600);                                                                                                                                             // Introducing the Series .

 
}


void loop () {


int TheButton = int (CustomKeypad.getKey () ) -48;


if (0 <= TheButton && TheButton <= 10) {

  Serial.print (TheButton);                                                                                                                            // Show The Desired Message .

  if (TheSection == false) {


    TheFirstNumber = TheFirstNumber * 10 + TheButton;


    }


    else {


      TheSecondNumber = TheSecondNumber * 10 + TheButton;


      }


  } else {


    switch (TheButton) {


        case 17:

        TheSection = true;
        TheType = 1;
        Serial.print (' + ');                                                                                                                              // Show The Desired Message .
        break;                                                                                                                                            // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .

        case 18:

        TheSection = true;
        TheType = 2;
        Serial.print (' - ');                                                                                                                       // Show The Desired Message .
        break;                                                                                                                                     // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .

        case 19:
         TheSection = true;
         TheType = 3;
         Serial.print (' * ');                                                                                                                // Show The Desired Message .
         break;                                                                                                                              // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .

         case 20:

          TheSection = true;
          TheType = 4;
          Serial.print (' / ');                                                                                                          // Show The Desired Message .
          break;                                                                                                                        // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .

         case -6:

          TheSection = false;
          TheType = 0;
          Serial.print ('  ');                                                                                                     // Show The Desired Message .
          break;                                                                                                                 // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .

         case -13:
          Serial.print (' = ');                                                                                              // Show The Desired Message .


          switch (TheType) {


            case 1:
              TheResult = (TheFirstNumber + TheSecondNumber);
              break;                                                                                         // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .
            case 2:
              TheResult = (TheFirstNumber - TheSecondNumber);
              break;                                                                                      // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .
            case 3:
              TheResult = (TheFirstNumber * TheSecondNumber);
              break;                                                                                    // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .
            case 4:
              TheResult = (TheFirstNumber / TheSecondNumber);
              break;                                                                                  // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .


      }


      TheType = 0;
      Serial.println (TheResult);                                                                // Show The Desired Message .
      TheFirstNumber = 0;
      TheSecondNumber = 0;
      TheSection = false;
      break;                                                                                 // Break is used to Exit from a for, While or Do…​While Loop, Bypassing the Normal Loop Condition. It is also used to Exit from a Switch Case Statement .


    }


  }


}
