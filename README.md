# Quick_checks-for-arduino
This repository is mainly to check all the components 

![Arduino Board](https://www.distrelec.biz/Web/WebShopImages/landscape_large/0-/01/Arduino_UNO_WIFI_30117100-01.jpg)


#### `Testing of Arduino`

* Test the Arduino Board by using blinking an In-Built LED (Below code) 

```C++
/*
  This Code is written by Rahul Sharma for Yolabs. 
This is the  simplest code possible to blink in build LED  
Turns inbuild LED on and off at diff frequency to chk your arduino IDE, Arduino and cable is working
Note: please check the port in case you have error while uploadig 
 www.yolabs.in - 2020
  
*/

// the setup function runs once when you press reset or power the board

void setup()
{
  pinMode(13,OUTPUT);
  Serial.begin(9600);
}

void loop()
{
    digitalWrite(13, HIGH);
    
    Serial.println("I am High");
    delay(3000); // Wait for 1000 millisecond(s)
    digitalWrite(13, LOW);
    Serial.println("I am Low");
    delay(3000);
 
}


```

* Motor Driver Test Checking Code

```C++


/*
  This Code is written by Rahul Sharma for Yolabs. 
This is the  simplest code possible to blink in build LED  
Turns inbuild LED on and off at diff frequency to chk your arduino IDE, Arduino and cable is working
The same code can be used to check your external LED circuit. Please connect that in LED  
Note: please check the port in case you have error while uploadig 
 www.yolabs.in - 2020
  
*/

// the setup function runs once when you press reset or power the board

#include <AFMotor.h>


void setup()
{
  pinMode(13,OUTPUT);
  pinMode(A0,OUTPUT);
  
  Serial.begin(9600);
}

void loop()
{
    digitalWrite(13, HIGH);
    digitalWrite(A0, HIGH);
    
    Serial.println("I am High");
    delay(3000); // Wait for 1000 millisecond(s)
    digitalWrite(13, LOW);
    digitalWrite(A0, LOW);
    Serial.println("I am Low");
    delay(3000);
 
}


```


