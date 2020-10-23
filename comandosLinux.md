# **comandos de linux utilies**

- **cambiar nombre de maquina**: sudo nano /etc/hostname
- **añadir usuario sudoer**: sudo adduser XXX ; sudo addgroup XXX sudo
- **ip a** : ver la ip de la maquina 
- **ip route** : ver la tabla de rutas
- **ss -ltnp** : ver puertos abiertos
- **exportar display con sudo o su** sudo touch /root/.Xauthority y sudo xauth add $(xauth -f ~clase/.Xauthority list| tail -1)
- **ccambiar configuracion red**:  sudo nano /etc/netplan/00-installer-config.yaml , sudo netplan apply, 
- **reiniciar red**: sudo systemctl restart systemd-networkd
- **comandos basicos iptables nat**: sudo iptables -P FORWARD ACCEPT , sudo iptables -t nat -A POSTROUTING -o enp0s3 -j MASQUERADE
- **router linux** sysctl -w net.ipv4.ip_forward=1 , permanente editar net.ipv4.ip_forward = 1  en /etc/sysctl.conf y reiniciar sysctl -p /etc/sysctl.conf
- **renew ip de un dhcp**: sudo dhclient -v
- **Ver el dns server**: sudo systemd-resolve --status , cat /etc/resolv.conf
- **Ver log servicios**: sudo journalctl -u isc-dhcp-server



