<!-- toc -->
Start to connect your power meter to *Iammeter* from here,
## 1 Previous preparation
Confirm you have prepared:
1. Power meter which supports Modbus RTU protocol
2. DTU device (Serial to TCP) or download the Virtual DTU Software [Serial to TCP converter for Iammeter][0]
## 2 Registration on Iammeter
**Step1**, Visit homepage https://www.iammeter.com , click "System" on the top menu, 
![Login page][1]
**Step2**, Click "Sign up", fill up the information, tick "Sign up by demo sn" so that you can get a free SN for the power meter.
![Sign up page][2]
**Step3**, Configure the parameters of your power meter on Iammeter. 
Login to Iammeter, Click "Meters"->"Edit", fill up the Modbus parameters (Slave ID, Registers configuration) correctly.
![Modbus config][3]
**Step4**, Go to "My places" to configure the location & time zone. 
> Wrong time zone selection will affect the data statistics on daily basis.

![My place][4]

## 3 DTU configuration
### 3.1 If you have a DTU device
Configure the below information on DTU settings,
TCP Server： pm.modbus.lewei50.com
TCP Port: 9970
Register SN: The SN you get when signing up on Iammeter.
Other DTU Information: Serial parameters, Network parameters (GPRS or WiFi)...
The below picture is only for your referrence, please configure your DTU referring to your DTU manual.
![DTU Config][5]
### 3.2 If you have no DTU device
You can use the software [Serial to TCP converter for Iammeter][0] to simulate DTU device
**Step1,** connect your power meter to PC serial port by using 485 to serial or tcp converter;
**Step2,** run software *Serial to TCP converter for Iammeter* on your PC, fill up the register SN 
![Software][6]
## 4 Check online data on Iammeter
Login to Iammeter again to check you data,
![Overview][7]

[0]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/software/Serial%20To%20TCP%20Converter%20for%20Iammeter.zip
[1]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20170818-1.jpg
[2]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20170818-2.jpg
[3]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20170818-5.jpg
[4]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20170818-6.jpg
[5]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20180105-3.jpg
[6]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20180105-2.jpg
[7]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iammeter-lewei50-20180105-4.png
