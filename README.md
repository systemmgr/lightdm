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
sudo git clone https://github.com/systemmgr/lightdm "/usr/local/etc/lightdm"
```  
  
<p align=center>
  <a href="https://wiki.archlinux.org/index.php/LightDM" target="_blank">LightDM wiki</a>  |  
  <a href="https://github.com/canonical/lightdm/" target="_blank">LightDM site</a>
</p>  
    
