### 

#### I.1 - Desactivar actualizaciones automáticas

~~~
gsettings set org.gnome.software download-updates false
~~~

#### I.2 - Nativa

• Listar actualizaciones disponibles

~~~
apt list --upgradable
~~~

• Instalar actualizaciones

~~~
sudo apt upgrade -y
~~~

#### I.3 - Flatpak

• Ver actualizaciones disponibles

~~~
flatpak remote-ls --updates
~~~

• Instalar actualizaciones

~~~
sudo apt upgrade -y
~~~

~~~
sudo sed -i 's/bookworm/stable/g' /etc/apt/sources.list
~~~

> **Advertencia:**
> <p> <p>
>  
> Para pegar este comando con la extraña configuración que en ciertos casos está habilitada por defecto debe pulsarse el touchpad con dos dedos al mismo tiempo. De persistir problemas, es recomendable usar un mouse

