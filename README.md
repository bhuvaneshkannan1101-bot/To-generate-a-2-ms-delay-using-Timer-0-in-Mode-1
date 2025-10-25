# To-generate-a-2-ms-delay-using-Timer-0-in-Mode-1(212224060048)
## AIM
To Write an assembly language program in 8051 to generate a 2 ms delay using Timer 0 in Mode 1 and toggle an LED connected to Port 2.0.

## Apparatus Required
- Personal Computer  
- Keil µVision software  
---

## Algorithm
1. Start the program.
2. Initialize Port 2 as output port (used to connect LEDs).
3. P2 = 0x00; → Set all pins of Port 2 to logic LOW initially.
4. Enter an infinite loop (while(1)) to continuously blink the LEDs.
5. Turn ON all LEDs by sending logic HIGH to Port 2.
6. P2 = 0xFF;
7. Call the delay function to keep LEDs ON for a short period.
8. Turn OFF all LEDs by sending logic LOW to Port 2.
9. P2 = 0x00;
10. Call the delay function again to keep LEDs OFF for a short period.
11. Repeat steps 4–7 infinitely to create a continuous blinking effect.
12. End (program runs indefinitely).

## Program
```
#include<reg51.h>
void delay();
void main ()
{
	P2 = 0x00; 
  while (1) 
	{
		P2 = 0xFF;
    delay () ;
    P2 = 0x00;
    delay () ; 
	}
}
void delay()
{
	int i;
	for(i=0;i<=5000;i++)
	{
	}
}
```

## OUTPUT

<img width="1654" height="744" alt="Screenshot 2025-10-25 084048" src="https://github.com/user-attachments/assets/5ac94061-8a27-43fa-a508-cbe18cd204ed" />


## RESULT

Thus To Write an assembly language program in 8051 to generate a 2 ms delay using Timer 0 in Mode 1 and toggle an LED connected to Port 2.0 was done using keil software.


