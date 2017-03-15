Connect your PC to your WiFi network of Bebop<br />
Click Bebop power button 4 times<br />
Start a Telnet client to connect to 192.168.42.1<br />
Type "mount -o remount,rw /"
Type "vi version.txt" followed by ENTER<br />
Type "r1:wq" followed by ENTER. This will cause the Bebop to think it's running an older version of the firmware.<br />
Connect FTP 192.168.42.1 and send the file "updater_payload.plf" folder to the “internal_000" folder<br />
Disconnect from FTP and Telnet back into Bebop<br />
Type "/bin/updater/updater_scan.sh /data/ftp/internal_000" followed by ENTER (note the space after "sh")<br />
Type "reboot" followed by ENTER<br />
Wait patiently for the firmware installation. During installation, the LED will blink in green orange and Bebop will test engine. When the cooling fan will begin the installation will be completed.
Extra: Factory Reset drone by holding power button 15 seconds (this will reset all your drone settings to default, should be done if down grading)