## Ja MOC (mocp) nevar piešķilt
Iemesls:
* kļūda FATAL_ERROR: TiMidity-Plugin: Error processing TiMidity-Configuration!
* kļūda FATAL_ERROR: Configuration file is not secure: /home/dainis/.moc/config

Jādara sekojošais:
1. ~~Maina direktoriju `cd /etc/popt.d`~~
2. ~~Uztaisa tukšu failu `sudo touch tukshs`~~
3. Sakopē vecās mašīnas .moc direktoriju jaunajā. Socket2 fails jāizlaiž.
4. Maina direktoriju `cd`, `cd .moc`
5. ~~Ar :punch: root tiesībām uztaisa config datni `sudo touch config` un tajā ievada noteikumu `TiMidity_Config = /etc/timidity.cfg`~~
6. Atver `config` failu un labo esošo saturu uz `TiMidity_Config = no`
7. `config` failam noņem atļaujas uz rakstīšanu grupai un pārējiem
