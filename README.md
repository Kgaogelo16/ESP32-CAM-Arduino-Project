Smart Surveillance System (ESP32-CAM)
Overview

This project is a smart, energy-efficient surveillance system built using an ESP32-CAM module.
It autonomously detects motion using an ultrasonic sensor and captures images only when triggered, conserving power.

Note: In this implementation, an HC-SR04 ultrasonic distance sensor was used instead of a PIR motion sensor. The sensor triggers the camera when an object enters a pre-defined distance range.

Project Type

Group / Academic Project

Module: Logic Design 

Hardware Components

-ESP32-CAM Module – Executes trigger logic, controls the camera, stores images on microSD, and transmits data via Wi-Fi.

-OV7670 Camera Module – Captures images when motion is detected.

-HC-SR04 Ultrasonic Distance Sensor – Measures object distance and triggers image capture.

-MicroSD Card – Stores captured images locally.

-FTDI Programmer (USB to Serial) – Used to flash code to the ESP32-CAM.

-Breadboard & Jumper Wires – Provides prototyping platform and connections.

-5V 2A DC Power Adapter – Supplies stable power for the ESP32-CAM and peripherals.

-LED (optional) – Visual feedback for motion detection.

-Software & Tools

-Arduino IDE

-ESP32 Libraries

-My Contribution

-Wired and assembled the breadboard and components.

-Configured and programmed the ESP32-CAM module.

-Assisted with testing, debugging, and verifying motion-triggered image capture.

Documented the project workflow and results.

Team Members

-Ntuli KJB (You)
-NF Maluleke
-NS NZUZA
-OO Nkwane
-SR Mapulane

Teammate 2

How It Works

The ESP32-CAM continuously monitors the ultrasonic sensor for changes in distance.

When an object enters the predefined "trigger zone," motion is detected.

The onboard LED provides immediate visual feedback.

The camera captures a single frame in QQVGA RGB565 format.

Captured images are transmitted via Serial or stored on the microSD card.

The system loops back to monitor for further motion events.

Observations / Results

Distance Measurement: Sensor readings remain stable when no motion occurs.

Motion Detection: LED lights up when an object moves more than 10 cm from the previous distance.

Image Capture: Serial monitor prints BMP_START and BMP_END; images can be saved as BMP files.

System Performance: Motion triggers repeated image captures; images are low-resolution (160x120) but sufficient for basic surveillance.

Learning Outcomes

Hands-on experience with ESP32 microcontrollers and camera integration.

Understanding motion-triggered automation systems.

Hardware troubleshooting and debugging.

Teamwork in designing and implementing an embedded system.

Future Improvements

Increase camera resolution and frame rate.

Implement Wi-Fi image upload for real-time surveillance.

Add adjustable motion sensitivity for different environments.

Include advanced storage options or cloud integration.

References

ESP32 Official Documentation

OV7670 Camera Datasheet

HC-SR04 Ultrasonic Sensor Datasheet
