[Learncodethehardway](http://cli.learncodethehardway.org/book/)
---

xclip for copying into clipboard
---
To install: sudo apt-get install xclip

```xclip id_rsa.pub``` should copy the content into primary selection. To copy into clipboard, follow the command with ```xclip -o | xclip -sel clip```



[using apt-get](http://www.tecmint.com/useful-basic-commands-of-apt-get-and-apt-cache-for-package-management/)
---

[how to use update-alternatives]()
---



##### Search packages
```apt-cache policy <package-name>```
More useful commands using [apt-get](http://www.tecmint.com/useful-basic-commands-of-apt-get-and-apt-cache-for-package-management/)

##### Installing package

  __Using apt-get__

   ```sudo apt-get install package-name```
  
  __Using .tar.xz file__

   1. download .tar.xz file.
   2. 

__Using .deb file__

1. download .deb file.
2. run command ```sudo dpkg i <file.deb>```
3. if errors outs due to dependencies, run command ```sudo apt-get install -f``` and rerun step 2.
 

##### Install package with specific version

```sudo apt-get install packagename=2.3.5```


##### Installing Eclipse
1. Download eclipse(*.tar.gz) from its [website](http://www.eclipse.org/downloads/)
2. Make sure you have java installed]()
3. Extract eclipse*.tar.gz into /opt
```cd /opt && tar -zxvfw ~/Downloads/eclipse*.tar.gz```
4. Create launcher shortcut for eclipse, create eclipse.desktop file in /usr/share/applications or ~/.local/share/applications and add following contents.
```
[Desktop Entry]
Name=Eclipse 4
Type=Application
Exec=/opt/eclipse/eclipse
Terminal=false
Icon=/opt/eclipse/icon.xpm
Comment=Integrated Development Environment
NoDisplay=false
Categories=Development;IDE;
Name[en]=Eclipse
```   
5. create symbolic link to open an eclipse from command line
```
 sudo ln -s /opt/eclipse/eclipse /usr/bin
```
or use update-alternatives
```
sudo update-alternatives --install /usr/bin/eclipse eclipse /opt/eclipse/eclipse
```
     
##### [Installing nodejs](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions).

##### [Installing java]()

#####[Where are package installed](http://www.howtogeek.com/howto/ubuntu/see-where-a-package-is-installed-on-ubuntu/)
