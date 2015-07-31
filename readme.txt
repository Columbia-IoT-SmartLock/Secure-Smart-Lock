This folder has the crypto server client code for our project
First release the "IoT_Security_StartingProject_latest version.RAR" from IOT_Project->GUI_Lock(1) 

Open this project using Atmel Studio 6.2
On the solution explorer on the right, select all .c and .h files under “src”, then right click,select remove->delete
Now exit Atmel Studio 6.2.

Open Atmel code folder and copy all the code to the “src” folder of the project.

Reopen Atmel Studio 6.2 and navigate to Solution Explorer > show all files. 
Select all files you just pasted, and left click > include files in the project.

Open demo.h change MAIN_WLAN_SSID to the wi-fi network you wish to use
 EX: Columbia University
            change MAIN_WLAN_PSK to the network password (for Columbia the MAIN_WLAN_AUTH should be M2M_WIFI_SEC_OPEN and leave the password "")
Now run the program. If wifi connection is successful, you will see the message: M2M_WIFI_REQ_DHCP_CONF: IP is XXX.XXX.X.XXX

Open the python file, change server_address = ('192.168.1.182', 6666) to server_address = ('XXX.XXX.X.XXX', 6666) with the IP you need to connect to.
Now run the python file and you will be able to see the result.

Always run Atmel first.
Once you have Atmel running, you should be able to run python file as many times you want to test.




