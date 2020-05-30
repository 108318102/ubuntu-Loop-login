# ubuntu-Loop-login

- Ctrl+Alt+F2進入命令界面

- 輸入以下命令確認顯示管理器
```
cat /etc/X11/default-display-manager
```
- 如果是LigthDM
```
sudo vi /etc/lightdm/lightdm.conf
```
- 註釋自動登入命令
```
#autologin-user=<user_name>
#autologin-user-tineout=0
```
- 如果是GDM3
```
sudo vi /etc/gdm3/custom.conf
```
- 註釋自動登入命令
```
#AutomaticLoginEnable = true
#AutomaticLogin = <user_name>
```
- 如果是SDDM
```
sudo vi /etc/sddm.conf.d/autologin.conf
```
- 註釋自動登入命令
```
#[Autologin]
#User=<user_name>
```
- reboot
