# **comandos de linux utilies**

- **ip a** : ver la ip de la maquina 
- **ip route** : ver la tabla de rutas
- **ss -ltnp** : ver puertos abiertos
- **exportar display con sudo o su** sudo touch /root/.Xauthority y sudo xauth add $(xauth -f ~clase/.Xauthority list| tail -1)
- **ccambiar configuracion red**:  sudo nano /etc/netplan/00-installer-config.yaml , sudo netplan apply, sudo systemctl restart systemd-networkd


