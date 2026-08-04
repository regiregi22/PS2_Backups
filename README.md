# PS2_Backups
Instrucciones para crear una Memory Card que permita cargar copias de seguridad por USB en la Playstation 2.


1.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "FMBC.7z" descargado de este Github (o de su web oficial: https://sites.google.com/view/ysai187/home/projects/fmcbfhdb).

2.- Introducimos el pendrive en un puerto USB de ls PS2. Instroducir en el zocalo MC-0 una memory card que tengas ya con FMCB/wLaunchELF. Introducir en MC-1 la tarjeta que queramos crear (AVISO: se borrarán todos los datos que haya en MC-1). Encendemos la PS2.

4- Ejecutar desde MC-0 el "wLaunchELF".  Navegar hasta "usb:/" y ejecutar "FMCBInstaller.elf". Click en "R1" y click en "Format MC", elegimos "Slot 2".

5.- CLick en "L1", click en "Install", click en "Slot 2", click en "Yes", click en "Cross-model"



