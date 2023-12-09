# Inspire Video Demo 2

This guide provides how to setup the Base Station (BS) and User Equipment (UE) for the Inspire Video Demo II. 

---
# **Table of Contents**
1. [Setup](#Setup) 
    1.2 [Base Station Setup](#Setup1.2) 
    1.3 [User Equipment Setup](#Setup1.3) 
2. [Launching](#Launching) 
    2.1 [Base Station Launch Commands](#BaseStationLaunch) 
    2.2 [User Equipment Launch Commands](#UserEquipmentLaunch) 
3. [Video Hosting](#VideoHosting) 
    3.1 [Base Station Commands](#BaseStationVideoCommands) 
    3.2 [User Equipment Commands](#UserEquipmentVideoCommands) 
4. [Prioritization](#Prioritization) 
    4.1 [Traffic Control](#TCCommands) 
    4.2 [Traffic Control Bandwidth](#BandwidthCommands) 
5. [Inteference](#Interference) 
---
# 1. Setup <a name = "Setup"></a>
---
### 1.1 Base Station Setup <a name = "Setup1.2"></a>
#### Commands:
```
cd ~/srsran-control/enb
sudo python3 support.py
```
---
### 1.2 User Equipment Setup <a name = "Setup1.3"></a>
#### Commands:
```
cd ~/srsran-control/ue
sudo python3 support.py
```
---
# 2. Launching <a name = "Launching"></a>
---
### 2.1 Base Station Launch Commands<a name = "BaseStationLaunch"></a>

**In a New Terminal Window**
#### Commands:
```
cd ~/srsran-control/enb
sudo python3 launch.py
```
---
### 2.2 User Equipment Launch Commands<a name = "UserEquipmentLaunch"></a>

**In a New Terminal Window**

#### Commands:
```
cd ~/srsran-control/ue
sudo python3 launch.py
```
---
# 3 Video Hosting (Base Station)<a name = "VideoHosting"></a>
---
### 3.1 Base Station Host Commands<a name = "BaseStationVideoCommands"></a>

**In a New Terminal Window**
#### Commands:

```
cd ~/inspire/docker-testbed/local/resources/
bash video1-server.sh
```
---
### 3.2 Video Receive (User Equipment)<a name = "UserEquipmentVideoCommands"></a>

**In a New Terminal Window**
#### Commands:

```
cd ~/srsran-control/video/
# ls to see available videos
bash {video-file.sh}
```
---
# 4. Prioritization (Base Station)<a name = "Prioritization"></a>
---
### 4.1 TC Set-up Commands <a name = "TCCommands"></a>
--
**In a New Terminal Window**

```
# Access using BS
cd ~/srsran-control/enb/
bash tc-setup-commands.sh
```
---
### 4.2 Add Mbps To TC <a name = "BandwidthCommands"></a>
```
cd ~/srsran-control/enb/
bash tc-setup-commands.sh {Mbytes}
```
#### Where {Mbytes} refers to max transfer rate (Mbps)
---
# 5. Interference <a name = "Interference"></a>
---
### Access using Silver 3
```
#TBD
```

