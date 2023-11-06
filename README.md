# EXPERIMENT--03-SIMULATION-OF-PUSHBUTTON-AND-LED INTERFACE WITH ARM CONTROLLER AND PROTEUS 
## Aim: To Interface a Digital output (LED) and Digital input (Pushbutton) to ARM development board , and simulate it in Proteus 
## Components required: STM32 CUBE IDE, Proteus 8 simulator .
## Theory 
The full form of an ARM is an advanced reduced instruction set computer (RISC) machine, and it is a 32-bit processor architecture expanded by ARM holdings. The applications of an ARM processor include several microcontrollers as well as processors. The architecture of an ARM processor was licensed by many corporations for designing ARM processor-based SoC products and CPUs. This allows the corporations to manufacture their products using ARM architecture. Likewise, all main semiconductor companies will make ARM-based SOCs such as Samsung, Atmel, TI etc.

What is an ARM7 Processor?
ARM7 processor is commonly used in embedded system applications. Also, it is a balance among classic as well as new-Cortex sequence. This processor is tremendous in finding the resources existing on the internet with excellence documentation offered by NXP Semiconductors. It suits completely for an apprentice to obtain in detail hardware & software design implementation.
## STM 32 CUBE PROGRAM :
```
Developed by : Tejusve Kabeer.F
Register no : 212222100054
#include "main.h"
#include "stdbool.h"
bool buttonstatus;
 while (1)
  {
	 buttonstatus= HAL_GPIO_ReadPin(GPIOA, GPIO_PIN_0);
	 if(buttonstatus==0)
	 {
		 HAL_GPIO_WritePin(GPIOA, GPIO_PIN_1, GPIO_PIN_RESET);
HAL_Delay(500);
HAL_GPIO_WritePin(GPIOA, GPIO_PIN_1, GPIO_PIN_SET);
HAL_Delay(500);
	 }
	 else
	 {
		 HAL_GPIO_WritePin(GPIOA, GPIO_PIN_1, GPIO_PIN_RESET);
	 }
  }
```
## Output screen shots of proteus  :
![ou1](https://github.com/Reebak04/EXPERIMENT--03-SIMULATION-OF-PUSHBUTTON-AND-LED-WITH-PROTEUS-/assets/118364993/81859a5a-a1b5-4129-8936-0f1729df32e5)

![ou2](https://github.com/Reebak04/EXPERIMENT--03-SIMULATION-OF-PUSHBUTTON-AND-LED-WITH-PROTEUS-/assets/118364993/4ecd2817-8a10-467b-ad58-942d8d242838)
## Proteus layout :
 ![ou3](https://github.com/Reebak04/EXPERIMENT--03-SIMULATION-OF-PUSHBUTTON-AND-LED-WITH-PROTEUS-/assets/118364993/c29d990e-53c2-490a-9f90-367cbf047ef8)

## Result :
Interfacing a digital output and digital input  with ARM microcontroller are simulated in proteus and the results are verified.


