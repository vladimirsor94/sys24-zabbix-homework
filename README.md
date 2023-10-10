# Домашнее задание к занятию "`Zabbix part1 `" - `Sorokin VV`


### Задание 1

1. `sudo apt install postgresql - установка Postgresql`
2. `dpkg -i zabbix-release_6.4-1+debian11_all.deb
    apt update
    apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-scripts - установка забикс сервера`
3. `systemctl restart zabbix-server apache2
    systemctl enable zabbix-server apache2 - перезапуск и автозагрузка сервера`

![face](https://github.com/vladimirsor94/sys24-zabbix-homework/blob/vladimirsor94-patch-1/face.png

---

### Задание 2

`Установка заббикс агента, ребут и включение автозагрузки
sudo apt install zabbix-agent
systemctl restart zabbix-agent
systemctl enable zabbix-agent

Настройка подключения агента к серверу ( разрешаем нашим хостам подключится прописывая их ip)
sed -i 's/Server=127.0.0.1/Server=192.168.1.32/g' /etc/zabbix/zabbix_agent.conf

sed -i 's/Server=127.0.0.1/Server=192.168.1.33/g' /etc/zabbix/zabbix_agent.con`

![2hosts](https://github.com/vladimirsor94/sys24-zabbix-homework/blob/vladimirsor94-patch-1/2%20hosts.png
![latest](https://github.com//sys24-zabbix-homework/blob/vladimirsor94-patch-1/latest.png
