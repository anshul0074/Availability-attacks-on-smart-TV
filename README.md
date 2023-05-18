# Availability-attacks-on-smart-TV
    Command Line Tool 

0. Python File Runner Tool 
    This script is designed to list all the Python files in the current directory and allow the user to run a selected file. 
    This tool allows you to run Python files in the current directory. It will list all the Python files in the directory and prompt you to select a file to run.

    USAGE 
    To use this tool, follow these steps:

    1. Navigate to the directory where your Python files are located.
    2. Run the script by typing `python3 tool.py` in the command line.
    3. The tool will list all the Python files in the directory (except for tool.py).
    4. Enter the number of the file you want to run. The tool will execute the file and return to the command prompt.

    ## Notes

        - This tool only works with Python 3.
        - The tool will only list files that end with the `.py` extension.
        - The tool will prompt you to enter the number of the file you want to run. If you enter an invalid number or a non-integer value, it will prompt you to enter a valid number.

    ## Requirements

        This tool requires Python 3 to be installed on your computer. It also requires the `os` and `subprocess` modules, which should be included with your Python installation.

    Note: This tool is used to run the subsequent files.   


1. Port Scanner

    This is a simple Python program for scanning open ports on a given IP address.
    USAGE

        Clone the repository or download the files to your local machine.
        Open the terminal and navigate to the directory where the files are located.
        Run the program using the command: python3 port_scanner.py
        Enter the IP address that you want to scan when prompted.
        Enter the range of port numbers to scan when prompted.
        Wait for the program to complete the scan.
        The program will display the open ports on the given IP address.

    Dependencies

    This program requires the following Python packages to be installed:

        pyfiglet
        argparse

    You can install these packages using the following command:
        pip3 install pyfiglet argparse


2. Wifi DoS Attack on Port

    This Python script performs a simple IP flooding attack on a target. It takes as input the IP address of the target and the port number to be attacked. It uses the hping3 tool to send a large number of packets to the target, which can cause the target to become unresponsive.
    
    Requirements
        hping3 tool must be installed on the system.
        Python 3.x should be installed.

    USAGE

        Run the script using the following command:
            python ip_flooding_attack.py
            Enter the IP address of the target when prompted.
            Enter the port number to be attacked when prompted.
            The script will perform the IP flooding attack on the target.

3. Wifi Deauth Attack

    This Python script performs a WiFi deauthentication attack on a selected wireless network. The script first checks for any existing .csv files in the current working directory, moves them to a /backup directory, and creates a new .csv file to store the results of the attack. It then prompts the user to select a wireless interface to use for the attack, and puts it into monitored mode using the airmon-ng utility.

    The script uses the airodump-ng utility to discover access points and continuously updates the results in the .csv file. It then displays the list of access points and prompts the user to select a target by ESSID. Once the target is selected, the script uses the aireplay-ng utility to launch a deauthentication attack against the target.

    The script also includes error handling, such as checking for the presence of a WiFi adapter and ensuring that the user enters a valid input when selecting a wireless interface or target ESSID.


    USAGE

        Connect your wireless interface
        Run the script with sudo privileges: sudo python3 wifi_dos.py
        Select the WiFi interface you want to use for the attack
        Wait for available networks to be displayed, and select the one you want to attack
        Press Ctrl+C to begin the attack

    NOTES

        This script is for educational purposes only. The author does not condone illegal or unethical use of this script.
        The script may not work on all WiFi adapters and drivers.
        If the script fails to find any wireless networks, try moving closer to a wireless access point.

    Requirements

        A WiFi adapter that supports monitor mode
        Aircrack-ng (install with sudo apt install aircrack-ng)


    Note : To quit any inifinite loop , press Ctrl + c.



4. Bluetooth Scanner

    This is a Python script that uses the Bleak library to scan for Bluetooth devices and print their information. The user can choose to run the script with or without threads.

    USAGE

        Install dependencies: This script requires the Bleak library to be installed. Install it using pip with the command:

        pip install bleak

        Run the script: Navigate to the directory where the script is located and run it with the command:

        python script.py

        Choose thread mode: When prompted, enter "1" if you want to run the script with threads, or "0" if you want to run it without threads. If you choose to use threads, you will be prompted to enter the number of threads to use.

        View output: The script will scan for Bluetooth devices and print their information to the console. Each thread will scan independently and print out the devices it discovers.

    NOTES

        This script has been tested on Python 3.8.5 and Bleak 0.11.0.
        When using threads, the number of threads should not exceed the number of available processor cores.
        The script suppresses warnings for convenience. Remove the line warnings.filterwarnings("ignore") if you want to see warnings.
        The script uses asyncio to run the Bleak scan function. This allows the script to be non-blocking and responsive.


5.  Bluetooth DoS Attack

    This script performs a Bluetooth denial-of-service (DoS) attack on a target device by sending a continuous stream of ping requests to it.
    
    USAGE

        Run the script with the following command:

        python3 bluetooth_dos.py

        Enter the MAC address of the target device and the desired packet size when prompted.

    

Note: Please use this script only for educational purposes and do not use it for any illegal or malicious activities. The author is not responsible for any damage caused by its usage.
