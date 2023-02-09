# Домашнее задание к занятию 10.3 «Pacemaker» Сергей Баранов


---

### Задание 1

Опишите основные функции и назначение Pacemaker.

*Приведите ответ в свободной форме.*

Pacemaker - это менеджер ресурсов кластера со следующими основными функциями:

* Обнаружение и восстановление сбоев на уровне узлов и сервисов;
* Независимость от подсистемы хранения: общий диск не требуется;
* Независимость от типов ресурсов: все, что может быть заскриптовано, может быть кластеризовано;
* Поддержка STONITH (Shoot-The-Other-Node-In-The-Head);
* Поддержка кластеров любого размера;
* Поддержка и кворумных и ресурсозависимых кластеров;
* Поддержка практически любой избыточной конфигурации;
* Автоматическая репликация конфига на все узлы кластера;
* Возможность задания порядка запуска ресурсов, а также их совместимости на одном узле;
* Поддержка расширенных типов ресурсов: клонов (запущен на множестве узлов) и с дополнительными состояниями (master/slave и т.п.);
* Единый кластерный шелл (crm), унифицированный, скриптующийся.


---

### Задание 2

Опишите основные функции и назначение Corosync.

*Приведите ответ в свободной форме.*

Corosync - программный продукт, позволяющий реализовать кластер серверов. Его основное назначение - знать и передавать состояние всех участников кластера. 

В основе работы заложены следующие функции:

* отслеживание состояния приложений;
* оповещение приложений о смене активной ноды кластера;
* отправка одинаковых сообщений процессам на всех узлах кластера;
* предоставление доступа к базе данных с конфигурацией и статистикой, а также отправка уведомлений о ее изменениях.


---

### Задание 3

Соберите модель, состоящую из двух виртуальных машин. Установите Pacemaker, Corosync, Pcs. Настройте HA кластер.

*Пришлите скриншот рабочей конфигурации и состояния сервиса для каждого нода.*

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3_node1.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3_node2.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3_pacemaker.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3_pacemaker_n2.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3apache2.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-3apache2_resources.png)


---

### Задание 4

Установите и настройте DRBD-сервис для настроенного кластера.

*Пришлите скриншот рабочей конфигурации и состояние сервиса для каждого нода.*

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-4.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-40.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-40_node2.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-41.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-41_node2.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-4_mysql.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-4_node2_mysql.png)

![monitoring](https://github.com/12sergey12/10.3_Pacemaker/blob/main/images/10.3-4_node2_www.png)
