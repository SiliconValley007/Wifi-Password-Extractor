# Wifi-Password-Extractor
This python script, once run will extract all the wifi passwords saved on the system and save it to a txt file. When you run the script, multiple cmd screen will open and close one after another and once everything has settled down, you will find a .txt file named "Wifi Passwords", inside which you will find all the saved wifi passwords on your system.

The steps for Implementation of the script are as follows:
• Import the subprocess module
• Get the metadata of the wlan(wifi) with the help of check_output method
• Decode the metadata and split the metadata according to the line
• From the decoded metadata get the names of the saved wlan networks
• Now for each name again get the metadata of wlan according to the name
• Start try and catch block and inside the try block, decode and split this metadata and get the password of the given wifi name
• Write the wifi name and password to the text file and print blank if there is not password
• In the except block if process error occurred print encoding error occur red.
