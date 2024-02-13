---
layout: post
title:  "Automated Blinds Project"
date:   2019-01-15 09:32:26 +0000
categories: Engineering Projects
---

### Project Summary:
This was a solo project undertaken to automate the task of raising and lowering bedroom blinds. This was completed by simply using two lasers and photo-sensitive resistors to accurately measure the binary state of the blind position. A DC motor and driver were fitted inside of the blind for discrete actuation, and a simple Arduino script was used for logic.

Although not the most technically complex project on the list, this is significant for its reliability and longevity. It has been changing state twice per day for 5 years with no need for maintenance so far!


### Gallery and Code
<div style="display: grid; grid-template-columns: 1fr 1fr;">
  <img src="/assets/Blinds/Blind1.jpeg" alt="Blinds 1" style="max-width: 100%;">
  <img src="/assets/Blinds/Blind2.jpeg" alt="Blinds 2" style="max-width: 100%;">
</div>

\
*Simple Arduino logic:*
```
void loop() {
  if (digitalRead(UpButton) == LOW){
    digitalWrite(TopLaserPin, HIGH);
    while (analogRead(TopLDR) < 950){
      Serial.println(analogRead(TopLDR));
      digitalWrite (MotorOut1, LOW);
      digitalWrite (MotorOut2, HIGH);
    }
    digitalWrite (MotorOut1, LOW);
    digitalWrite (MotorOut2, LOW);
    digitalWrite (TopLaserPin, LOW);
  }
  if (digitalRead(DownButton) == LOW){
    digitalWrite(BottomLaserPin, HIGH);
    while (analogRead(BottomLDR) > 900){
      Serial.println(analogRead(BottomLDR));
      digitalWrite (MotorOut1, HIGH);
      digitalWrite (MotorOut2, LOW);
    }
    digitalWrite(BottomLaserPin, LOW);
    digitalWrite (MotorOut1, LOW);
    digitalWrite (MotorOut2, LOW);
  }
}
```