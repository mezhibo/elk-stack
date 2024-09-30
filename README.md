
**Задание 1**

Вам необходимо поднять в докере и связать между собой:

 - elasticsearch (hot и warm ноды);

 - logstash;

 - kibana;

 - filebeat.

Logstash следует сконфигурировать для приёма по tcp json-сообщений.

Filebeat следует сконфигурировать для отправки логов docker вашей системы в logstash.

В директории help находится манифест docker-compose и конфигурации filebeat/logstash для быстрого выполнения этого задания.

Результатом выполнения задания должны быть:

 - скриншот docker ps через 5 минут после старта всех контейнеров (их должно быть 5);

 - скриншот интерфейса kibana;

 - docker-compose манифест (если вы не использовали директорию help);

 - ваши yml-конфигурации для стека (если вы не использовали директорию help).



**Решение 1**

Выполнял ДЗ с использованием директории Help


Запускаем докер-коспос файл, и видм что все необходимые контейнеры у нас запустились

![alt text](https://github.com/mezhibo/elk-stack/blob/3be49a71854c558058a4dee17af20abba780b90b/IMG/1.jpg)


Проверяем доступность источников данных через консоль 


![alt text](https://github.com/mezhibo/elk-stack/blob/3be49a71854c558058a4dee17af20abba780b90b/IMG/2.jpg)




**Задание 2**

Перейдите в меню создания index-patterns в kibana и создайте несколько index-patterns из имеющихся.

Перейдите в меню просмотра логов в kibana (Discover) и самостоятельно изучите, как отображаются логи и как производить поиск по логам.

В манифесте директории help также приведенно dummy-приложение, которое генерирует рандомные события в stdout-контейнера. Эти логи должны порождать индекс logstash-* в elasticsearch. Если этого индекса нет — воспользуйтесь советами и источниками из раздела «Дополнительные ссылки» этого задания.



**Решение 2**


Создал index-patterns из logstash


![alt text](https://github.com/mezhibo/elk-stack/blob/3be49a71854c558058a4dee17af20abba780b90b/IMG/3.jpg)
