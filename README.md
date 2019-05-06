# Sixfab RPi CellularIoT HAT

Repository of Sixfab RPi CellularIoT HAT.

# Library Installation
## Manual Installation
```
git clone https://github.com/sixfab/Sixfab_RPi_CellularIoT_App_Shield.git
cd Sixfab_RPi_CellularIoT_App_Shield
sudo python3 setup.py install
```
[Sixfab_RPi_CellularIoT_App_Shield](https://github.com/sixfab/Sixfab_RPi_CellularIoT_App_Shield)

**! Note:** Sixfab_RPi_CellularIoT_HAT uses the same python library with Sixfab_RPi_CellularIoT_App_Shield. 
Please visit the library repo above. You can find the detailed instructions there. 

## Install with pip3
Use pip3 to install from PyPI.
```
sudo pip3 install sixfab-cellulariot
```

## Test
Enable `serial_hw` and `I2C` interfaces by following instructions below:  
1. Run `sudo raspi-config`
2. Select `5 Interfacing Options`
3. Enable `P5 I2C`
4. For `P6 Serial`
    * Disable `Login shell to be accessible over serial`
    * Enable `Serial port hardware`
5. Finish
6. Reboot
7. It's done.

```
cd sample
python3 sensor_test.py  #for testing sensor_test example
```

## Examples
** [basicUDP](https://github.com/sixfab/Sixfab_RPi_CellularIoT_App_Shield/blob/master/sample/basicUDP.py)   
** [buton_led_test](https://github.com/sixfab/Sixfab_RPi_CellularIoT_App_Shield/blob/master/sample/buton_led_test.py)   
** [sendSMS](https://github.com/sixfab/Sixfab_RPi_CellularIoT_App_Shield/blob/master/sample/sendSMS.py)   

## Tutorials
** [Basic UDP Communication Tutorial for Sixfab RPi CellularIoT HAT](https://sixfab.com/cellular-iot-hat-getting-started-with-udp-connection/)  
** [PPP Connection Tutorial](https://sixfab.com/ppp-installer-for-sixfab-shield/) 

# Pinout
![Pinout Schematic](https://sixfab.com/wp-content/uploads/2019/04/RPi_Cell_IoT_Hat_Pinout_2-e1555326552762.jpg)


# Attention
! All data pins work with 3.3V reference. Any other voltage level should harm your hat or RPI.

# Layout
![Layout](https://sixfab.com/wp-content/uploads/2019/05/RPi_Cell_IoT_Hat_Layout_3-1-e1557136705232.jpg)
