University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2022/2023
Group: K4110c
Author: Ovchinnikov Ruslan Dmitrievich
Lab: Lab1
Date of create: 29.11.2022
Date of finished: 00.00.2022

# Ход работы

1) После установки docker и minikube был развернут minikube cluster:
![Screenshot_1](https://user-images.githubusercontent.com/79364379/204817030-bd27bc53-e2cf-42ed-8fc8-dccd0a1459a5.png)

2) Создан под vault по образу HashiCorp Vault (файл yaml приложен в папке лабораторной):
![vault](https://user-images.githubusercontent.com/79364379/204817815-e4cbcb12-57b8-44e1-b29f-7944544deb11.png)

3) Создан сервис для доступа к vault
![podExpose](https://user-images.githubusercontent.com/79364379/205054462-0a991212-9e8c-4284-b003-61a33cfb52c3.png)

4) Проброшен 8200 порт командой "minikube kubectl -- port-forward service/vault 8200:8200"

5) Заходим в vault по ссылке "http://localhost:8200". Токен для входа берем в логах vault:
![vaultLogs](https://user-images.githubusercontent.com/79364379/204819525-a9b0d923-4bce-4725-be4a-ebb28dae1418.png)
![Enter](https://user-images.githubusercontent.com/79364379/204819764-5272ece1-afaf-4bd5-a081-d6b8557cc06c.png)

