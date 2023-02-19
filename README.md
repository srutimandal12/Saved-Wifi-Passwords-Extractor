# Saved-Wifi-Passwords-Extractor
-python


Usually while connecting with the wifi we have to enter some password to access the network, but we are not directly able to see the password we have entered earlier i.e password of saved network. In this article, we will see how we can get all the saved WiFi name and passwords using Python, in order to do this we will use subprocess module of python. Wi-Fi is a wireless networking technology that allows devices such as computers (laptops and desktops), mobile devices (smartphones and wearables), and other equipment (printers and video cameras) to interface with the Internet. The subprocess module present in Python(both 2.x and 3.x) is used to run new applications or programs through Python code by creating new processes. It also helps to obtain the input/output/error pipes as well as the exit codes of various commands.

Steps for Implementation :

Import the subprocess module
Get the metadata of the wlan(wifi) with the help of check_output method
Decode the metadata and split the meta data according to the line
From the decoded metadata get the names of the saved wlan networks
Now for each name again get the metadata of wlan according to the name
Start try and catch block and inside the try block, decode and split this metadata and get the password of the given wifi name
Print the password and the wifi name and print blank if there is no password
In except block if process error occurred print encoding error occurred
