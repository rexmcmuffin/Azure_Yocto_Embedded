# Lista de comandos necesarios durante el taller

Este es el contenido introductorio del documento. Aquí puedes agregar una descripción general o un resumen.

## SSH

En powershell se debera de ejecutar el comando de 

ssh username@ip

reemplazando el username por el generado en el paso 10 y la direccion ip que se detalla en el paso 13


## Creacion del escritorio remoto por medio de xrdp

Se contiene la lista de comandos para instalar y configurar xrdp.

1. sudo apt update
2. sudo apt install xfce4 xfce4-goodies -y
3. sudo apt install xrdp -y
4. sudo systemctl status xrdp
Si el estado no es running ejecutar este comando
	4.1. sudo systemctl start xrdp
5. echo "xfce4-session" | tee .xsession
6. sudo systemctl restart xrdp
7. sudo ufw allow from ip/32 to any port 3389
8. sudo ufw status

## Instalacion de Yocto en la VM por medio de xrdp. 

