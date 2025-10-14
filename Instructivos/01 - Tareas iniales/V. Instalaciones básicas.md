# Instalaciones básicas

> **Enfoque:**
> <p> <p>
>  
> Se reserva la paquetería nativa para aquello que está íntimamente conexo al Sistema


#### V.1 - Utilidades de consola

• Para Android:

~~~
sudo apt install adb fastboot -y
~~~

• Para descargar archivos de repositorios en línea:

~~~
sudo apt install git wget -y
~~~

• Para mover archivos descargados:

~~~
sudo apt install rsync -y
~~~

• Para agregar soporte RAR:

~~~
sudo apt install unrar -y
~~~

• Fuentes de Microsoft:
~~~
sudo apt install ttf-mscorefonts-installer
~~~

#### V.2 - Herramientas

• Para gestionar particiones:

~~~
sudo apt install gparted -y
~~~

• Para crear puntos de restauración:

~~~
sudo apt install timeshift -y
~~~

• Para virtualizaciones:

~~~
sudo apt install gnome-boxes -y
~~~


## Recomendaciones

#### R.V.1 - Quitar software preinstalado poco utilizado

~~~
sudo apt remove aisleriot debian-reference-common evolution five-or-more four-in-a-row hdate-applet hitori iagno im-config gnome-2048 gnome-chess gnome-contacts gnome-klotski gnome-mahjongg gnome-maps gnome-mines gnome-nibbles gnome-robots gnome-sudoku gnome-taquin gnome-tetravex gnome-weather goldendict kasumi lightsoff malcontent mlterm-common mozc-utils-gui quadrapassel rhythmbox shotwell swell-foop tali thunderbird transmission-gtk xiterm+thai yelp 
~~~

> **Nota:**
> <p> <p>
>  
> El siguiente comando opera como una herramienta de limpieza

~~~
sudo apt autoremove 
~~~
