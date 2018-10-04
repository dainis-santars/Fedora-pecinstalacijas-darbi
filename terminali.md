# Termināļi
## Smuks Gnome Terminal

1. `sudo dnf install powerline powerline-fonts`
2. `gedit ~/.bashrc`
3. Pievieno sekojošu bloku:
```
if [ -f `which powerline-daemon` ]; then
  powerline-daemon -q
  POWERLINE_BASH_CONTINUATION=1
  POWERLINE_BASH_SELECT=1
  . /usr/share/powerline/bash/powerline.sh
fi
```
Būs:

![smuki](https://fedoramagazine.org/wp-content/uploads/2015/08/Screenshot-from-2015-08-28-10-34-25.png)
