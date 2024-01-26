## Adafruit CAN Bus BFF Add-On for QT Py PCB

<a href="http://www.adafruit.com/products/5877"><img src="assets/5877.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit CAN Bus BFF Add-On for QT Py. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5877

### Description

Our QT Py boards are a great way to make very small microcontroller projects that pack a ton of power - and now we have a way for you to turn many QT Py boards into powerful CAN bus devices that are super small!

CAN Bus is a small-scale networking standard, originally designed for cars and, yes, busses, but is now used for many robotics or sensor networks that need better range and addressing than I2C, and don't have the pins or computational ability to talk on Ethernet. CAN is 2 wire differential, which means it's good for long distances and noisy environments.

Messages are sent at about 1Mbps rate - you set the frequency for the bus and then all 'joiners' must match it, and have an address before the packet so that each node can listen in to messages just for it. New nodes can be attached easily because they just need to connect to the two data lines anywhere in the shared net. Each CAN devices sends messages whenever it wants, and thanks to some clever data encoding, can detect if there's a message collision and retransmit later. 

If you'd like to connect your QT Py or Xiao to a CAN Bus, the Adafruit CAN Bus BFF will work with any and all boards thanks to the simple SPI interface! The controller used is the MCP26525 - also known as the MCP2515 controller plus MCP2551 transceiver, an extremely popular and well-supported chipset that has drivers in Arduino and CircuitPython and only requires an SPI port and 1 pin for chip-select, plus another for optional IRQ. Use it to send and receive messages in either standard or extended format at up to 1 Mbps.

We've added a few nice extras to this BFF to make it useful in many common CAN scenarios:

* JST PH socket - Plug in one of our JST PH 3-pn cables (not included!) for fast wiring and connection/disconnection. Black wire is ground, Red wire is CAN H, White wire is CAN L.
* 120 ohm termination resistor on board, you can remove the termination easily by cutting the jumper on the top of the board.
* Pre-connected CS pin to A3. There's also jumpers if you want to connect the IRQ, Reset and Silent pins.

We include some header that you can solder to your QT Py. You can also pick up an Itsy Bitsy short female header kit to make it removable but compact, you'll just need to trim down the headers to 7 pins long. Works with any QT Py or Xiao-shaped board that has the SPI port and A3 pin available.

QT Py and JST PH 3-Pin cable is not included.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
