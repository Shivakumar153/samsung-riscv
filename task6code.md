
#include <Arduino.h>

#define TRIG_PIN PD2  
#define ECHO_PIN PD5  
#define LED_PIN  PD6  

void setup() {
    pinMode(TRIG_PIN, OUTPUT);
    pinMode(ECHO_PIN, INPUT);
    pinMode(LED_PIN, OUTPUT);
}

void loop() {
    uint16_t duration;
    int distance;

    // Send trigger pulse
    digitalWrite(TRIG_PIN, LOW);
    delayMicroseconds(2);
    digitalWrite(TRIG_PIN, LOW);
    delayMicroseconds(10);
    digitalWrite(TRIG_PIN, HIGH);

    // Wait for Echo pin (with timeout)
    unsigned long startTime = millis();
    while (digitalRead(ECHO_PIN) == LOW) {
        if (millis() - startTime > 100) return;  // Exit if timeout
    }

    // Measure Echo duration
    duration = 0;
    while (digitalRead(ECHO_PIN) == HIGH) {
        duration++;
        delayMicroseconds(1);
    }

    // Convert to distance (integer math)
    distance = (duration * 34) / 2000;

    // LED logic
    if (distance > 0 && distance < 10) {
        digitalWrite(LED_PIN, HIGH);
    } else {
        digitalWrite(LED_PIN, LOW);
    }

    delay(500);
}











