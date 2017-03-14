Connect your PC to your WiFi network of Bebop<br />
Click Bebop power button 4 times<br />
Start a Telnet client to connect to 192.168.42.1<br />
Type "vi version.txt" followed by ENTER<br />
Type "r1:wq" followed by ENTER. This will make you believe to Bebop it's running an older version of the firmware.<br />
Connect FTP address 192.168.42.1 and send the file "updater_payload.plf" folder "internal_000"<br />
Disconnect from FTP and Telnet back into Bebop<br />
Type "/bin/updater/updater_scan.sh / data / ftp / internal_000" followed by ENTER (note the space after "sh")<br />
Type "reboot" followed by ENTER<br />
Wait patiently for the firmware installation. During installation, the LED will blink in green orange and Bebop will test engine. When the cooling fan will begin the installation will be completed.