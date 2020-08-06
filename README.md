# Smart-warehouse
A small IoT project which reads the temperature of the room and sends the temperature to a server using a simcard. The project is designed for a smart warehouse and it is implemented by an arduino and a sim800l module.

### preparing the hardware:
the implementation starts with connecting arduino-uno, sim800l module, the resistor which measures temperature and a DC to DC convertor(LM2596),they should be connected as followed:


![connections](https://github.com/pariyamd/Smart-warehouse/blob/master/images/connections.jpg)

i did not connect sim800l module to arduino pins as shown above, i connected them to a0 and a1 analogue pins of arduino,but i guess any other pin should work.
here is a picture of my implementations:

![implementation](https://github.com/pariyamd/Smart-warehouse/blob/master/images/implemented1.jpg)


### programming the arduino:
As a client, a TCP connection is stablished using the AT+COMMANDs in [datasheet](http://www.rhydolabz.com/wiki/wp-content/uploads/sim800_series_tcpip_application_note_v1.001.pdf) and the temperature is sent to server.(arduinouno.ino)

### on the server:
The data is saved to a file using "input.php".
now you can read the data from the file and display it (it is done in "server.php" but it can be more customized)
