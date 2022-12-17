# Microprocessors 1 @ UMass Lowell
# Christopher Aguirre
# PIC32MM0064GPL036 Microcontroller

1) Inputs:
S1 (RB7), S2 (RB13)

2) Functionality:
* If S1 held down, emit LED1
* If S2 held down, emit LED2
* If S1 & S2 held down at the same time, blink LED 3 (period 0.25 sec), turn off LED1 & LED2
* If both are not held down,  emit LED3

3) Outputs:
LED1 (RA0), LED2 (RC9), 3rd LED placed into some slot on PIC board

4) Scenario:
- Hold down S1 (LED 1 should emit, LED3 blink 1 sec)
- Keep holding S1, then hold S2 (LED1 & LED2 should be off, LED3 blinking 0.25 sec)
- Let go of S1 (LED1 should turn off, LED2 should stay on, LED3 blink 1 sec)
- Let go of S2 (LED2 should turn off, LED3 blink 1 sec)
- Hold S2 (LED2 should turn on, LED3 stay at 1 sec blink rate)
- Hold S1 (LED1 should turn on, then LED3 should blink 0.25 sec delay)
- Let go of both (LED1 & LED2 off, LED3 blink 1 sec)
