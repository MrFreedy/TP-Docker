# TP-Docker

## TP-1

### Question 5:
a) Récupération de l'image nginx depuis Docker Hub:<br>
`docker pull nginx`

b) Vérification de la présence de l'image nginx:<br>
`docker images`
![alt text](./TP-1/img/q5_image_1.png)

c) (Cf. index.html)

d) Lancement du container:<br>
`docker run --name TP-1 -d -p 8080:80 -v $(pwd)/TP-1:/usr/share/nginx/html nginx`
![alt text](./TP-1/img/q5_image_2.png)

e) 
#### Suppression:<br>
`docker stop tp-nginx-vol
docker rm tp-nginx-vol`

#### Utilisation de la commande `cp`

- Démarrage du container sans volume:<br>
`docker run --name tp-nginx-cp -d -p 8080:80 nginx`

- Copie des fichiers:<br>
`docker cp ./TP-1/index.html TP-1:/usr/share/nginx/html/index.html`

![alt text](./TP-1/img/q5_image_3.png)

![alt text](./TP-1/img/q5_image_4.png)

### Question 6:




## TP-2

### Question 2:

L'option npm est `npm install`. Elle permettra d'installer toutes les dépendances nécessaires dans le container. Cela permettra d'avoir une image Docker reproductible et stable.

### Question 3:

La commande pour build l'image Docker est la suivante : `docker build -t ma_super_app .`<br><br>![alt text](./TP-2/img/q3_image_1.png)

![alt text](./TP-2/img/q3_image_2.png)

### Question 4:

![alt text](./TP-2/img/q4_image_1.png)

![alt text](./TP-2/img/q4_image_2.png)