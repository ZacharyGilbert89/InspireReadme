# Inspire Video Demo 2

Setting Up Video Demo

## BS Setup
### Setup Commands:
```
cd ~/srsran-control/enb
sudo python3 support.py
```
## UE Setup
### Setup Commands
```
cd ~/srsran-control/ue
sudo python3 support.py
```
## Launching
### BS Launch Commands

New Terminal Window
```
cd ~/srsran-control/enb
sudo python3 launch.py
```
## UE Launch Commands
New Terminal Window
```
cd ~/srsran-control/ue
sudo python3 launch.py
```

## Video Hosting (BS)
### BS Host Commands
New Terminal Window
```
cd ~/inspire/docker-testbed/local/resources/
bash video1-server.sh
```
## Video Receive (UE)
### Video Recieve Commands
New Terminal Window
```
cd ~/srsran-control/video/
# ls to see available videos
bash {video-file.sh}
```

## Prioritization (BS)
### TC Set-up Commands 
New Terminal Window
```
# Access using BS
cd ~/srsran-control/enb/
bash tc-setup-commands.sh
```
### Add MBYTES To TC
```
cd ~/srsran-control/enb/
bash tc-setup-commands.sh {bytes}
```
# Where {bytes} refers to max transfer rate
## Interference 
### Access using Silver 3
```
#TBD

```

