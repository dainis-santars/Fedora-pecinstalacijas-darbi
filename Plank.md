## Lai atrisinātu problēmu ar Plank settingu nesaturēšanu, jādara sekojošais.
1. Nokopē mapi Launchers no _~/config/plank/dock1/_ uz _~/.skripti_. Datni __planksetting.dockitem__ var izlaist.
2. Iekš _~/.skripti_ ieraksta failu __plank.sh__ ar saturu:
```sh
#!/bin/bash
killall plank
cp ~/.skripti/launchers/*.dockitem ~/.config/plank/dock1/launchers/
sleep 5 && plank
```
2. Pārtaisa par izpildāmo:
`chmod +x plank.sh`
3. Iekļauj skriptu __plank.sh__ pie startējamajiem vienumiem iekš _~/config/autostart_, izveidojot datni __setplank.desktop__. Datnes saturs:
```.desktop
[Desktop Entry]
Name=SetPlank
Comment[en_US]=set Plank
Type=Application
Exec=/home/skolens/.skripti/plank.sh
NoDisplay=true
X-GNOME-Autostart-enebled=true 
```
4. Alles!
