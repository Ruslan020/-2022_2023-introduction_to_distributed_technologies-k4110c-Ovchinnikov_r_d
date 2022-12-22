1. Запускаем minikube c необходимыми для создания 2 нод и включения плагина calico параметрами

![createNodes](https://user-images.githubusercontent.com/79364379/209167029-f899fc0a-d1bb-41d8-8dfa-71d9db92610d.png)


2. Проверка pods и nods

![Nodes](https://user-images.githubusercontent.com/79364379/209167215-75717874-852e-4f89-af4e-1c0eae677a0a.png)
![PodsCalcio](https://user-images.githubusercontent.com/79364379/209167255-65d0d3c9-2488-488b-9028-8c324519c6e5.png)

3. Для дальнейшей работы запускаем calicoctl.yaml

![calcioctlRun](https://user-images.githubusercontent.com/79364379/209167618-9d729711-4a69-4afd-b9ce-c51815ab3ef2.png)

4. Назначение зон для узлов

![Labled](https://user-images.githubusercontent.com/79364379/209167760-ec62949d-ce15-4858-bdf5-370e0446fc17.png)

5. Создаем ip пул с помощью IPpoll.yaml

![image](https://user-images.githubusercontent.com/79364379/209170131-9d5e8517-f991-412b-ac07-3d0875bc7744.png)
![IPpoolCreate](https://user-images.githubusercontent.com/79364379/209168014-92ece1f1-7546-4977-bd18-8dc073853ed9.png)
![GetIpPools](https://user-images.githubusercontent.com/79364379/209168126-10c5ae32-1805-4cfd-9a7c-86d103b9d033.png)

6. Аналогично прошлым работытм создаем поды и сервис для доступа

![CreateDeploypent](https://user-images.githubusercontent.com/79364379/209168514-10e7f23b-a4a5-48c8-8624-35226d8515d9.png)
![Service](https://user-images.githubusercontent.com/79364379/209168424-8391662d-6c48-4a53-9772-204c8eb663f1.png)

7. Отображение в бразуере

![икщцыу](https://user-images.githubusercontent.com/79364379/209168601-c9475976-09f8-4d80-a825-5d26f1d17faf.png)

8. Ping между подами

![ping1](https://user-images.githubusercontent.com/79364379/209168791-9f894998-103b-4bfa-b45e-dad0f082917f.png)

9. Схема

![image](https://user-images.githubusercontent.com/79364379/209169929-e24ae502-39d2-492d-b7f0-93b802a4d26e.png)

