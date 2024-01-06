Домашнее задание к занятию «Система мониторинга Zabbix. Часть 2» Тихун Вадим 
В практике есть 4 основных и 5 дополнительных (со звездочкой) заданий. Основные задания нужно выполнять обязательно, со звездочкой - по желанию и его решение никак не повлияет на получение вами зачета по этому домашнему заданию, при этом вы сможете глубже и/или шире разобраться в материале.

Пожалуйста, присылайте на проверку все задачи сразу. Любые вопросы по решению задавайте в чате учебной группы.

Цели задания
Научитья создавать свои шаблоны в Zabbix, добавлять в Zabbix хосты и связывать шаблон с хостами
Научиться составлять кастомный дашборд
Научиться создавать UserParameter на Bash
Научиться создавать Python-скрип, добавляться в него UserParameter и прикреплять к шаблону
Научиться создавать Vagrant-скрипты для Zabbix Agent
Чеклист готовности к домашнему заданию
 Просмотрите в личном кабинете занятие "Система мониторинга Zabbix. Часть 2"
Инструкция по выполнению домашнего задания
Сделайте fork репозитория c шаблоном решения к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw).
Выполните клонирование этого репозитория к себе на ПК с помощью команды git clone.
Выполните домашнее задание и заполните у себя локально этот файл README.md:
впишите вверху название занятия и ваши фамилию и имя;
в каждом задании добавьте решение в требуемом виде: текст/код/скриншоты/ссылка;
для корректного добавления скриншотов воспользуйтесь инструкцией «Как вставить скриншот в шаблон с решением»;
при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в инструкции по MarkDown.
После завершения работы над домашним заданием сделайте коммит (git commit -m "comment") и отправьте его на Github (git push origin).
Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
Любые вопросы задавайте в чате учебной группы и/или в разделе «Вопросы по заданию» в личном кабинете.












Задание 1
Создайте свой шаблон, в котором будут элементы данных, мониторящие загрузку CPU и RAM хоста.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
В веб-интерфейсе Zabbix Servera в разделе Templates создайте новый шаблон
Создайте Item который будет собирать информацию об загрузке CPU в процентах
Создайте Item который будет собирать информацию об загрузке RAM в процентах
Требования к результату
 Прикрепите в файл README.md скриншот страницы шаблона с названием «Задание 1»




 
 Решение 1


1.Создан шаблон и items

2.Скриншоты item CPU И RAM приложены

![Задание-1](https://github.com/sailent9/zabbix-2/assets/130309754/b83e2d50-b820-4797-9e78-29f0e92b7a57)
![Задание-1 2](https://github.com/sailent9/zabbix-2/assets/130309754/21b0b6f8-1663-4ce8-9498-bc3ac99b122f)
















Задание 2
Добавьте в Zabbix два хоста и задайте им имена <фамилия и инициалы-1> и <фамилия и инициалы-2>. Например: ivanovii-1 и ivanovii-2.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
Установите Zabbix Agent на 2 виртмашины, одной из них может быть ваш Zabbix Server
Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов
Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera
Прикрепите за каждым хостом шаблон Linux by Zabbix Agent
Проверьте что в разделе Latest Data начали появляться данные с добавленных агентов
Требования к результату
 Результат данного задания сдавайте вместе с заданием 3


Решение 2

Приведите ответ в свободной форме........

Установлен агент на Zabbix server и одну VM
Добавлены в Host
Прикреплен шаблон "by Zabbix agent"
Скриншоты прикреплены 
![задаие 2 1](https://github.com/sailent9/zabbix-2/assets/130309754/5c79b906-774b-4c95-8569-817193499ac9)
![задаие 2 2](https://github.com/sailent9/zabbix-2/assets/130309754/f9ebc160-7340-4eaf-a0ae-81b05c3d6e6a)




Задание 3
Привяжите созданный шаблон к двум хостам. Также привяжите к обоим хостам шаблон Linux by Zabbix Agent.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
Зайдите в настройки каждого хоста и в разделе Templates прикрепите к этому хосту ваш шаблон
Так же к каждому хосту привяжите шаблон Linux by Zabbix Agent
Проверьте что в раздел Latest Data начали поступать необходимые данные из вашего шаблона
Требования к результату
 Прикрепите в файл README.md скриншот страницы хостов, где будут видны привязки шаблонов с названиями «Задание 2-3». Хосты должны иметь зелёный статус подключения


Решение 3
Приведите ответ в свободной форме........

Созданный шаблон прикперплен к каждому хосту
Скриншоты прилагаются
Поле для вставки кода...
git commit -m "название commit"
git push origin
![задаие 3 1](https://github.com/sailent9/zabbix-2/assets/130309754/ca8df144-67cd-4c7c-b374-a52f606a8437)




Задание 4
Создайте свой кастомный дашборд.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
В разделе Dashboards создайте новый дашборд
Разместите на нём несколько графиков на ваше усмотрение.
Требования к результату
 Прикрепите в файл README.md скриншот дашборда с названием «Задание 4»



Решение 4 
Приведите ответ в свободной форме........

Создан тестовый дашбоард
Добавлено пару графиков
Скриншоты прилагаются
Поле для вставки кода...
git commit -m "название commit"
git add *
git push origin
![Задание-4](https://github.com/sailent9/zabbix-2/assets/130309754/bc5e553d-746a-4754-8ded-deb0ca8ed8fb)
