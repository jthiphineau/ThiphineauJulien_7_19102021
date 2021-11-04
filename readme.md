# PROJET 7

# GROUPOMANIA - CREER UN RESEAU SOCIAL D'ENTREPRISE

## INSTRUCTIONS 

* Prérequis:
    * Node.js (npm),
    * MySQL,
    * Git.

- Clonez ce repository:

```bash
git clone https://github.com/jthiphineau/ThiphineauJulien_7_19102021.git
```


## FRONTEND

- Ouvrez le terminal sur "Frontend" et faites:

```bash 
npm install
```

- Mettez en route le Front:

```bash
npm run serve
```


## MySQL

- Ouvrez un autre terminal:

```bash
cd /usr/local/mysql
```

- Connectez-vous à mysql:

```bash
mysql -h localhost -u root -p
```
ainsi que votre mot de passe pour la base de donnée

- Importez le fichier " initialisationBdd.sql "

```bash
mysql> source (chemin vers le fichier initialisationBdd.sql)
```

- Création de la base de données nommée "groupomania"

## BACKEND

- Ouvrez le fichier " .env.initial " : Donnez des valeurs aux 3 variables:

```bash
DB_USER = 
DB_PASS = 
TKN_SECRET = 
```

- DB_USER: nom d'utilisateur pour votre base de données.
- DB_PASS: mot de passe pour votre base de données.
- TKN_SECRET = variable de votre choix.

- Renommer ce dossier " .env " à la place de " .env.initial ".

- Ouvrez un autre terminal sur "Backend" et faites:

```bash
npm install
```

- Mettez en route le Back:

```bash
node server
```

## DANS LE NAVIGATEUR

- Ouvrez votre navigateur à l'adresse: http://localhost:8080/

- Vous voyez l'écran de connexion à l'application. Allez dans la rubrique INSCRIPTION, inscrivez l'utilisateur de votre choix en suivant les instructions, puis connectez-vous.

- Pour avoir le privilège d'Adminstrateur, revenez dans votre terminal connecté à MySQL, et importez le fichier setAdmin.sql. 

```bash
mysql> source (chemin vers le fichier setAdmin.sql)
```

Cela attribuera au premier utilisateur créé (User id=1), les privilèges d'administration (isAdmin=1).

Recharger la page de votre naviguateur pour voir votre compte passer de simple utilisateur à adminstrateur.

Le site vous permet de partager des images et de les commenter, les vôtres et celles des autres. Vous pouvez supprimer votre compte. L'administrateur peut supprimer les comptes de n'importe qui, ainsi que les commentaires et les images.

