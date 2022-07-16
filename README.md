wireless adb basic

	1. Initiating The ADB:
	- Head over to the ADB website and download and extract the package on your computer.
	- Launch the Settings app on your Android device, tap on Developer options, and enable the option that says USB debugging.
	  This is the option that lets you connect your computer to your Android over ADB.
	- Plug-in your Android device to your computer using a USB cable.
	- Launch a Command Prompt window (Windows) or Terminal window (Mac) in the ADB folder that you just extracted from the package. 
	  Type in the following command into the window and hit Enter.
			adb devices (windows)
			./adb devices (mac)
	- A prompt asking if you’d like to allow USB debugging will appear on your device’s screen.
	  Checkmark the Always allow from this computer box and tap on OK.
	- You’ll see your Android device listed in your command line window. Type in the following command and hit Enter.
	  There won’t be an output for this command.
			adb tcpip 5555 (Windows)
			./adb tcpip 5555 (Mac)
	- You’ve successfully set up the ADB service on port number 5555.

	2. Finding Out The IP Address Of The Android Device:
	- Launch the Settings app on your Android device and tap on About phone at the bottom.
	- On the following screen, tap on the option that says Status which will let you see your network details.
	- Scroll down on the following screen and you’ll find an entry saying IP address.
	  This is the address you’ll be using so note it down somewhere.
	- You now know the location of your device on your network and it’s time to establish a connection between two of your machines.

	3. Connect Wirelessly To An Android Device Using ADB:
	- Get back to your command line window, type in the following command, and hit Enter. 
	  Be sure to replace IP with the actual IP address of your Android device.
			adb connect IP (windows)
			./adb connect IP (Mac)
	- If all goes well, the command line will output a message saying you’re now connected to the specified IP address.
	- Now that you’re connected to your Android device using ADB,
	  you can issue any of the ADB commands you know and those will be executed on your Android phone.

wireless adb without usb

	1. Initiating The ADB:
	- Launch an android emulator on your Windows/mac
	- Launch a Command Prompt window (Windows) or Terminal window (Mac) in the ADB folder that you just extracted from the package. 
	  Type in the following command into the window and hit Enter.
			adb devices (windows)
			./adb devices (mac)
	- You’ll see your Android(emulator) device listed in your command line window. Type in the following command and hit Enter.
	  There won’t be an output for this command.
			adb tcpip 5555 (Windows)
			./adb tcpip 5555 (Mac)
	- You’ve successfully set up the ADB service on port number 5555.

	2. Finding Out The IP Address Of The Android Device:
	- Launch the Settings app on your Android device and tap on About phone at the bottom.
	- On the following screen, tap on the option that says Status which will let you see your network details.
	- Scroll down on the following screen and you’ll find an entry saying IP address.
	  This is the address you’ll be using so note it down somewhere.
	- You now know the location of your device on your network and it’s time to establish a connection between two of your machines.

	3. Connect Wirelessly To An Android Device Using ADB:
	- Get back to your command line window, type in the following command, and hit Enter. 
	  Be sure to replace IP with the actual IP address of your Android device.
			adb connect IP (windows)
			./adb connect IP (Mac)
	- If all goes well, the command line will output a message saying you’re now connected to the specified IP address.
	- Now that you’re connected to your Android device using ADB,
	  you can issue any of the ADB commands you know and those will be executed on your Android phone.
	  
NB: u must at first use the basic method (for initialitation) before u can use the fully wireless method (with emulator)
