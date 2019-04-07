# Le Fameux Docker ? 
![Docker logo](https://www.docker.com/sites/default/files/social/docker_facebook_share.png)


### Docker est une plateforme qui permet de créer, envoyer et deployer des application dans n'importe quel environnement.
Cett definition de Docker met des étoiles dans les yeux de n'importe quel developper (spécialement devops).

_Mais attend, n'est-ce pas ce qu'une Machine Virtuelle (VM) fait déjà de mieux?_\
_D'un point de vue oui... Mais rassures toi, les développeurs de Docker y ont déjà pensé, et biensûr ils n'ont juste pas fait de renommer la roue (de VM à Docker) mais ils l'ont re-disigner, pas une roue carrée quand même_

Jette un regard sur l'image ci dessous pour mieux comprendre la différence entre Docker et VM.
![alt](https://i.gyazo.com/627f3585a7f0e89d706ee02c9883f651.png)

En effet comme tu peux le voir, Docker supprime la difficulté d'avoir un autre système d'exploitation (OS) sur un autre. Et tu l'as bien déviné, en supprimant déjà la nécessité du système additionnel, Docker devient beaucoup plus léger et plus facile à gérer.
Pour effectuer une autre analogie, pense à l'idée de JAVA et JVM.

J'espère jusque là t'avoir convaincu pour continuer notre voyage au coeur de Docker.

## Voyage
Comme tout voyage, il faut la préparer pour éviter certaines surprise. Dans notre cas, notre voyage au coeur de Docker se constiturera de la Péparation, du Trajet et de l'Exploration. Biensûr nous avons pris un ticket Aller.

## Préparation
### Example 1
Ok, jusque-là je n'ai juste fais que de parler de Docker et de notre voyage, et parlé à longueur de journée par fini devient ennuyant. Là je suis d'accord mon ami.

Nous allons donc jetter un coup d'oeil à quoi notre voyage pourrait ressembler.
Dans cette partie, nous allons tout simplement télécharger une application et la lancer avec Docker.
Mais avant tout, tu rappelles je t'ai parlé de JAVA et JVM, n'est-ce pas ? Comme pour lancer une application JAVA tu as besoin d'un JVM, aussi pour lancer une application avec Docker, il faut aussi Docker-engine (Nous allons en revenir là dessus).

### Installer Docker engine et Docker client
Si tu n'as pas docker déjà installé sur ta machine, tu peux le faire en suivant ce lien.\
[Installer Docker Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/) Tu peux aussi l'installer sur d'autres systèmes linux.\
[Installer Docker sur MacOS](https://docs.docker.com/docker-for-mac/install/)\
[Installer Docker sur Windows](https://docs.docker.com/docker-for-windows/install/)

### Lancer l'application
J'ai écris cet article entièrement dans un fichier markdown (.md), et j'ai utiliser [dillinger](https://dillinger.io "diilinger.io") pour le publier. Cela m'a donné l'idée donc d'utiliser dilliger comme application de test tout au long de cet article.
```sh
docker run --name mon_premier_conteneur -p 4200:8080 joemccann/dillinger
```
Maintenant ouvre ton navigateur préféré et va sur le lien ``http://localhost:4200``\

Comme par magie, l'application dillinger est bien lancée sur notre machine sur le port 4200.
Félicitations! Tu viens de lancer ta première application avec Docker.

### Comment ça marche ?
Si tu te poses la question de comment ça marche, permet moi donc te t'expliquer cela.
``docker run``, cette commande tu l'auras déviner, ordonne à Docker (pour être précis docker daemon) de lancer un conteneur.

``--name`` c'est une option de la commande ``docker run`` qui permet donne un nom à notre conteneur qui sera lancé.

``-p 8080:4200`` cette option dis à docker de faire correspondre le port ``8080`` de notre machine au port ``4200`` du conteneur

## Le Trajet

## l'Exploration

<footer>
<img src="https://www.docker.com/sites/default/files/social/docker_facebook_share.png" width=50px>
</footer>

### Author: Chriss Osler Santi, osler.santi@gmail.com