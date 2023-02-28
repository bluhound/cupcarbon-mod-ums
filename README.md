# cupcarbon-mod-ums
Modified Cupcarbon 5.2

Forked from https://github.com/bounceur/CupCarbon for the purpose of PhD UMS Sabah.

Modifications done to this fork:

Build 14 February 2023
1. Fixed SenScript’s ‘receive’ command that causes an infinite freeze to the automation sequence
2. Increased default node buffer from 1KB to 10MB
3. Changed default LoRa frequency from 868 MHz to 923 MHz
4. Changed the default radius for LoRa’s radio from 5 km to 1.6 km
5. Changed default radio (RADIO1) of sensor nodes from Zigbee to LoRa to ease deployment of virtual sensor nodes.
6. Removed Mac compatibility to simplify compiling in Windows environment.

Requires Java JDK 1.8. Tested on JDK 1.8b351.

Java parameters used:
.\jdk1.8.0_351\bin\java.exe -XX:+UseG1GC -XX:+UseStringDeduplication -Xms64M -Xmx16G -jar cupcarbon52.jar
