# TCAN4550_DEMO

Description: A basic version of code to set up and receive a packet.
- This is designed to work with the EVM the TCAN4550EVM
- It assumes TCAN4550 Oscillator of 40 MHz
- Sets CAN arbitration rate at 500 kBaud
- Sets CAN FD data phase for 2 MBaud
- The interrupt pin is used for signal a received message, rather than polling

Pressing S1 will transmit a CAN message.
S1 is on the MSP430FR6989/MSP430FR5994 launchpad to the left.
```
   Pin             MSP430FR6989            MSP430FR5994
-  MOSI / SDI      P1.6                    P5.0
-  MISO / SDO      P1.7                    P5.1
-  SCLK            P1.4                    P5.2
-  ChipSelect/nCS  P2.5                    P5.3

-  MCAN Int 1/nINT P2.3                    P1.4
- Ground wire is important!!!```
