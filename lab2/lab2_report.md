University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2022/2023
Group: K4110c
Author: Ovchinnikov Ruslan Dmitrievich
Lab: Lab1
Date of create: 01.12.2022
Date of finished: 00.12.2022

# Ход работы

1) Создан deployment с 2 репликами контейнера ifilyaninitmo/itdt-contained-frontend:master, в которые переданы необходимые переменные (Файл deployment.yaml в приложении)

![ifilyaninApply](https://user-images.githubusercontent.com/79364379/205309290-8000e87e-2438-4870-8259-8ebc4b41d270.png)

2) Создан сервис для доступа к контейнерам и проброшен 3000 порт

![ExposePortForward](https://user-images.githubusercontent.com/79364379/205309521-1f0a10be-77f5-482e-a09c-10a2b60994ee.png)

3) Заходим в контейнеры по ссылке "http://localhost:3000", где можем увидеть введенные ранее переменные

![Browse3000](https://user-images.githubusercontent.com/79364379/205309842-9e26368f-1e27-4147-b86e-008ab4925697.png)

4) Логи контейнеров

![logs](https://user-images.githubusercontent.com/79364379/205310291-31427f23-f3d2-432f-9630-205c7870e0c7.png)

5) Схема 

![image](https://user-images.githubusercontent.com/79364379/205452614-cc925bb2-3c36-44b1-86b7-931492a1c339.png)

# Вопросы и ответы
Вопрос: Чем отличается Deployment от ReplicaSet и DaemonSet

Ответ:

Deployment позволяет обновить сами поды и реплики или создать новые.
ReplicaSet позволяет сохранять стабильный набор подов (всегда доступно определенное количество подов).
DaemonSet автоматически добавляет копию пода в ново созданный узел и удаляет под при его удалении (работает сборщик мусора).
