\# Gesture Hardware Controller



A real-time gesture-controlled hardware system that enables touchless control

of physical devices using computer vision and embedded electronics.



The project uses a standard camera and hand tracking to control a stepper motor

and LED lighting via intuitive hand gestures.



---



\## Overview



This system connects computer vision to physical hardware through a layered

architecture:



\- Hand tracking using MediaPipe

\- Real-time gesture recognition in Python

\- Serial communication with Arduino

\- Stepper motor and LED control



The goal is to explore natural human–machine interaction for interactive

installations, robotics UI, and rapid hardware prototyping.



---



\## Features



\- Real-time hand tracking (single or dual hand)

\- Gesture-based control modes

\- Stepper motor position and speed control

\- LED on/off toggle via gesture

\- LED brightness control via hand rotation

\- Gesture hysteresis and smoothing

\- Modular architecture for easy extension



---



\## Gesture Controls



| Gesture | Action |

|------|------|

| Pinch (thumb + index) | Enable / clutch control |

| Hand rotation (right hand) | Stepper motor control |

| Fist (short) | Toggle LED on/off |

| Hand rotation (left hand) | LED brightness control |

| Long fist | Mode switching |



Gesture logic is designed to be robust against noise and accidental triggers.



---



\## System Architecture



Camera  

→ Python (OpenCV + MediaPipe + control logic)  

→ Serial protocol  

→ Arduino  

→ Stepper motor \& LED



Detailed architecture and gesture documentation can be found in the `docs/`

directory.



---



\## Hardware



\- Arduino Uno

\- 28BYJ-48 stepper motor + ULN2003 driver

\- LED (PWM controlled)

\- USB camera



---



\## Software



\- Python 3.10+

\- OpenCV

\- MediaPipe

\- Arduino IDE



Python dependencies are listed in `python/requirements.txt`.



---



\## Use Cases



\- Interactive installations

\- Touchless hardware interfaces

\- Robotics UI experiments

\- Creative technology prototypes

\- R\&D and rapid prototyping



---



\## Status



This project is a functional prototype intended for experimentation,

demonstration, and further development.



---



\## License



MIT



