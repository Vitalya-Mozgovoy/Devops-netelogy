Задание №1 
1. Опишите своими словами основные преимущества применения на практике IaaC паттернов.
Ответ:
Непрерывная интеграция позволяет быстро находить ошибки в коде за счет постоянного тестирования небольшими объемами.
Непрерывная доставка также позволяет легко исправить или откатиться на недавнее состояние в случае ошибок.
2. Какой из принципов IaaC является основополагающим?
Ответ: 
Идемпоте́нтность-Получение стабильного и предсказуемого результата каждый раз при использовании(запуске) кода.

Задание №2

1. Чем Ansible выгодно отличается от других систем управление конфигурациями?
Ответ:
Его основные преимущества это использование SSH инфраструктуры без установки дополнительного окружения, 
а также наличие большого количества модулей.
2. Какой, на ваш взгляд, метод работы систем конфигурации более надёжный push или pull?
Ответ: 
На мой взгляд более надежный метод push В этом режиме конфигурация серверу отправляется управляющим сервером. 
Задание №3

F:\Netelogy>vagrant --version      
Vagrant 2.2.19

iva@c8:~/Documents/netology/devops-netology/DevVirt/05-virt-02-iaac  (05-virt-02-iaac *)$ ansible --version
[DEPRECATION WARNING]: Ansible will require Python 3.8 or newer on the controller starting with Ansible 2.12. Current version: 3.6.8 (default, Sep 10 2021, 09:13:53) [GCC 8.5.0 20210514 (Red Hat 8.5.0-3)]. This feature will be removed from ansible-core in version 2.12. Deprecation
 warnings can be disabled by setting deprecation_warnings=False in ansible.cfg.
ansible [core 2.11.7] 
  config file = None
  configured module search path = ['/home/iva/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /home/iva/.local/lib/python3.6/site-packages/ansible
  ansible collection location = /home/iva/.ansible/collections:/usr/share/ansible/collections
  executable location = /home/iva/.local/bin/ansible
  python version = 3.6.8 (default, Sep 10 2021, 09:13:53) [GCC 8.5.0 20210514 (Red Hat 8.5.0-3)]
  jinja version = 3.0.3
  libyaml = True
