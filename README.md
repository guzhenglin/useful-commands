# useful-commands
### 修改键盘映射
```shell
sudo vi /usr/share/X11/xkb/keycodes/evdev
```
*Windows*
```c
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout\Scancode Map填值
00 00 00 00 00 00 00 00
02 00 00 00 1C 00 3A 00              //00000002：两个功能交换  |  键盘扫描值(小端序)，用001C(Enter)实现003A(Caps_Lock)的功能
3A 00 1C 00 00 00 00 00              //00 00 00 00结尾
```

### 开关系统代理
```shell
#开
gsettings set org.gnome.system.proxy mode 'manual'
#关
gsettings set org.gnome.system.proxy mode 'none'
```
