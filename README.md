# Herman-sedar-
Arduino coding 
const int buttonPin = 2;
const int ledPin = 13;  // Built-in LED

void setup() {
  pinMode(buttonPin, INPUT_PULLUP);  // Activate internal pull-up
  pinMode(ledPin, OUTPUT);
}

void loop() {
  int buttonState = digitalRead(buttonPin);

  if (buttonState == LOW) {  // LOW means pressed
    digitalWrite(ledPin, HIGH);
  } else {
    digitalWrite(ledPin, LOW);
  }
}
