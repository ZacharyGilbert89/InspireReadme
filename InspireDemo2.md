<a href="https://airanaculus.com" target="_self" itemprop="url"><img decoding="async" width="321" height="60" style ="background: black; margin: auto;" alt="AiRANACULUS" itemprop="image" data-srcset="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png 321w, https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb-300x56.png 300w" title="AiRANACULUS" data-src="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png" data-sizes="(max-width: 321px) 100vw, 321px" class="pp-photo-img wp-image-169 ls-is-cached lazyloaded" src="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png" sizes="(max-width: 321px) 100vw, 321px" srcset="https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb.png 321w, https://cv45a2.p3cdn1.secureserver.net/wp-content/uploads/2020/06/tgffb-300x56.png 300w">
</a>

---

# Inspire Video Demo 2

This guide provides how to setup the Base Station (BS) and User Equipment (UE) for the Inspire Video Demo II. 

---
# **Table of Contents**

---
# 1. Setup
---
### 1.1 Base Station Setup
#### Commands:
```
cd ~/srsran-control/enb
sudo python3 support.py
```
---
### 1.2 User Equipment Setup
#### Commands:
```
cd ~/srsran-control/ue
sudo python3 support.py
```
---
# 2. Launching
---
### 2.1 Base Station Launch Commands

**In a New Terminal Window**
#### Commands:
```
cd ~/srsran-control/enb
sudo python3 launch.py
```
---
### 2.2 User Equipment Launch Commands

**In a New Terminal Window**

#### Commands:
```
cd ~/srsran-control/ue
sudo python3 launch.py
```
---
# 3 Video Hosting (Base Station)
---
### 3.1 Base Station Host Commands

**In a New Terminal Window**
#### Commands:

```
cd ~/inspire/docker-testbed/local/resources/
bash video1-server.sh
```
---
### 3.2 Video Receive (User Equipment)

**In a New Terminal Window**
#### Commands:

```
cd ~/srsran-control/video/
# ls to see available videos
bash {video-file.sh}
```
---
# 4. Prioritization (Base Station)
---
### 4.1 TC Set-up Commands
--
**In a New Terminal Window**

```
# Access using BS
cd ~/srsran-control/enb/
bash tc-setup-commands.sh
```
---
### 4.2 Add Mbps To TC
```
cd ~/srsran-control/enb/
bash tc-setup-commands.sh {Mbytes}
```
#### Where {Mbytes} refers to max transfer rate (Mbps)
---
# 5. Interference
---
### Access using Silver 3
```
#TBD
```
---
<div style="font-size: 5px;">Authors: Zach Gilbert, Keegan Chhay</div> 
