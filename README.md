# RF-TRANSMITTER-AND-RECEIVER
Building a RF transmitter circuit and RF receiver circuit without arduino using HT12D and HT12E

#### 1. LIST OF COMPONENTS USED IN THE EXPERIMENT

  1. Leds 
  2. Resistors (1M ohm, 51K ohm, 1k ohm)
  3. HT12D (Decoder)
  4. HT12E (Encoder)
  5. Push Buttons
  6. Antenna

#### 2. BRIEFLY  EXPLAIN  THE FUNCTION OF EACH COMPONENTS

  1. LEDs- its used as an indicator to show that the receiver is receiving a signal.
  2. Resistors-help to reduce the flow of electric current
  3. HT12E- it is an encoder which is used to encode (protect/encrypt)  the data to be transmitted
  4. HT12D- it is a decoder and it is used to decode(decrypt) the data that is received
  5. Push Buttons- are connected to the data line of the HT12E and is used to send data when pressed(grounded).
  6. Antenna- it is an interface between radio wave propagation through space

#### 3. PROCEDURE

The transmitter module consists of three pins that is VCC, Data and GND. The VCC pin has a wide range input voltage from 3V to 12V. The transmitter consumes a minimum current of 9mA and can go as high has 40mA during transmission. The centre pin is the data pin to which the signalto be transmitted is sent.The signal is then modulated using ASK(Amplitude Shift Keying) and then sent on air at a frequency of 434MHz. The speed at which it can transmit data is 10kbps.

The receiver module has four pins namely VCC, Dout, Linear Out and GND. The VCC pinshould be powered by a regulated 5V DC power supply. The operating current of this module is 5.5mA. The pins Dout and Linear Out is shorted together to receive the 434MHz signal from air. The signal is then demodulated to get the data and is sent out through the data pin.

HT12E is an encoder IC that converts the 4-bit parallel data from the 4 data pins into serial data in order to transmit over RF link using transmitter. While HT12D is a decoder IC that converts the serial data received by the RF receiver  into 4-bit  parallel data and drives the LED accordingly.

#### 4. EXPLAIN THE CIRCUIT OPERATION

The transmitter/receiver pair operates at a frequency of 434MHz. An RF transmitter receives serial data and transmits it wirelessly through RF through its antenna connected at pin 4. The transmission occur at the rate of 1kbps-10kbps. The transmitted data is received by an RF receiver operating at the same frequency as that  of the transmitter. The RF module is used with a pair of encoder and decoder. The encoder is used for encoding parallel data for transmission feed while reception is decoded by a decoder.

#### CIRCUIT DIAGRAM
![My Image4](/Images/RF-transeiver.png)
