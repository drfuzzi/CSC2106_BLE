# Bluetooth Low Energy (BLE) IoT

## Objectives
- Familiarize yourself with Bluetooth Low Energy (BLE) IoT.
- Develop a BLE solution using M5StickC Plus boards.

## Equipment
- Computer / Laptop
- M5StickC Plus Kit

## Bluetooth Low Energy

Bluetooth Low Energy, often referred to as BLE, Bluetooth LE, or Bluetooth Smart, was initially designed by Nokia as Wibree and later implemented by the Bluetooth Special Interest Group (SIG). BLE operates in the 2.4 GHz frequency band and is optimized for low-power consumption. It uses a robust frequency-hopping spread spectrum (FHSS) approach with 40 channels for data transmission. Bluetooth 5 introduces support for various network topologies, including point-to-point, broadcast, and mesh networking.

BLE is independent of classic Bluetooth radio (also referred to as Bluetooth Basic Rate/Enhanced Data Rate or BR/EDR) and has no compatibility, but BR/EDR and LE can coexist. The Bluetooth classic radio is designed for low-power operation and leverages a robust FHSS approach, transmitting data over 79 channels. However, Bluetooth classic radio supports only a point-to-point network topology. You may learn more about the main differences between Bluetooth Classic and Bluetooth Low Energy [here] (https://www.bluetooth.com/learn-about-bluetooth/tech-overview/).

![image](https://github.com/drfuzzi/CSC2106_BLE/assets/108112390/b982bd43-89a1-453d-a563-b097ae9583ee)

Figure 1: Bluetooth Architecture

In this lab session, M5StickC Plus kits are used to develop BLE solution that takes advantage of the various sensors included in the kit. Figure 2 shows the simple pinout for the M5StickC Plus kit that shows the pins to be used to access the various sensors.

![image](https://github.com/drfuzzi/CSC2106_BLE/assets/108112390/786519ea-b43f-486e-8e69-bc78ec39ea22)
![image](https://github.com/drfuzzi/CSC2106_BLE/assets/108112390/378c4096-e11e-4843-a625-0c8f7e7bbb09)

Figure 2: M5StickC Plus - Structure block diagrams

In addition, the lab only covers point-to-point communication, and other modes like broadcast and mesh networks will not be covered. The lab session guides how to make a BLE connection between two M5StickC Plus kits, where one is designated as Server and the other as Client. The Server advertises its presence, so it can be found by other devices and contains data that the Client can read. The Client scans the nearby devices, and when it finds the Server it is looking for, it establishes a connection and listens for incoming data. The source code for both Server and Client can be found on the xSITe, under Lab Codes.

Step 1: Compile the Server code and upload it to one device.

Step 2: Compile the Client code and upload it to **another** device.

Step 3: Modify the Server code to obtain data from actual sensors and be notified of new readings.

At the end of this lab session, you have learned how to set up the M5StickC to connect it to another device via BLE, install the necessary libraries, and configure it for point-to-point communication. You have also tested the M5StickC with BLE, giving you a foundation for using it in future projects, i.e. indoor tracking, etc.

## Lab Exercise

In this lab session, M5StickC Plus kits are used to develop a BLE solution that utilizes various sensors included in the kit. The pinout diagram in Figure 2 shows the pins used to access these sensors.

Please note that this lab session only covers point-to-point communication, and other modes like broadcast and mesh networks will not be covered. The lab guides you through establishing a BLE connection between two M5StickC Plus kits, designating one as the Server and the other as the Client. The Server advertises its presence and contains data that the Client can read. The Client scans for nearby devices, establishes a connection with the Server, and listens for incoming data. You can find the source code for both [Server]() and [Client]() are here.

### Steps:
1. Compile the Server code and upload it to one device.
2. Compile the Client code and upload it to another device.
3. Modify the Server code to obtain data from actual sensors and be notified of new readings.

By the end of this lab session, you will have learned how to:
- Set up the M5StickC for BLE communication
- Install the necessary libraries
- Configure it for point-to-point communication
- Test the M5StickC with BLE, providing a foundation for future projects such as indoor tracking, etc.

## Lab Assignment

Extend your lab to incorporate the following functionality:

1. Press the button to change the LED status on the BLE server and set new notify status for the BLE Client.
2. Press the button to read characteristics from the BLE server on demand.
3. Press the button to write characteristics to the BLE server, changing the status of the LED on the Server.

## Reference

- [Bluetooth SIG](https://www.bluetooth.com/learn-about-bluetooth/radio-versions)
- [M5Stack Arduino Library](https://github.com/m5stack/M5StickC-Plus)
- [Arduino IDE environment for M5StickC Plus](https://docs.m5stack.com/en/quick_start/m5stickc_plus/arduino)
- [M5StickC Plus Documentation](https://docs.m5stack.com/en/core/m5stickc_plus)
- [M5StickC Plus Additional Documentation](https://cdn.competec.ch/documents2/8/5/9/185624958/185624958.pdf)
- [Bluetooth Technology Overview](https://www.bluetooth.com/learn-about-bluetooth/tech-overview/)
- [ESP32 BLE Server and Client (Bluetooth Low Energy)](https://randomnerdtutorials.com/esp32-ble-server-client/)
