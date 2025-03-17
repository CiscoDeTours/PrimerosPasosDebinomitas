# Add efi entry

• Ingresar a la ruta

~~~
cd /etc/grub.d/proxifiedScripts
~~~

• Modificar el archivo

~~~
sudo nano uefi-firmware
~~~

• Agregar -- class efi justo después de '$LABEL' y antes de \menuentry
