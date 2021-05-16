# Circular-buffer
Circular buffer for Arduino

Code ex.:

#######################################

#include "cbuff.h"

int SIZE = 3;

Cbuff<float> tmp(SIZE);
  
float a = 9.613;

float b = 12.971;

void setup() {

  Serial.begin(9600);
  
  tmp.push(a);
  
  tmp.push(b);
  
  tmp.printArr();
  
  Serial.println(tmp.get(0), 3);
  
}


void loop() {
}
#######################################
