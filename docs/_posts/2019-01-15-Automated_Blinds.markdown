---
layout: post
title:  "Automated Blinds Project"
date:   2019-01-15 09:32:26 +0000
categories: Engineering Projects
---

### Project Summary:
This was a solo project undertaken to automate the task of raising and lowering bedroom blinds. This was completed with simply using two lasers and photo-sensitive resistors to accurately measure the binary state of the blind position. A DC motor and driver were fitted inside of the blind for discrete actuation, and a simple arduino script was used for logic.

Although not the most technically complex project in the list, this is significant for its reliability and longevity. It has been changing state twice per day for 5 years with no need for maintenance so far!


### Gallery and Code
<div style="display: flex; flex-wrap: wrap;">
    <img src="/assets/Blinds/Blind1.jpeg" alt="Farm V1" style="flex: 1; max-width: 50%;" />
    <img src="/assets/Blinds/Blind2.jpeg" alt="Farm V2" style="flex: 1; max-width: 50%;" />
</div>

\
*Simple arduino logic:*
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