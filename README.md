Termux的motd(欢迎界面信息显示)脚本。      
### 截图：  
![](https://github.com/Moe-hacker/termux-motd/raw/main/.screenshot.png)
相比脚本原版修改：        
Android logo居中输出，无论字体/窗口大小如何变化，下次输出始终居中。        
Cpu核心计数修复，原版通过读取cpuinfo获取cpu核心数可能会比实际数量多1，原因是cpuinfo这个文件的格式问题，改成lscpu成功解决。        
增加docker自启和状态显示，手机没大佬适配docker内核的看看就行了。       
disk usage横条根据屏幕宽度自动调整。        
原版：[Generator/termux-motd](https://github.com/Generator/termux-motd)           
### 使用：
内核有docker支持的，可在安装docker后将目录中的26-docker.disabled重命名为26-docker。        
```shell
git clone https://github.com/Moe-hacker/termux-motd ~/.motd
echo ~/.motd/init.sh >> ~/.profile
echo ~/.profile >> ~/.zshrc
chmod 777 ~/.profile
```
有docker支持的需额外运行：      
```shell
mv ~/.motd/26-docker.disabled ~/.motd/26-docker
```
