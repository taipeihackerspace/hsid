Hackerspace ID (hsid)
====================

Continuing the people counter project, this is using the ubiquous
EasyCard system (which is basically a Mifare 13.56MHz RFID setup).

The aim of this whole thing is to make it easy to check in and out
of the hackerspace, and make it easy to see who was there and when,
see whether there's anyone at the space right now.

This project should include some hardware and plenty of software
to make it work. All components required should be listed here,
such that it enables replication of the project.

Planned parts
-------------

 * [ ] RFID identification and store in database
 * [ ] Checking in and out, button and automatic
 * [ ] Door opening sensor to warn people to check in and out
 * [ ] Web presence for person count
 * [ ] Statistics

Hardware
--------

 * Arduino Mega ADK, better brakeout of SPI pins for starters. Should replace it in the future with a bare ATMega chip
 * RFID-RC522 reader
 * LCD matrix display
 * LEDs and switches for interaction

Software
--------

 * [ ] Sketch to read and transmit RFID card serial numbers
 * [ ] Database to store person<->serial<->check in times
 * [ ] Local web interface adding name to users (as an optional activity)
 * [ ] Web interface for person counting / presence indication

Sources
-------

Some excellent starting information from the web.

 * A [small intro and excellent sketch to use with arduino][arduino]
 * [Pin schematics for Arduino Mega][pins] to use with this board
 * More in the [Arduino Forums][forum]


[arduino]: http://www.grantgibson.co.uk/blog/2012/04/how-to-get-started-with-the-mifare-mf522-an-and-arduino/ "How to get started with the Mifare MF522-AN and Arduino"
[pins]: http://www.b2cqshop.com/images/thumbs/0000433.jpg
[forum]: http://forum.arduino.cc/index.php?topic=111113.0 "MF522-AN RFID Reader"
