# Lenovo-Hackintosh
macOS Catalina on Lenovo lap top from 2017 and later

<h2>Info</h2>

<h3>Tested on configuration</h3> 

- Computer model : IdeaPad 520-15IKB

- Processor	: Intel Core i5-8250U

- Memory : 12GB Samsung DDR4 2400MHz

- Integrated Graphics : 	Intel UHD Graphics 620

- Sound Card : (layout-id:13)

- Wireless Card :	Original Intel Wireless 8265 swapped to (BCM94360NG - airdrop, wifi, bluetooth, everything works)

<h3>Current Status in Clover</h3>

- Discrete graphic card doesn't work, since macOS doesn't support Optimus technology

SSDT-DDGPU disabled in order to save power

- Fingerprint sensor is not working

SSDT-USB disabled in order to save power

- Original Intel Bluetooth has sleep problems and does not support some Bluetooth devices

(swapped to wifi/bt card BCM94360NG solved problem)

- Intel Wi-Fi (Intel Wireless 8265) has beta kext that partly works

<a href="https://www.tonymacx86.com/threads/success-working-intel-wifi-drivers-for-7265ac-on-catalina.292207/page-27">Find kext here</a>

(I swapped card to BCM94360NG, everything works perfect)

- USB SD Card Reader is not working

SSDT-USB disabled in order to save power



Everything else works perfect!!!

<h3>Installation</h3>

1. Download and copy EFI folder

2. Generate serial number and other with clover...

3. When booting press FN+F4 or F4 to dump ORIGIN files

4. Open Origin folder and copy DSDT to Patched folder

5. Open Terminal.app and run sudo kextcache -i /

6. Restart


In order to get working touchpad, battery status and more, you need to copy DSDT.


<h3>Wifi and Bluetooth change card</h3>

- If you want to have Airdrop, handoff, wifi, bluetooth and other stuff working, you need to buy BCM94360NG card, its about 40$ and it's easy to find it online.

It's important to remove all kexts related to wifi, before installing new card in lap top. 

Card is plug n play, no need for any setup or kexts.

<h3>Screenshots</h3>

<p align="center">
  <img src="https://i.imgur.com/cShAl8t.png"> 
  <img src="https://i.imgur.com/BXi1ZKX.png">
  <img src="https://i.imgur.com/ITS7LgW.png">
</p>

