### Домашнее задание к занятию "3.8. Компьютерные сети, лекция 3"   

1. Создайте dummy0 интерфейс в Ubuntu. Добавьте несколько статических маршрутов. Проверьте таблицу маршрутизации.  
Ответ: Запускаем модуль Настройка интерфейса через `systemd ` Добавлен маршрут, конфигурация через `netplan`  
[скриншот_1 ](https://drive.google.com/file/d/1WUBvmcOBXq7RtZkz-um5vnBnMiudQIwN/view?usp=sharing)
[скриншот_2](https://drive.google.com/file/d/13v8qW4dPFM18hsziIsqLuKDdp5evtnbl/view?usp=sharing)
[скриншот_3 ](https://drive.google.com/file/d/19hl7Et8aewTCHFh5_bSBQRaMP6Jy1hJj/view?usp=sharing)
2. Проверьте открытые TCP порты в Ubuntu, какие протоколы и приложения используют эти порты?  
Приведите несколько примеров.  
Ответ: Порты TCP [скриншот_4](https://drive.google.com/file/d/1nY0nTrOKsgbfGxvoPpUotjI_inEf4ENZ/view?usp=sharing)  

53 порт - это DNS.  

22 порт - это SSH.  
3. Проверьте используемые UDP сокеты в Ubuntu, какие протоколы и приложения используют эти порты?  
Ответ: Порты UDP   
[скриншот_5](https://drive.google.com/file/d/1xyTUL-_HIe60qxyo8OCNLejmK4DLVQ7Q/view?usp=sharing)   
  53 порт - так же DNS.  
    68 порт использует DHCP для отправки сообщений клиентам.  
4. Используя diagrams.net, создайте L3 диаграмму вашей домашней сети или любой другой сети, с которой вы работали.  
Ответ: [скриншот](https://drive.google.com/file/d/13yba8d-UDb3WwU1a_nNQpCPZAlRtHga3/view?usp=sharing) 