# PS2_Backups
Instrucciones para crear una Memory Card que permita cargar copias de seguridad por USB en la Playstation 2.


1.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "FMBC.7z" descargado de este Github (o de su web oficial: https://sites.google.com/view/ysai187/home/projects/fmcbfhdb).

2.- Introducimos el pendrive en un puerto USB de la consola. Instroducir en el zocalo MC-0 una memory card que tengas con FMCB/wLaunchELF ya instalado, es requisito. Introducir en MC-1 la tarjeta que queramos crear (AVISO: se borrarán todos los datos que haya en MC-1). Encendemos la PS2.

4- Ejecutar desde MC-0 el "LaunchELF".  Navegar hasta "usb:/" y ejecutar "FMCBInstaller.elf". Click en "R1" y click en "Format MC", elegimos "Slot 2".

5.- CLick en "L1", click en "Install", click en "Slot 2", click en "Yes", click en "Cross-model". Click en "OK", click en "Exit".

6.- Apagamos la consola, extraemos el pendrive USB, extraemos la MC-0 (la anterior), y movemos la tarjeta (la nueva) de MC-1 a MC-0. Encendemos la consola, y verificamos si ha funcionado: comprobamos que arranque el menú de FMBC. Apagamos la consola.

7.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "FAT32". Descomprimimos ahi el contenido del archivo "EXTRAS.7z"

8.- Introducimos el pendrive en un puerto USB de la consola, y la encendemos. Arrancamos "LaunchELF". Navegar hasta "usb:/", nos ponemos sobre "APPS", click en "R1", click en "Copy". Navegar hasta "MC-0", click "R1" y click "Paste", click sobreescribir "Yes". Repetimos esto mismo con los directorios "BOOT", "neutrino", "POPS", "POPSTARTER" y "SYS-CONF".

9.- Apagamos la consola. Extraemos el pendrive USB. Encendemos la consola. Si todo va bien, apareceran en el menú todas las opciones.

10.- Formateamos el pendrive con sector de arranque en "MBR" y en formato "exFAT". Introducimos el pendrive en un puerto USB de la consola. Arrancamos "RiptOPL". Cuando termine de dar vueltas el circulo rojo, apagamos la consola y extraemos el pendrive USB. Con esto hemos creado en el pendrive la estructura necesaria para meter juegos.

11.- Copiamos los juegos que queramos en la carpeta "DVD" del pendrive en formato ISO (o en la carpeta CD para los juegos de PS2 en ese formato).



---------------------------------------------------------------------------------
Estructura de fabrica  de "FMCB - "v1.966 - 2019/04/13" en "Normal, cross-region":

Estructura de fábrica de "FMCB - v1.966 - 2019/04/13" en "Normal, cross-region":

mc1:/
├── APPS/
│   ├── FMCBapps.icn
│   └── icon.sys
├── BAEXEC-SYSTEM/
│   ├── osd120.elf
│   ├── osd130.elf
│   ├── osdmain.elf
│   ├── FMCB.icn
│   └── icon.sys
├── BCEXEC-SYSTEM/
│   ├── osdmain.elf
│   ├── FMCB.icn
│   └── icon.sys
├── BEEXEC-SYSTEM/
│   ├── osd130.elf
│   ├── osdmain.elf
│   ├── FMCB.icn
│   └── icon.sys
├── BIEXEC-SYSTEM/
│   ├── osd110.elf
│   ├── osd130.elf
│   ├── osdmain.elf
│   ├── osdsys.elf
│   ├── atad.irx
│   ├── dev9.irx
│   ├── FMCB.icn
│   ├── hddload.irx
│   └── icon.sys
├── BOOT/
│   ├── BOOT.ELF
│   ├── BOOT.icn
│   └── icon.sys
└── SYS-CONF/
    ├── FMCB_CFG.ELF
    ├── endvdpl.irx
    ├── FREEMCB.CNF
    ├── icon.sys
    ├── sysconf.icn
    ├── USBD.IRX
    └── USBHDFSD.IRX
