<img decoding="async" width="321" height="60" style ="background-color: black; margin: auto;" alt="AiRANACULUS" itemprop="image" data-srcset="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png 321w, https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb-300x56.png 300w" title="AiRANACULUS" data-src="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png" data-sizes="(max-width: 321px) 100vw, 321px" class="pp-photo-img wp-image-169 ls-is-cached lazyloaded" src="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png" sizes="(max-width: 321px) 100vw, 321px" srcset="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png 321w, https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb-300x56.png 300w">

# Inspire Video Demo 2

This guide provides how to setup the Base Station (BS) and User Equipment (UE) for the Inspire Video Demo II. 

---
## **Table of Contents**
   * [1. Setup ](#1-setup)
        * [1.1 Base Station Setup](#11-base-station-setup)
        * [1.2 User Equipment Setup](#12-user-equipment-setup)
   * [2. Launching ](#2-launching)
        * [2.1 Base Station Launch Commands](#21-base-station-launch-commands)
        * [2.2 User Equipment Launch Commands](#22-user-equipment-launch-commands)
   * [3 Video Hosting](#3-video-hosting)
        * [3.1 Base Station Host Commands](#31-base-station-host-commands)
        * [3.2 Video Receive (User Equipment)](#32-video-receive-user-equipment)
   * [4. Prioritization (Base Station)](#4-prioritization-base-station)
        * [4.1 TC Set-up Commands](#41-tc-set-up-commands)
        * [4.2 Rate Control](#42-rate-control)
   * [5. Interference](#5-interference)
        * [Access using Silver 3](#access-using-silver-3)
---
## 1. Setup 
##### Note: The UE and BS are on seperate machines.
---
#### 1.1 Base Station Setup
##### Commands:
```
cd ~/srsran-control/enb
sudo python3 support.py
```
---
#### 1.2 User Equipment Setup
##### Commands:
```
cd ~/srsran-control/ue
sudo python3 support.py
```
---
## 2. Launching 
---
#### 2.1 Base Station Launch Commands

##### **In a New Terminal Window**
##### Commands:
```
cd ~/srsran-control/enb
sudo python3 launch.py
```
---
#### 2.2 User Equipment Launch Commands

##### **In a New Terminal Window**

##### Commands:
```
cd ~/srsran-control/ue
sudo python3 launch.py
```
---
## 3 Video Hosting
---
#### 3.1 Base Station Host Commands

##### **In a New Terminal Window**
##### Commands:

```
cd ~/inspire/docker-testbed/local/resources/
bash video1-server.sh
```
---
#### 3.2 Video Receive (User Equipment)

##### **In a New Terminal Window**
##### Commands:

```
cd ~/srsran-control/video/
# ls to see available videos
bash {video-file.sh}
```
---
## 4. Prioritization (Base Station)
---
#### 4.1 TC Set-up Commands

##### **In a New Terminal Window**
##### Default Rate
```
# Access using BS
cd ~/srsran-control/enb/
bash tc-setup-commands.sh
```
---
#### 4.2 Rate Control
##### Specific Rate
```
cd ~/srsran-control/enb/
bash tc-setup-commands.sh {Mbytes}
```
##### Where {Mbytes} refers to max transfer rate (Mbps)
---
## 5. Interference
---
#### Access using Silver 3
```
#TBD
```
---
