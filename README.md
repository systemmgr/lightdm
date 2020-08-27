## lightdm  
  
LightDM is a cross-desktop display manager  
  
requires:    
apt: ```apt install lightdm lightdm-gtk-greeter-settings```  
yum: ```yum install lightdm lightdm-gtk-greeter-settings```  
pacman: ```pacman -S lightdm lightdm-gtk-greeter-settings```  
  
Automatic install/update:
```
sudo bash -c "$(curl -LSs https://github.com/systemmgr/lightdm/raw/master/install.sh)"
```
Manual install:
```
sudo bash -c " 
git clone https://github.com/systemmgr/lightdm "/usr/local/etc/lightdm"
if [ -d /usr/share/lightdm-gtk-greeter-settings ]; then
  LIGHTDMG=/usr/share/lightdm-gtk-greeter-settings
elif [ -d /usr/share/lightdm-gtk-greeter ]; then
  LIGHTDMG=/usr/share/lightdm-gtk-greeter
else
  LIGHTDMG=/usr/share/lightdm/lightdm-gtk-greeter.conf.d
fi

if [ -d /etc/lightdm ]; then
  cp -Rf $APPDIR/etc/* /etc/lightdm/
  cp -Rf $APPDIR/share/lightdm/* /usr/share/lightdm/
  cp -R $APPDIR/share/lightdm-gtk-greeter-settings/* $LIGHTDMG/lightdm-gtk-greeter.conf.d
fi
"
```  
  
<p align=center>
  <a href="https://wiki.archlinux.org/index.php/LightDM" target="_blank">LightDM wiki</a>  |  
  <a href="https://github.com/canonical/lightdm/" target="_blank">LightDM site</a>
</p>  
    
