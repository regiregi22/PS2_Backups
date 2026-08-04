# PS2_Backups
Instrucciones para crear una Memory Card que permita cargar copias de seguridad por USB en la Playstation 2.


1.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "XXXXXXXX.7z" descargado de este Github.

2.- Introducimos el pendrive en un puerto USB de ls PS2. Instroducir en el zocalo MC-0 una memory card que tengas ya con FMCB/wLaunchELF. Introducir en MC-1 la tarjeta que queramos crear (AVISO: se borrarán todos los datos que haya en MC-1).

3-. Ejecutar desde MC-0 el "wLaunchELF". Navegar hasta "usb:/MCA/mca_new/", ejecutar "mca.elf". Elegimos "slot 2" (la MC-1), "Format Full", elegimos "8Mb" y "Yes". Reiniciamos.

4- Ejecutar desde MC-0 el "wLaunchELF".  Navegar hasta "usb:/FMCB/", ejecutar "FMCBInstaller.elf".
