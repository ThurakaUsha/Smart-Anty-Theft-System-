# Smart-Anty-Theft-System-
Security and safety have always become a basic necessity in the present World to secure and guard the house in our  absence.The fundamental idea is to design a cost effective and efficient system for an individual to be able to detect any kind of theft in real-time  and provide instant notification of the theft to the house owner.

How does it work?

As you know, the NodeMCU is a WiFi-enabled microcontroller, Which can connect to the internet via WiFi. 
So, using the BLYNK Blynk application, we can activate the device. For this purpose, we connected the button with the virtual pin, so that when the activate button is pressed, the value in the variable "state" will change from "1" to "0" (Refer code).

In the next step, if the "state" is 1, the PIR Sensor starts to check for the intruders. 
So, whenever an intruder (ie, motion) is detected, the sensor will send a HIGH value to the NodeMCU. When NodeMCU reads a HIGH value, an HTTP request will be sent from the NodeMCU. 
This HTTP request (WebHooks API) will trigger ClickSend SMS Service, thus we receive the SMS in our Phone as soon as the Motion is Detected.
HTTP (Hypertext Transfer Protocol) is a standard Application protocol that functions as a request-response protocol between client and server.

HTTP client helps to send HTTP requests and receive HTTP responses from HTTP server.

It is widely used in IoT based embedded applications like Home Automation, vehicle engine parameter monitoring remotely for analysis, etc.
