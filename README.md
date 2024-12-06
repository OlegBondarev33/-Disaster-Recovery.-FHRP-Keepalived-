# Домашнее задание к занятию «Disaster Recovery. FHRP и Keepalived» - Бондарев Олег`




### Задание 1

Что нужно сделать:

1. Дана схема для Cisco Packet Tracer, рассматриваемая в лекции.
2. На данной схеме уже настроено отслеживание интерфейсов маршрутизаторов Gi0/1 (для нулевой группы)
3. Необходимо аналогично настроить отслеживание состояния интерфейсов Gi0/0 (для первой группы).
4. Для проверки корректности настройки, разорвите один из кабелей между одним из маршрутизаторов и Switch0 и запустите ping между PC0 и Server0.
5. На проверку отправьте получившуюся схему в формате pkt и скриншот, где виден процесс настройки маршрутизатора.

![image](https://github.com/user-attachments/assets/5d99425d-31b1-478e-ad61-ac71d451e6d2)
![image](https://github.com/user-attachments/assets/5e262545-5c78-456f-ada5-1882c479d090)


### Задание 2

Что нужно сделать:

1. Запустите две виртуальные машины Linux, установите и настройте сервис Keepalived как в лекции, используя пример конфигурационного файла.
2. Настройте любой веб-сервер (например, nginx или simple python server) на двух виртуальных машинах
3. Напишите Bash-скрипт, который будет проверять доступность порта данного веб-сервера и существование файла index.html в root-директории данного веб-сервера.
4. Настройте Keepalived так, чтобы он запускал данный скрипт каждые 3 секунды и переносил виртуальный IP на другой сервер, если bash-скрипт завершался с кодом, отличным от нуля (то есть порт веб-сервера был недоступен или отсутствовал index.html). Используйте для этого секцию vrrp_script
5. На проверку отправьте получившейся bash-скрипт и конфигурационный файл keepalived, а также скриншот с демонстрацией переезда плавающего ip на другой сервер в случае недоступности порта или файла index.html

![image](https://github.com/user-attachments/assets/eed090dd-40c9-4253-b57b-bede86e4cbfd)
![image](https://github.com/user-attachments/assets/e3d18b21-8be9-4743-8521-c9bde903be45)
![image](https://github.com/user-attachments/assets/64103edb-c15e-4bd9-87c4-2f1461214fbb)
![image](https://github.com/user-attachments/assets/95d874b5-1532-4103-a6fa-d4d057266d6e)
![image](https://github.com/user-attachments/assets/68881d10-3594-4757-beea-127fa63dc563)
![image](https://github.com/user-attachments/assets/59a7a73b-b25e-420e-8341-890257ab49b6)
![image](https://github.com/user-attachments/assets/74a548d9-1c51-4c44-b00c-0bbec7569f97)

https://github.com/OlegBondarev33/-Disaster-Recovery.-FHRP-Keepalived-/blob/main/port
