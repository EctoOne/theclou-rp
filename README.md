# The Clue! Linux Port

Basic Installation:
---
```
cd ~
git clone https://github.com/vcosta/derclou
cd derclou
make
```

Select Language:
---
```
wget "https://sourceforge.net/projects/cosp/files/Original Game Files/The Clue! + Profidisk (English)/TheClueProfiData.zip"
```
```
wget "https://sourceforge.net/projects/cosp/files/Original Game Files/The Clue! + Profidisk (German)/DerClouProfiData.zip"
```

Move Files:
---
```
sudo unzip TheClueProfiData.zip -d /opt/retropie/ports/derclou
sudo mv derclou /opt/retropie/ports/derclou/derclou
```

Add Plan Save Error Fix:
---
```
cd ~
git clone https://github.com/EctoOne/theclou-rp
cd theclou-rp/opt/retropie/ports/derclou/DATADISK/
sudo mv *.PLN /opt/retropie/ports/derclou/DATADISK/

cd ~
sudo mv /home/pi/theclou-rp/opt/retropie/configs/ports/derclou /opt/retropie/configs/ports/derclou
```

Move launch sript to Ports Rom folder:
---
```
cd /home/pi/theclou-rp/home/pi/RetroPie/roms/ports/
sudo mv "Der Clou.sh" "/home/pi/RetroPie/roms/ports/Der Clou.sh"
```

Cleanup:
---
```
cd ~
rm -rf derclou
rm -rf theclou-rp
```

# Controls:
* Arrow Keys to move selection / Person while planing
* Enter to select option
* ESC to undo while planing
* F1 opens Save/Load/Quit Menu

