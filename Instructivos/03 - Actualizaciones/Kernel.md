#BACKPORTS

~~~
sudo apt install -t bookworm-backports linux-image-amd64
~~~

~~~
sudo apt install -t bookworm-backports mesa-vulkan-drivers
~~~

#REMOVE KERNEL

~~~
dpkg --list | grep linux-image
~~~

~~~
sudo rm (IMAGE)
~~~
