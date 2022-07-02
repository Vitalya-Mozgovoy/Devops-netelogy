# Домашнее задание к занятию "3.6. Компьютерные сети, лекция 1"
1.Работа c HTTP через телнет.
Подключитесь утилитой телнет к сайту stackoverflow.com telnet stackoverflow.com 80
отправьте HTTP запрос  

``GET /questions HTTP/1.0 
HOST: stackoverflow.com
[press enter]   
[press enter]`   ``

В ответе укажите полученный HTTP код, что он означает?  

Ответ: на сайт mail.ru Получили код 301 редирект с http на https [скриншот ](https://drive.google.com/file/d/1Uz2F89E4k0jpMa7gmdpCIA6Ti0i-G1gK/view?usp=sharing)

2.Повторите задание 1 в браузере, используя консоль разработчика F12.  

откройте вкладку Network  
отправьте запрос http://mail.ru  
найдите первый ответ HTTP сервера, откройте вкладку Headers  
укажите в ответе полученный HTTP код.  
проверьте время загрузки страницы, какой запрос обрабатывался дольше всего?  
приложите скриншот консоли браузера в ответ.  

Ответ: [скриншот ](https://drive.google.com/file/d/1b5MI70pjy5cnwpeKDE4Vqof7NdzbJh6L/view?usp=sharing)
HTTP код 200 время загрузки 357.11 мс долше всего обрабатывался запрос к картинке 561 мс

3.Какой IP адрес у вас в интернете?
Ответ: `dig resolver4.opendns.com myip.opendns.com +short`
208.67.X.X

4.Какому провайдеру принадлежит ваш IP адрес? Какой автономной системе AS? Воспользуйтесь утилитой whois  

Ответ: `vagrant@vagrant:~$ whois  208.67.x.x | grep ^descr
descr:          DSL access network in  Moscow region
descr:          Rostelecom networks`

`vagrant@vagrant:~$ whois  208.67.X.X | grep ^origin
origin:         AS12389`  

5. Через какие сети проходит пакет, отправленный с вашего компьютера на адрес 8.8.8.8? Через какие AS?  
Воспользуйтесь утилитой traceroute  
Ответ:` vagrant@vagrant:~$ traceroute -An 8.8.8.8
traceroute to 8.8.8.8 (8.8.8.8), 30 hops max, 60 byte packets
 1  10.0.2.2 [*]  13.999 ms  0.554 ms  0.270 ms
 2  10.0.2.2 [*]  10.160 ms  9.844 ms  9.892 ms`

6. Повторите задание 5 в утилите mtr. На каком участке наибольшая задержка - delay?
Ответ  [скриншот ](https://drive.google.com/file/d/1iXH5eDwIwn-TCEQMu294G0f99LcpBoPp/view?usp=sharing)
Задержка на 8 ходе 
7. Какие DNS сервера отвечают за доменное имя dns.google? Какие A записи? воспользуйтесь утилитой dig
Ответ: [скриншот](https://drive.google.com/file/d/1B2f__E-QdWdsHLUer6fpOcbil8gBVzFC/view?usp=sharing) 
8. Проверьте PTR записи для IP адресов из задания 7. Какое доменное имя привязано к IP? воспользуйтесь утилитой dig
Ответ: [скриншот](https://drive.google.com/file/d/1ScUIMM7i0_7-qkF-lL2XNFPrLw1H7dKx/view?usp=sharing) 
