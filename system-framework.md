<!-- toc -->

## System framework
The framework of the iammeter platform and communication process are shown in the following flowchart.
![Framework][1]

The system framework includes:

**1. Modbus power meter**
Modbus power meter refers to any power meter which suports Modbus RTU protocol.  It can be seen as a RTU device and easily connected to *iammeter* by few steps of setup. 
**2. DTU devices (Serial to TCP)**
DTU devices (Serial to TCP) is like a gateway. It can not only communicate with Modbus power meter by standard serial port, but also communicate with TCP server by standard TCP/IP protocol.  It makes the power meter internet-enabled. 
There are different types of DTU devices, such as WiFi, Ethernet and GPRS. DTU devices can also be divided into built-in DTU (which is embeded inside the meter, such as the iMeter-W meter provided by us) and external DTU based on different ways of use.
We also developed a virtual Serial to TCP software in case you need to test on* iammter* when you have no a DTU devices on hand.
**3. TCP server**
TCP server is communicated with DTU devices by Socket.
**4. Data cloud**
All the data uploaded by power meter and user information are stored in data cloud for further data statistics and analysis.
**5. Online monitoring platform-Iammeter**
By calling all kinds of device data and user data of the data cloud, the *Iammeter* platform can display data and enrich online applications through abundant charts and reports.

## Communication process

The power meters communicates with the *Iammeter* by below process,

1. Sign up on *Iammeter*, you will get a Demo SN(Serial Number) for your power meter; This SN is like the unique ID of your power meter to access the system. Then you add your meter on *Iammeter*.
 
2. Set your DTU device, configure the TCP server information (IP address, port No.) and SN and other necessary settings;
3. After DTU configured, DTU can communicate with TCP server by establishing the TCP Socket.
4. TCP Server recieve the registration package(including the SN) sent by DTU, and find your *Iammeter* account information from database based on the SN.
5. TCP Server read the configuration information of the meter you created on your *Iammeter* acount
6. TCP Server communicates with your power meter via DTU and then store the realtime data recieved to the database under your account.
7. After all pervious steps, you can log into the *Iammeter* and view the online data chart of your meter.

 [1]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-PlatformStructure-20180111-1.jpg