# mc
To download all the files: open up the terminal and paste in:
```
cd ~/Downloads
git clone https://github.com/markperez1904/mc.git
```
Prerequisites for Linux Server (Debian - root access)
```
apt update && apt upgrade
apt install vim curl wget git screen openjdk-8-jdk-headless
```
To build a Minecraft Server, use these set of commands (root access)
```
cd /opt
git clone https://github.com/markperez1904/mc.git && cd /opt/mc
java -jar forge-1.12.2-14.23.5.2768-installer.jar --installServer
echo "eula=true" > eula.txt
chmod +x mc.sh && ./mc.sh
```
To delete Minecraft Server:
```
rm -rf /opt/mc
```
