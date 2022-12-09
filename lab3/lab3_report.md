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
1) Создаем ConfigMap
![image](https://user-images.githubusercontent.com/79364379/206775760-0b75f455-a45d-45d7-9335-17e45bbb851b.png)
![image](https://user-images.githubusercontent.com/79364379/206775692-7b1a71fa-a395-462c-bf09-b75cabfff5eb.png)

2) Создаем replicaSet с 2 репликами контейнера ifilyaninitmo/itdt-contained-frontend:master и передаем переменные из ConfigMap
![image](https://user-images.githubusercontent.com/79364379/206776098-f036b9a2-d808-4604-9d63-bf25b0bc9e7c.png)
![image](https://user-images.githubusercontent.com/79364379/206776186-7ca89329-588e-4b77-bd14-4c8b9b20c2d5.png)

3) Создаем сервис для доступа
![image](https://user-images.githubusercontent.com/79364379/206776424-9d1e510a-d341-4322-88b4-6612baf3a857.png)
![image](https://user-images.githubusercontent.com/79364379/206776546-65c17a94-6375-40dd-b2f1-65d3008659bb.png)

4) Включаем ingress
![image](https://user-images.githubusercontent.com/79364379/206776810-cb6d0959-73a6-4fc2-a594-34ce890f5867.png)

5) Создаем TSL сертификат
