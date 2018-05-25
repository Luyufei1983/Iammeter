<!-- toc -->

![Product Image][0]

eBay Link:
https://www.ebay.com/itm/132635546075
https://www.ebay.com.au/itm/132635546075

## 1 Product Introduction
iMeter-WiFi is highly-integrated, single-phased power meter with Wi-Fi module embedded and 1 RS-485 port, which can measure and transmit the data of specific electricity equipments, such as single-phase AC voltage, current, power etc. It supports MODBUS-RTU protocol.
iMeter-W can be connected to our energy online monitoring system-*Iammeter* (http://www.iammeter.com/) by one-key setup.

## 2 Installation
### 2.1 Wire Connection
iMeter-WiFi can be easily fixed into distribution box. Refer to the below picture for L/N wire and antenna connection. 
UL port: Live line
UN port: Neutral Line
Aerail port on the left bottom: Antenna port
![Wiring][1]
### 2.2 C/T Connection
**Step1**,Open the C/T;
**Step2**, View the bottom-marked current flow of C/T, live wire across C/T from bottom-marked L to N;
**Step3**, Close the C/T
![C/T][2]
## 3 WiFi configuration
**Step1**, Power on the meter, use a smartphone/laptop to search the WiFi signal from the Meter. (SSID: Netmeter_xxxxxxxx, xxxxxxx is Meter SN)

>Note: Note down the Meter SN for later registration on *Iammeter*.

![WiFi signal][3]
**Step2**, Connect to WiFi signal
**Step3**, Open the browser(IE, Chrome, Firefox...) and type in http://11.11.11.1/
**Step4**, Type the username and password (Username:admin,Password:admin)
![admin][4]
**Step5**:,Enter setting page
5.1 Connect to home router by clicking "Find AP" or manually input home router's SSID
5.2 Input password of home router as "Key" 
5.3 Click "Save&Reboot"
![Wifi Setting][5]
Step6: Connect to Netmeter_xxxxxxxx again, then input IP address http://11.11.11.1/ on browser and click "IP Address". If the meter has obtained the IP address from the home router (pictured as below), it means connected successfully.
![IP address][6]
###4 Registration on Iammeter
**Step1,** Confirm the WiFi setting is correctly done and the internet service is normal for your home wifi network
**Step2,** Visit Iammeter website (http://www.iammeter.com/), click "System" on top menu bar, and the login page is shown
**Step3,** Click "Sign up", fill up the information on sign up page, 
enter the meter SN noted previously into SN column
![Sign up][7]
**Step4** : Log into *Iammeter*, you can see the meter is already added in the system, click "My place" on the left menu bar to edit the location and time zone information. 

>Note: Time zone must be correctly selected or it will affect the data statistics on daily basis.

![My place][8]
**Step5**, now you can check the online data chart and report on Iammeter.
![Overview][9]

[0]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/imeter-lewei50-20180116-1.jpg
[1]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-1.jpg
[2]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-2.jpg
[3]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-3.jpg
[4]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-4.jpg
[5]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-5.jpg
[6]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-6.jpg
[7]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-7.jpg
[8]: http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180112-8.jpg
[9]:http://leweidoc.oss-cn-hangzhou.aliyuncs.com/lewei50/img/iMeter-lewei50-20180111-1.jpg