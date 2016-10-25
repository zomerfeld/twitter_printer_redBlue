
#include "Adafruit_Thermal/Adafruit_Thermal.h"

Adafruit_Thermal printer;

// String tweet;
char tweet[300];
String oldTweet;


void setup(){
  Serial.begin(9600); // Uses regular serial
  Serial1.begin(19200); //Starts printer serial (RX (green printer wire), TX (yellow printer wire)
  printer.begin(&Serial1); //uses RX and TX
  Particle.subscribe("TrumpTweet", myHandler); //subscribes to the event

  //Particle.subscribe("weathertoday", printWeather);
  

   printer.println(tweet);
   printer.feed(1);


 }


void loop() {
//empty   
}
    
    
void myHandler(String event, String data) { //this triggers from bluetweet)
  /* Particle.subscribe handlers are void functions, which means they don't return anything.
  They take two variables-- the name of your event, and any data that goes along with your event.
  In this case, the event will be "buddy_unique_event_name" and the data will be "intact" or "broken"

  Since the input here is a char, we can't do
     data=="intact"
    or
     data=="broken"

  chars just don't play that way. Instead we're going to strcmp(), which compares two chars.
  If they are the same, strcmp will return 0.
  */
  Particle.publish("myhandlerBlue Triggered", "YES"); //Debug - let me know it was triggered

  int result = data.compareTo(oldTweet); //compares to old tweet
  if (result == 0) { 
    Particle.publish("Blue_the_same", "Samesies");
    } else {
    // if the data is something else
      printReal(data); //sends this to the printing function
      oldTweet = String(data); //saves this tweet in oldTweet
      Particle.publish("Blue_the_same", "Not The Same"); //publish a message
  }
}
    
    void printReal(String thing) { //the printer function
        printer.wake();
        printer.boldOn();
        Particle.publish("thing_I_printed_blue", thing);
        printer.println(thing);
        printer.feed(8); //8 lines are enough to clear the opening
        printer.sleep();

    }

void print2(String event, String data) { 
    printer.wake();
    printer.inverseOn();
    printer.println(data);
    printer.inverseOff();
    printer.feed(8);
    printer.sleep();
    Particle.publish("thing_I_printed_blue", data);

}


    
