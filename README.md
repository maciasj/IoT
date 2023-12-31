# MiniProject1 for IoT course
This Mini Project1, designed for the IoT course, centers around the utilization of an m3 board. The project facilitates the reading of temperature/pressure via "lps start/stop" commands and acceleration/magnetic force through "lsp start/stop" commands on the m3 node. Temperature and pressure data are collected every 30 seconds, while accelerometer and magnetometer data are gathered every 15 seconds. Subsequently, this information is transmitted to an AWS cloud server, specifically configured to receive these calls.

To get started, set up the RIOT environment following the instructions outlined at https://github.com/RIOT-OS/RIOT. Additionally, establish the border router by referring to https://www.iot-lab.info/learn/tutorials/riot/riot-public-ipv6-m3/.

Conduct an experiment in FitIoT Lab and submit the .elf file into one node. Locate the node's firmware in MiniProject/task01 by executing the command "make."
Once the firmware is flashed into the board you can activate the sensors, lps for temperature and pressure and lsm for acceleration and magnetic force, by:
```bash
lps start
lsm start
```
To stop the sensors from reading data you can also do:
```bash
lps stop
lsm stop
````

In the video demonstration provided below, the operational AWS CoAP server is showcased. Unfortunately, due to challenges in obtaining the IPv6 address, the nodes are not connected to the cloud service. Complications also arose in configuring the CoAP client, resulting in compilation errors with local files from other RIOT folders. However, a successful GET call from the laptop is demonstrated.

https://drive.google.com/file/d/1CCrxBQtsxZgoeXTnDD2AEPtg2aGmS_1H/view?usp=sharing

A note to the professor expresses regret for not achieving all project goals, citing challenges faced as a degree exchange student learning from scratch. 
Despite these obstacles, valuable learning experiences were gained, acknowledging difficulties in collaboration with an unresponsive partner.

