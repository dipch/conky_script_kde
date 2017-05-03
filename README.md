# conky_script_kde
Awesome conky scripts modified for KDE 
Conky is a system monitor software for the X Window System. It is available for GNU/Linux and FreeBSD. It is free software released under the terms of the GPL license. Conky Manager offers a simple GUI for managing and customizing conkys. Additional theme packs are available, too. KDE often conflicts with default ```conkyrc``` file. So, KDE users need to slightly change their conkyrc scripts. Here is procedure for installing/configuring ```conky``` ```conky-manager``` in KDE.  

![My desktop](https://github.com/charbaak/conky_script_kde/blob/master/Preview.png)
# Installing Conky
### For Ubuntu/Linux Mint
```sudo apt-get install conky-all``` 
### For Arch linux/Manjaro
```sudo pacman -S conky-lua``` (with lua support)
```sudo pacman -S conky-lua-nv``` (with both lua & nvidia support)

# Installing Conky Manager
### For Ubuntu/Linux Mint
##### Via ppa
```sudo apt-add-repository -y ppa:teejee2008/ppa```
```sudo apt-get update```
```sudo apt-get install conky-manager```
##### Via .deb file
[64bit]
### For Arch linux/Manjaro
```yaourt -S conky-manager```

##### To start conky just enter :
```$ conky``` or
```$ conky -d```
To edit conky you need to open the conkyrc and change the parameters :
```$ sudo nano ~/.conkyrc```
A lot of conkyrc files can be found around the net, check google and deviantart in particular. 

### Fixing isssues with KDE
Simply open any ```.conkyrc``` file and replace

```own_window yes
own_window_transparent yes
own_window_type normal
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
```

##### with,

```own_window yes
own_window_type dock
own_window_argb_visual yes
own_window_transparent yes
own_window_hints below,skip_taskbar,sticky
```

### Additional
Install ```curl```, ```lm-sensors```, ```hddtemp``` packages.

Now download included ```conky``` folder. Rename it to ```.conky```  and place in
```/home/user``` directory (replace with previous ```.conkyrc``` folder)
Open ```conky-manager``` and enable widgets

##### VOILA!
##### Feel the geek look.
