# Smart-warehouse
A small IoT project which reads the temperature of the room and sends the temperature to a server using a simcard. The project is designed for a smart warehouse and it is implemented by an arduino and a sim800l module.

the implementation starts with connecting arduino-uno, sim800l module, the resistor which measures temperature and a DC to DC convertor(LM2596),they should be connected as followed:


![connections](https://github.com/pariyamd/Smart-warehouse/blob/master/images/connections.jpg)

i did not connect sim800l module to arduino pins as shown above, i connected them to a0 and a1 analogue pins of arduino,but i guess any other pin should work.
here is a picture of my implementations:

![implementation](https://github.com/pariyamd/Smart-warehouse/blob/master/images/implemented1.jpg)
