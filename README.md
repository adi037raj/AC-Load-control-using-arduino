# Bulb-Control-By-Arduino-and-Mobile

## [Download the app] (from the play store)
## [Arduino Code](/bluetooth/bluetooth.ino)

### Implementing a system where we can automatically switch on or off any two appliances through a mobile device using Arduino Uno and Bluetooth module.

### COMPONENTS REQUIRED:
1. Arduino Uno
2. Bluetooth Module HC-05
3. 2 channel Relay
4. Breadboard
5. 2 Bulbs
6. Wires
7. [A Bluetooth Control App](https://github.com/Devansh-Maurya/Bulb-Control-By-Arduino-and-Mobile/raw/master/Bluetooth%20Bulb%20Control.apk)

### ARDUINO UNO
It can be powered by a USB cable or by an external 9 volt battery, though it accepts voltages between 7 and 20 volts. It is also similar to the Arduino Nano and Leonardo. The hardware reference design is distributed under a Creative Commons Attribution Share-Alike 2.5license and is available on the Arduino website. Layout and production files for some versions of the hardware are also available.

![Arduino](/arduino.png "Arduino")

### BLUETOOTH MODULE
HC‐05 module is an easy to use Bluetooth SPP (Serial Port Protocol) module, designed for transparent wireless serial connection setup. The HC-05 Bluetooth Module can be used in a Master or Slave configuration, making it a great solution for wireless communication. This serial port Bluetooth module is fully qualified Bluetooth V2.0+EDR (Enhanced Data
Rate)3Mbps Modulation with complete 2.4GHz radio transceiver and baseband. It uses CSR Bluecore 04‐External single chip Bluetooth system with CMOS technology and with AFH (Adaptive Frequency Hopping Feature).

<p align="center">
  <img src="/bluetooth.png">
</p>

The HC-05 has two operating modes, one is the Data mode in which it can send and receive data from other Bluetooth devices and the other is the AT Command mode where the default device settings can be changed. We can operate the device in either of these two modes by using the key pin as explained in the pin description.

### RELAY
The Arduino Relay module allows a wide range of microcontroller such as Arduino, AVR, PIC, ARM with digital outputs to control larger loads and devices like AC or DC Motors, electromagnets, solenoids, and incandescent light bulbs. This module is designed to be integrated with 2 relays that it is capable of control 2 relays.The relay shield use one QIANJI JQC-3F high-quality relay with rated load 7A/240VAC,10A/125VAC,10A/28VDC.The relay output state is individually indicated by a light-emitting diode.

<p align="center">
  <img src="/relay.png">
</p>

The relay has two outputs-normally open and normally closed (NO and NC). When the IN1 or IN2 pin is connected to ground, NO will be open and NC will be closed, and when IN1 or IN2 is not connected to ground the opposite occurs. Connecting a circuit or device between one of these two pins, the common pin on the relay output, and a power source will allow you to toggle power to a circuit or device.


### CIRCUIT:
The necessary circuit for the project can be built up with the help of the following diagram.
The diagram shows connection of a single relay. It can be extended to two bulbs using a 2
channel relay.

![Circuit](/circuit.png "Circuit")

#### To make the proper circuit for the connections, follow the given instructions:

1. Provide Vcc and ground to the relay, either by taking two wires directly from the
Arduino, or by using a breadboard.
2. Connect one end of the wire connected to the bulb to the relay’s NC part, and
connect the other part, labelled as COM to the power supply directly. Repeat the
same process with the other bulb. As we are using a two-channel relay, the Vcc and
ground will be the same for both the relays.
3. Connect the other wires coming out of both the bulbs to the main power supply.
4. Take two wires from digital pins **2 and 3** of the Arduino and connect them with the
input pins 1 and 2 of relay. The pins 2 and 3 are the output pins.
5. To connect the Bluetooth module, connect the Vcc and GND pins of Bluetooth
module with the Vcc and GND pins of Arduino.
6. Connect the **TX and RX** pins of the Bluetooth module with the **pins 10 and 11** of
the Bluetooth module, as the pins 10 and 11 of the Arduino board have been defined
as the RX and TX pins.

### WORKING:

Follow the following steps to use the model:
1. Give power to the Arduino board by connecting it with any 5V power source either
by using the cable provided with the board.
2. The Bluetooth module LED will start blinking rapidly, which indicates that the
Bluetooth module is ready to accept a connection, but is not yet connected.
3. Now open the Android app and press the SHOW PAIRED DEVICES button at the
bottom of the screen. If the Bluetooth module is already paired up, it will show up
there. If it doesn’t show up, go to the Bluetooth options in the settings of your
Android phone and scan for the Bluetooth module and pair the mobile phone with it.
4. Now, if you will click on the name of the Bluetooth module from the app, you will be
taken to the next screen, from where you will be able to control the bulbs. The
controlling process has already been described in the app section.

### CONCLUSION:
Thus, finally we can see how using a prebuilt technology in our mobile phones, i.e.,
Bluetooth, we are able to control electrical appliances if our home. The technology can find
numerous uses in the daily life.

