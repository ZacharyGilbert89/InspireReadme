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
```
cd ~/srsran-control/enb
sudo python3 launch.py
```
## UE Launch Commands
```
cd ~/srsran-control/ue
sudo python3 launch.py
```

## Video Hosting (BS)
### BS Host Commands
```
cd ~/inspire/docker-testbed/local/resources/
bash video1-server.sh
```
## Video Receive (UE)
### Video Recieve Commands
```
cd ~/srsran-control/video/
# ls to see available videos
bash {video-file.sh}
```

## Prioritization (BS)
### TC Set-up Commands 
```
# Access using BS
cd ~/srsran-control/enb/
tc-setup-commands.sh
```
### Add MBYTES To TC
```
tc-setup-commands.sh {bytes}
```
## Interference 
### Access using Silver 3
```
#TBD

```

