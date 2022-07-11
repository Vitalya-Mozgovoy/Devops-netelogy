# Домашнее задание к занятию "3.9. Элементы безопасности информационных систем"  
1.Установите Bitwarden плагин для браузера. Зарегестрируйтесь и сохраните несколько паролей.  
Ответ: [скриншот](https://drive.google.com/file/d/1QhrNREA-wMRdFo2dC6-EzdYUOHUspDkE/view?usp=sharing)

2. Установите Google authenticator на мобильный телефон.  
Настройте вход в Bitwarden акаунт через Google authenticator OTP.  
Ответ: [скриншот](https://drive.google.com/file/d/1wyy490afE3RF-Yr7VP02PfzDj1VGHLxP/view?usp=sharing)   
3. Установите apache2, сгенерируйте самоподписанный сертификат, настройте тестовый сайт для работы по HTTPS.  
Ответ: [скриншот ](https://drive.google.com/file/d/1yV_yWK0yMDSHYw5HQupBVoIigHFpvuiN/view?usp=sharing)  
[скрин_2](https://drive.google.com/file/d/1Ig2zVbkOQxSCYiaZLAfgKJZSxDltjr0M/view?usp=sharing)  

4. Проверьте на TLS уязвимости произвольный сайт в интернете (кроме сайтов МВД, ФСБ, МинОбр, НацБанк, РосКосмос,  
РосАтом, РосНАНО и любых госкомпаний, объектов КИИ, ВПК ... и тому подобное).
Ответ: [скриншот ](https://drive.google.com/file/d/1maW8MmbSGhttIrJQKyd2alNiR1jyy_Ok/view?usp=sharing)
5. Установите на Ubuntu ssh сервер, сгенерируйте новый приватный ключ. Скопируйте свой публичный ключ   
на другой сервер. Подключитесь к серверу по SSH-ключу.
Ответ: [скриншот](https://drive.google.com/file/d/1bKemP-gr0iAF2w7TdGEbB24qNq3xRFIR/view?usp=sharing)  
6. Переименуйте файлы ключей из задания 5. Настройте файл конфигурации SSH клиента,  
так чтобы вход на удаленный сервер осуществлялся по имени сервера.  
Ответ:   
vagrant@netologyVM1:~$ sudo mv ~/.ssh/id_rsa ~/.ssh/id_rsa_netology  
vagrant@netologyVM1:~$ sudo nano ~/.ssh/config  
Host netologyVM2  
                HostName 172.28.128.60      
                User vagrant     
                Port 22   
                IdentityFile ~/.ssh/id_rsa_netology  
                vagrant@netologyVM1:~$ ssh netologyVM2  
                Welcome to Ubuntu 20.04.2 LTS (GNU/Linux 5.4.0-80-generic x86_64)  
                ....  
                vagrant@netologyVM2:~$  
7. Соберите дамп трафика утилитой tcpdump в формате pcap, 100 пакетов. Откройте файл pcap в Wireshark.  
Ответ:  
tcpdump -nnei any -c 100 -w 100packets.pcap  
tcpdump: listening on any, link-type LINUX_SLL (Linux cooked v1), capture size 262144 bytes  
100 packets captured  
178 packets received by filter  
0 packets dropped by kernel  
[скрин](https://drive.google.com/file/d/1eOd44Y4N48e3dTLzDHAh4OlnE2-dR7GU/view?usp=sharing)   


