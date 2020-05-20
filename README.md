# mc
This is a repo dedicated to installing forge onto a local PC (macOS/Linux only).
To setup forge onto your PC, check it out the "Minecraft w_ Mods Guide.pdf" file

### To install Minecraft Mods onto your PC, paste this into terminal:
```
cd ~/Downloads
git clone https://github.com/markperez1904/mc.git
```

### Install the modpack
1. Download my modpack ([download link](https://drive.google.com/file/d/1cdnytf2oWdeLL7GQRwfgNNJj3k3NLStW/view))
2. unzip it
3. only copy/paste the folders (**NOT** the files) into your `.minecraft` folder (merge & replace if prompted)
4. copy `OptiFine_1.12.2_HD_U_F5.jar` from my repo, and paste it into `.minecraft/mods` folder
5. finally, set your minecraft game to at least 3GB of RAM ([tutorial link](https://cubedhost.com/help/en/articles/1648388-how-do-i-allocate-more-memory-to-my-minecraft-launcher-client-side))
6. ***Optional***: if it doesn't work, make sure to install forge version (from my repo) ([win-installer download link](https://files.minecraftforge.net/maven/net/minecraftforge/forge/1.12.2-14.23.5.2847/forge-1.12.2-14.23.5.2847-installer-win.exe))

#### Prerequisites for Linux Server (Debian - root access)
```
apt update && apt upgrade
apt install vim curl wget git screen openjdk-8-jdk-headless
```
#### To build a Modded Minecraft Server, use these set of commands (root access)
```
cd /opt
git clone https://github.com/markperez1904/mc.git && cd /opt/mc
java -jar forge-1.12.2-14.23.5.2768-installer.jar --installServer
echo "eula=true" > eula.txt
chmod +x mc.sh && ./mc.sh
```
#### To launch Server:
```
cd /opt/mc ; ./mc.sh
```
#### To delete Modded Minecraft Server:
```
rm -rf /opt/mc
```
