Message of the Day for Termux.     
### Screenshot：  
![](https://github.com/Moe-hacker/termux-motd/raw/main/.screenshot.png)
### Thanks:
[Generator/termux-motd](https://github.com/Generator/termux-motd)           
### Installation：        
```shell
git clone https://github.com/Moe-hacker/termux-motd ~/.motd
echo ~/.motd/init.sh >> ~/.bashrc
echo ~/.motd/init.sh >> ~/.zshrc
```
If your device has docker support:        
```shell
mv ~/.motd/26-docker.disabled ~/.motd/26-docker
```
