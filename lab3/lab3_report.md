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
Предварительно установив mkcerе

![image](https://user-images.githubusercontent.com/79364379/206779063-c676c1e3-6f66-4820-92d4-820c29ab5f96.png)

![image](https://user-images.githubusercontent.com/79364379/206782175-a25d7421-f90d-4a91-aed9-8c0debbdf308.png)

6) Создаем ingress в minikube

![image](https://user-images.githubusercontent.com/79364379/206855860-b056a613-7adc-41d9-8124-42ec12d5b495.png)

![image](https://user-images.githubusercontent.com/79364379/206855863-5b6dcb66-ef33-4539-9c09-c1c609189bab.png)

7) Запускаем тунель minikube

![image](https://user-images.githubusercontent.com/79364379/206857781-5c24fa67-ebee-4d74-ad50-5467c58af6a6.png)

8) Далее (после редактирования файла hosts) смотрим результат

![image](https://user-images.githubusercontent.com/79364379/206857823-b285c127-2ccf-478e-b17b-ab2d580a41bf.png)




