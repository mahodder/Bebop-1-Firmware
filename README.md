Connect your PC to your WiFi network of Bebop
Start a Telnet client to connect to 192.168.42.1
Type "you version.txt" followed by ENTER
Type "r0" (lower case r, zero) to change the first digit of the version "0". This will make you believe to Bebop to have an older version of the firmware and then he will update
Type ": wq" followed by ENTER to save changes to files
Connect FTP address 192.168.42.1 and send the file "updater_payload.plf" folder "internal_000"
Disconnect from FTP and Telnet in return
Type "/bin/updater/updater_scan.sh / data / ftp / internal_000" followed by ENTER (note the space after "sh")
At this point you will see a written like this:
Type "reboot" followed by ENTER
Wait patiently for the firmware installation. During installation, the LED will blink in green orange and Bebop will test engine. When the cooling fan will begin the installation will be completed