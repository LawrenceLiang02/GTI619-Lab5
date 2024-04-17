# GTI619-Lab5

Notre projet est configuré avec **Docker** seulement pour **le backend et la base de données MySQL**, puisque dockerize le frontend rendra le processus de load plus lent, react a beaucoup de modules qui ne sont pas nécessaire, mais doivent être là. **Le frontend est avec React donc faudait Node**.

## Run Project
Pour run le frontend, vous devez **etre dans le fichier "React_Frontend"** et ensuite utiliser la commande npm run start. Vous pouvez suivre les commandes ci-dessous.

Frontend: ```cd React_Frontend``` et  ```npm run start```

Pour run le backend et database avec docker, vous devez être dans le top directory du projet, donc "/GTI619-Lab5", puis utiliser la commande qui suit. **Il se peut que le backend ne run pas après la première fois**. C'est normal puisqu'on n'a pas de tests qui vérifie si le database est en marche avant de run le backend, on a seulement un delay. 

**Dans le cas que lorsque vous buildez, et ça ne run pas le backend**, si vous avez docker desktop, vous pouvez juste recommencer le server qui est le flask app, ou sinon réutiliser la commande.

Il se peut que vous ayez un message en disant que le port 0.0.0.0:3306 n'est pas disponible, faut juste cliquer le boutton restart dans le docker desktop et ça va marcher.

Backend and Database with Docker: ```docker-compose up --build```

## Git Commands:

### Clone project: 
```git clone https://github.com/LawrenceLiang02/GTI619-Lab5.git ```

 ### Commit Project:
 Ajouter les fichiers: 
 ```git add .```

 Commit avec un commentaire:
 ``` git commit -m " [COMMENTAIRE] "```

 Push: 
 ``` git push ```


### Merge Conflict:

Fetch files from main:
``` git fetch origin main```

Rebase Code:
``` git rebase origin/main```

Rebase merge conflicts:
``` git add .```
``` git rebase --continue```

Force Push (only after using rebase):
``` git push -f```

