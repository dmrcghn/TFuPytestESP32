<p align="center">
    <img src="images/tensorflow-micropython-examples.png">
</p>

# Tensorflow Micropython Examples - Renewed, maybe

This is a fork of https://github.com/mocleiri/tensorflow-micropython-examples
For most relevant information, see there. I only forked it because the binaries for the firmware to upload to an ESP32 
was showing as "expired" on the original project page. As of 2024 Sept 26th, you can find the bin file here for an ESP-WROOM-32:

https://github.com/DOBsby/TFuPytestESP32/actions/runs/11068324078

To flash it successfully (without it continuously rebooting), I used this exact command per the screenshot in the repo I forked this from

esptool --port COM4 write_flash -z 0x1000 firmware.bin

(you'll probably need to change "COM4" to your port)
