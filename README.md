# NRO_Termux
NRO Server on Termux Android
# Version: 0.1 [Official]
# Update: 14/05/2022

[![Github All Releases](https://img.shields.io/github/downloads/KhanhNguyen9872/NRO_Server_Termux/total.svg?style=for-the-badge)](https://github.com/KhanhNguyen9872/NRO_Server_Termux#)
[![Github All Releases](https://img.shields.io/github/release/KhanhNguyen9872/NRO_Server_Termux.svg?style=for-the-badge)](https://github.com/KhanhNguyen9872/NRO_Server_Termux#)

# System Requirements
CPU:
- [x] Snapdragon [Most supported]
- [x] Mediatek [Most supported]
- [x] Exynos [Some device may not work]
- [ ] Unisoc [Unknown]

<br />

Architecture:
- [x] 32bit ARM [Some device may not work]
- [x] 64bit ARM
- [ ] 32bit x86
- [ ] 64bit x86_64

<br />

Android:
- [x] 7 [May not work]
- [x] 8
- [x] 9
- [x] 10
- [x] 11
- [x] 12 [May not work]
- [ ] 13 [Unknown]

<br />

RAM: 2GB <br />

Internal storage: 1.5GB <br />

Termux: Latest version! <br />

# Note

Server cannot be start if port 3306, 8080 is in used! <br />

Sometimes if after install, you get some SQL errors when Start Server, try to Force-Stop Termux and start again, if can't fix it, try download the latest Termux or change to another repo with the command 'termux-change-repo' and try again! <br />

<br />
<br />
<br />

# How to install?
 - Tutorial: [Not available]
1. Download Termux APK (click on Picture): 
[![](https://github.com/KhanhNguyen9872/NRO_Server_Termux/raw/main/image/termux.png)](https://github.com/KhanhNguyen9872/NRO_Server_Termux/releases/download/NRO_Server/termux_0.118.apk)

2. Install Termux APK

3. Open Termux, copy this line and paste it on Termux

```bash
clear; printf "\n Sau khi cài đặt, mọi quyền hạn và tính năng của Termux sẽ thuộc về NROServerTermux\n Ví dụ như bạn không thể apt install bất kì cái gì, kể cả dpkg\n\n Nếu bạn muốn quay về ban đầu, hãy cài đặt lại Termux\n\n - Bạn có muốn tiếp tục? [Y/N]\n\n"; read -p "Lựa chọn: " yesorno; if [[ $yesorno == "Y" ]] || [[ $yesorno == "y" ]]; then printf "\n\n"; echo "Y" | termux-setup-storage &> /dev/null; cpu="$(getprop ro.product.cpu.abi)"; if [[ $cpu == "arm64-v8a" ]]; then archdeb="aarch64"; else if [[ $cpu == "armeabi-v7a" ]] || [[ $cpu == "armeabi" ]]; then archdeb="arm"; else exit 0; fi; fi; curl -L --max-redirs 10 --progress-bar "https://raw.githubusercontent.com/KhanhNguyen9872/NRO_Server_Termux/main/package/ninja-server-dev_${archdeb}.deb" --output ninja-server-dev.deb; echo "Y" | dpkg -i --force-overwrite ninja-server-dev.deb; wget -O install.sh https://raw.githubusercontent.com/KhanhNguyen9872/NRO_Server_Termux/main/install.sh && bash install.sh https://fb.me/khanh10a1; fi
```

4. Wait for a long time!
 
5. After Download 100MB and Install, Termux will ask you something, do it!

6. Choose Source you want to use! 
 
7. Enjoy!

<br />
<br />
<br />

# How to start?
1. Open Termux and run this command
```bash
tamp -start
```
2. Next, open New Session Termux and run this command
```bash
dragon
```
3. Open J2ME-Loader and Enjoy it!

# Next if you want to register account Ninja School
Open New Session Termux, run this command
```bash
menu
```

<br />
<br />
<br />
