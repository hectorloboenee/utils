## Steps

1. Disabled Wasyland by uncommenting ```WaylandEnable=false``` in the ```/etc/gdm3/custom.conf```
2. Add ```QT_QPA_PLATFORM=xcb``` in ```/etc/environment```
3. Check whether you are on Wayland or Xorg using: ```echo QT_QPA_PLATFORM=xcb```

sudo apt-get install acpi
watch --interval=5 acpi -V
