# PS2_Backups
Instrucciones para crear una Memory Card que permita cargar copias de seguridad por USB en la Playstation 2.


1.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "FMBC.7z" descargado de este Github (o de su web oficial: https://sites.google.com/view/ysai187/home/projects/fmcbfhdb).

2.- Introducimos el pendrive en un puerto USB de la consola. Instroducir en el zocalo MC-0 una memory card que tengas con FMCB/wLaunchELF ya instalado, es requisito. Introducir en MC-1 la tarjeta que queramos crear (AVISO: se borrarán todos los datos que haya en MC-1). Encendemos la PS2.

4- Ejecutar desde MC-0 el "LaunchELF".  Navegar hasta "usb:/" y ejecutar "FMCBInstaller.elf". Click en "R1" y click en "Format MC", elegimos "Slot 2".

5.- CLick en "L1", click en "Install", click en "Slot 2", click en "Yes", click en "Cross-model". Click en "OK", click en "Exit".

6.- Apagamos la consola, extraemos el pendrive USB, extraemos la MC-0 (la anterior), y movemos la tarjeta (la nueva) de MC-1 a MC-0. Encendemos la consola, y verificamos si ha funcionado: comprobamos que arranque el menú de FMBC. Apagamos la consola.

7.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "EXTRAS.7z"

8.- Introducimos el pendrive en un puerto USB de la consola, y la encendemos. Arrancamos "LaunchELF". Navegar hasta "usb:/", nos ponemos sobre "APPS", click en "R1", click en "Copy". Navegar hasta "MC-0", click "R1" y click "Paste", click sobreescribir "Yes". Repetimos esto mismo con los directorios "BOOT", "neutrino", "POPS", "POPSTARTER" y "SYS-CONF".
