# conky_script_kde

Conky is a system monitor software for the X Window System available for GNU/Linux and FreeBSD.KDE plasma often conflicts with default ```conkyrc``` file, hence needs to slightly change conkyrc scripts (>=KDE Plasma 5).

# Installing Conky
### For *buntu/Mint
```sudo apt-get install conky-all``` 
### For Arch/Manjaro
```sudo pacman -S conky-lua``` (with lua support)
```sudo pacman -S conky-lua-nv``` (with both lua & nvidia support)

# Installing Conky Manager
### For *buntu/Mint
##### Via ppa
```sudo apt-add-repository -y ppa:teejee2008/ppa```
```sudo apt-get update```
```sudo apt-get install conky-manager```
##### Via .deb file
[64bit]
### For Arch/Manjaro
```yaourt -S conky-manager```

##### start :
```$ conky``` or
```$ conky -d```
open conkyrc and change the parameters :
```$ sudo nano ~/.conkyrc```

### Fixing isssues with KDE
Open any ```.conkyrc``` file and replace

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
```/home/user``` directory (replace with previous ```.conky``` folder)
Open ```conky-manager``` and enable widgets


