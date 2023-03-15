It exposes a number of **kernel parameters** as files so that we can easily reconfigure the kernel without specialized tools. It does not exist on **Windows and macOS** <!--SR:!2023-03-15,2,210-->

# brightness
We can change the brightness using the command below: 
```shell 
cd /sys/class/backlight/thinkpad_screen 
echo 3 | sudo tee brightness # tee program is used to open the /sys file for writing and it is running as root. 
```