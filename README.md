# ~~Big Sur Dynamic Wallpaper on Linux~~

# Big Sur Dynamic Wallpaper on Ubuntu

The world of open source may seem intimidating, but there’s more to it than meets the eye. Customizing your Linux system may seem like a daunting task at first, but with these simple steps, you will be up and running in no time.

MacOS Big Sur has a breathtaking dynamic wallpaper and there’s no reason for someone to not enjoy them.

Here’s how to get macOS Big Sur-like dynamic wallpaper on your Gnome desktop.

# Installation for Ubuntu
### Material required:
> 1. Ubuntu Desktop.  
> 2. Internet connection.

### .xml files
- focal.xml (Ubuntu 20.04)
- groovy.xml (Ubuntu 20.10)
- f33.xml (Fedora 33 from Maxmud Fayziev)

### 1. Clone the resource
```
cd ~/Pictures
git clone https://github.com/eallion/Big-Sur-Ubuntu.git
```

### 2. Change the file path
My username is `eallion`, you must change `eallion` to your username in .xml file.
If you are`alex`, you can change it in the terminal:
```
cd Big-Sur-Ubuntu
sed -i "s/eallion/alex/g" focal.xml
```
or change it in a text editer.
```
<file>/home/eallion/Pictures/Big-Sur-Ubuntu/Night.jpg</file>
```

### 3. Setting
> Two ways, change one.

- 3.1 Setting with gnome tweaks:

```
gnome-tweaks
```
Go to the `Appearance` section and under `Backgrounds`, select the XML file.  
Also set the Adjustment to `ZOOM`.

- 3.2 Setting in system settings:

```
cd ~/Pictures/Big-Sur-Ubuntu/
sudo mv /usr/share/backgrounds/contest/focal.xml /usr/share/backgrounds/contest/focal.xml.bak
sudo cp focal.xml /usr/share/backgrounds/contest/focal.xml
```
Open the system settings, go to the `Backgrouds` section.  
Choose the picture with a clock icon.

### 4. Reboot
```
reboot
```

### 5. Notice
You should change the file path in `focal.xml`:
```
<file>/home/eallion/Pictures/Big-Sur-Ubuntu/Night.jpg</file>
```

# Installation for other Linux Gnome desktop (Untested)

### Material required:

> 1. A Linux system with Gnome GUI.  
> 2. Internet connection.  
> 3. Familiarity with the Linux distro.  

1. Open up the terminal.
3. Then run `sudo apt-get update`.
3. Next run `sudo apt get gnome-tweaks`. This is the tool you will use to set the dynamic wallpaper later.
4. Next, download or clone the wallpapers from this GitHub repository.
5. Next, extract the folder onto your Pictures folder. Keep in mind that the XML file is hard coded. Thus if you change the image name, you must make the required changes in the XML file.
6. Open the XML using any word processor and replace the file path.
7. Lastly, open Gnome Tweak Tools go to the `Appearance` section and under `Backgrounds`, select the XML file. Also set the Adjustment to `ZOOM`.

**Voilà enjoy your beautiful desktop.**
