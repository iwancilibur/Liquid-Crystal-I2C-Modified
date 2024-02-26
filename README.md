# Installation #
Create a new folder called "LiquidCrystal_I2C" under the folder named "libraries" in your Arduino sketchbook folder.
Create the folder "libraries" in case it does not exist yet. Place all the files in the "LiquidCrystal_I2C" folder.

# Usage #
To use the library in your own sketch, select it from *Sketch > Import Library*.

-------------------------------------------------------------------------------------------------------------------
#include <LiquidCrystal_I2C.h>
#include <Wire.h>

LiquidCrystal_I2C lcd(0x27, 16, 2);

void setup() {
 Serial.begin(115200);
 lcd.begin();
}

void loop() { 
  lcd.clear();
  lcd.setCursor(0,0); lcd.print("HALLO ^_^");
  lcd.setCursor(0,1);lcd.print("IWAN CILIBUR");
  delay(1000);
  
  lcd.clear();
  lcd.setCursor(0,0); lcd.print("HALLO ^_^");
  lcd.setCursor(0,1);lcd.print("ROBOTIKA");
  delay(1000);
}
