# mc
This is a repo dedicated to installing forge onto a local PC (macOS/Linux only).
To setup forge onto your PC, check it out the "Minecraft w_ Mods Guide.pdf" file

To install Minecraft Mods onto your PC, open up the terminal and paste in:
```
cd ~/Downloads
git clone https://github.com/markperez1904/mc.git
```
Prerequisites for Linux Server (Debian - root access)
```
apt update && apt upgrade
apt install vim curl wget git screen openjdk-8-jdk-headless
```
To build a Modded Minecraft Server, use these set of commands (root access)
```
cd /opt
git clone https://github.com/markperez1904/mc.git && cd /opt/mc
java -jar forge-1.12.2-14.23.5.2768-installer.jar --installServer
echo "eula=true" > eula.txt
chmod +x mc.sh && ./mc.sh
```
To launch Server:
```
cd /opt/mc ; ./mc.sh
```
To delete Modded Minecraft Server:
```
rm -rf /opt/mc
```
