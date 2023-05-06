# IOT-Access

## Name of Project
Access Location, Camera, and mic using rasberry PI device with Kali Linux

## Purpose
NOBODY is safe when it comes to Technology, Purpose of this project is to use Rasberry PI device with KALI LINUX to Obtain Device information without any permission. Access Locations, access cameras, access microphone.

## Dependencies 
* Storm Breaker
  * php
  * python3
  * git
  * Ngrok

## Equipment
* [Rasberry PI](https://www.amazon.com/Raspberry-Pi-4-4G-Model/dp/B081YD3VL5/ref=sr_1_14?crid=36AFWDBCXWU86&keywords=rasberry+pi+4%2B&qid=1683306173&sprefix=rasberry%2Caps%2C275&sr=8-14&ufe=app_do%3Aamzn1.fos.f5122f16-c3e8-4386-bf32-63e904010ad0)
* [USB Micro Data Cable](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_ffob_sspa?crid=DO75SIR3SOBU&keywords=micro+usb+data+cable&qid=1678902219&sprefix=Micro+USB+data%2Caps%2C119&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUEyODVZTFRIVTQ3WFhUJmVuY3J5cHRlZElkPUEwMDU4NDczMkU3RTJKNllMTkpJSCZlbmNyeXB0ZWRBZElkPUEwMTg1MTU1MjBZR042R1ZLNTUzUCZ3aWRnZXROYW1lPXNwX2F0ZiZhY3Rpb249Y2xpY2tSZWRpcmVjdCZkb05vdExvZ0NsaWNrPXRydWU=)
*  [HDMI](https://www.amazon.com/AmazonBasics-High-Speed-HDMI-Cable-1-Pack/dp/B014I8SIJY/ref=sr_1_1_ffob_sspa?crid=15PE2GIND6GN4&keywords=hdmi&qid=1683307963&sprefix=hdmi%2Caps%2C305&sr=8-1-spons&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFDUjVYN003R0FLNTgmZW5jcnlwdGVkSWQ9QTAxMTAxMjgyT1dVMU5GMjM0NjBRJmVuY3J5cHRlZEFkSWQ9QTEwMzMyMTgySkxBWkpYUFFQUElBJndpZGdldE5hbWU9c3BfYXRmJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ&th=1)
*  [MicroSD Card](https://www.amazon.com/SanDisk-2-Pack-microSDHC-Memory-2x32GB/dp/B08J4HJ98L/ref=sr_1_3?crid=KB3HHVZ44PIC&keywords=micro+sd+card+32gb&qid=1683308044&sprefix=micro+sd+%2Caps%2C257&sr=8-3)
*  [mouse](https://www.amazon.com/Wireless-YOOSO-Computer-Adjustable-Ergonomic/dp/B094QH5MWN/ref=sr_1_2_sspa?crid=17O5QS2YNRBMR&keywords=mouse&qid=1683308190&sprefix=mouse%2Caps%2C416&sr=8-2-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFQSTAxSkFRRUJJNzgmZW5jcnlwdGVkSWQ9QTAzOTQyMzQxRUY4QUQ1VkJKRDJLJmVuY3J5cHRlZEFkSWQ9QTA2OTU4ODEzNlY1Q1FYQTFSTDRCJndpZGdldE5hbWU9c3BfYXRmJmFjdGlvbj1jbGlja1JlZGlyZWN0JmRvTm90TG9nQ2xpY2s9dHJ1ZQ==)
*  [Micro Keyboard](https://www.amazon.com/Backlit-Keyboard-Touchpad-Wireless-Multimedia/dp/B07QNPX8C2/ref=sr_1_9?crid=3DQ1JCBQSRLBM&keywords=micro+keyboard&qid=1683308256&sprefix=micro+keyboard%2Caps%2C269&sr=8-9)
## Link for Document
- [Github - UltraSecurity/Strom-Breaker](https://github.com/ultrasecurity/Storm-Breaker)
<!--(https://www.youtube.com/watch?v=h_f9lB4i-LA)-->

<a href="https://www.youtube.com/watch?v=h_f9lB4i-LA" target="_blank"><img src="https://github.com/Kenielmc/IOT-Access/blob/main/Screenshot%202023-05-05%20132309.png" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

## Steps I Followed
* Download [Rasberry PI imager](https://www.raspberrypi.com/software/)

* Save to Micro sd card(make sure it's more than 8gbs)

* Once installed for Username: kali Password: kali

* Open terminal

* you will need to download [StormBreaker](https://github.com/ultrasecurity/Storm-Breaker)

* Enter command in Kali linux and get storm breaker running 
  * Commands get into the root dir
  * Sudo su
  * cd /opt
  * git clone https://github.com/ultrasecurity/Storm-Breaker.git
  * apt install python3-requests python3-colorama python3-psutil
  * bash install.sh
  * pyhton3 st.py (runs the storms breaker program)
  * split the terminalby right clicking and selecting split terminal
  
* Follow steps to get into the root strom breaker directory
  * sudo cd /opt
  * Storm-Breaker

* In the meanwhile you will need to sign up for a free account at Ngrok to be obtain a token to link the system to be able to use the FULL functionality of the software, meaning outside your local network
  * Go ngrok.com and register
* Once done you will copy your token and paste it to the second terminal. Your command should look like this
  * ngrok authtoken XXXXXXXXXXXXXXXXXXXXXXX( the x represents your personal authtoken)
  
* To run the tunnel enter command 
  * ngrok http 2525

* A black screen will appear copy and paste the fowarding link into your web browser 

 
  
