## 🔐 Настройка SSH-доступа между виртуальными машинами


| Устройство         | IP-адрес        |
| ----------         | --------------- |
| Kali               | 192.168.50.30 |
| Debian1 (machine1) | 192.168.50.10 |
| Debian2 (machine2) | 192.168.50.20 |


## 1) Подключение с Kali к Debian1
```bash
sudo ip addr add 192.168.50.30/24 dev eth1
sudo ip link set eth1 up
ssh machine1@192.168.50.10
```
<p align="center"> <img src="2.debian1-ssh.png" width="900"> </p>
