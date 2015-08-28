0. INTRODUCTION

It is highly recommended to read the excellent stack documentation from Microchip before proceeding. The demo is based on the original Microchip Application Libraries. The TCPIP version is 5.31 - part of Microchip Application Libraries v2010-10-19.

--------------------------------------------------------------------------------

1. RUNNING THE DEMO

You might use the prebuilt files in directory "Prebuilt". If you wish to build the demo yourself please continue reading.

Open "./TCPIP Demo App/TCPIP Demo App-C18.mcw" workspace. 

*Note: In order to compile successfully you need to have MC18 installed. Please also ensure that project directories are set properly to match path of the compiler (i.e. right-click the project->Build Options...->Directories tab).
	
Now you can compile the project and download it to the board. Of course, you can also use the project as a starting project for your custom application.
	
	
2. UPDATING THE WEB PAGE


The source web page files for PIC-MICRO-WEB are located in 
	./TCPIP Demo App/WebPagesOlimex"
	
You should run the "./Microchip/TCPIP Stack/Utilities/MPFS2.exe" to regenerate the image file (default is "MPFSImg2.bin") that shoulb be uploaded to the flash memory of the board.

Then, assuming PIC-WEB has IP address 192.168.0.30, open the following URL in your web browser: "http://192.168.0.30/mpfsupload". Browse to "MPFSImg2.bin" and upload it. After that the new web page should be available.

*Note: You might also use the ready MPFSImage2.bin located in directory "Prebuilt"

3. LOCATING PIC-WEB

Run the "./Microchip/TCPIP Stack/Utilities/Microchip Ethernet Discoverer.exe" utility in order to find what IP address has PIC-WEB fetched from DHCP. Another option is to connect a serial port to the board RS232 connector, configure your terminal application for 19200 8N1, and see the board status messages during power up.

*Note: Default setting of the board is to use DHCP to retrieve network configuration (IP address, etc.).. This can be modified by editing the "TCPIPConfig.h".

Last edit: 11 Nov 2013

Special thanks to Paolo for providing this demo!



