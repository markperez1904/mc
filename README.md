# mc
This is a repo dedicated to installing forge onto a local PC (macOS/Linux only).
To setup forge onto your PC, check it out the "Minecraft w_ Mods Guide.pdf" file

### To install Minecraft Mods onto your PC, paste this into terminal:
```
cd ~/Downloads
git clone https://github.com/markperez1904/mc.git
```

### Install the modpack
1. Download the modpack ([download link](https://www.curseforge.com/minecraft/modpacks/life-in-the-village-lite/files/2915654))
2. unzip it
3. only copy/paste the folders (not the files) into your minecraft folder
4. copy the mod files from my repo, and paste them into the minecraft mods folder
5. install this mod file. it's too big to upload on github ([download link](https://www.curseforge.com/minecraft/mc-mods/lycanites-mobs/files/2935745))
6. finally, set your minecraft game to at least 3GB of RAM ([tutorial link](https://cubedhost.com/help/en/articles/1648388-how-do-i-allocate-more-memory-to-my-minecraft-launcher-client-side))
7. ***Optional***: if it doesn't work, make sure to install forge version (from my repo)

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
