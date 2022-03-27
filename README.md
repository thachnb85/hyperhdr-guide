# Installation
Download the RPI image and flash to SD card.
https://github.com/awawa-dev/HyperHDR

Access from: 192.168.0.12:8090
<img width="1591" alt="image" src="https://user-images.githubusercontent.com/21049491/160305265-cc031be3-7d2b-4fcc-9149-e8b6a21da0a8.png">

# Enable LED hardward
Without this step, LED hardware won't work.

```
ssh pi@192.168.0.12
```
Default ssh password is rapsberry

We need the service runs under `root`
```bash
sudo systemctl disable --now hyperhdr@pi
sudo systemctl enable --now hyperhdr@root
```

# Config the LEDs
<img width="949" alt="image" src="https://user-images.githubusercontent.com/21049491/160305229-129fb6fc-7808-4386-a5cd-26e3a5b3aada.png">

LED layout
<img width="1598" alt="image" src="https://user-images.githubusercontent.com/21049491/160305250-68e9edff-60d6-45f1-9389-0afb78dae140.png">
