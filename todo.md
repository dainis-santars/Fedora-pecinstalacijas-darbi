# Darbi
## Iestatījumi
### Tīkls
* Statiska IP adrese!
  - IP adrese: 192.168.250.2XX
  - Tīkla maska: 255.255.255.0
  - Vārteja: 192.168.250.1
* DNS:
  - 81.198.84.242
  - 185.122.12.242
  - 8.8.8.8

### Webmin
Lejupielāde no: [SF.net]

### Sistēmas informācija:
hostname 219kabXX, kur XX datora kārtas numurs
### Fedy
```{r, engine='bash', fedy}
bash -c 'su -c "curl http://folkswithhats.org/fedy-installer -o fedy-installer && chmod +x fedy-installer && ./fedy-installer"'
```
Iekš Fedy jāuzstāda:
* Adobe Flash
* Archive formats
* libdvdcss
* Google Chrome
* Microsoft TrueType Fonts
* Multimedia codecs
* Theme engines
* Arc Theme
* Better font rensering
* Fancy Bash prompt
* Permissive SELinux

### Panelis
```{r, engine='bash', plank}
dnf install plank
```
Lai panelis neslēpjas un rezervē sev vietu ekrānā, jārediģē */home/dainis/.config/plank/dock1/settings* datne, kur **HideMode=0**

### DropDown Teminal
```{r, engine='bash', guake}
dnf install guake
```

### Utilītas
```{r, engine='bash', dconf}
dnf install dconf-editor
```


[SF.net]: <http://www.webmin.com/download.html>
