### 1-clic Factory

Depuis, plusieurs mois, si vous nous suivez, vous avez pu voir passer les différents épisodes des [Stacks 5 Minutes](http://dev.cloudwatt.com/fr/blog/index.html)
Les apps sont mises à disposition dans notre répertoire Github pour un déploiement en ligne de commande. Mais elles sont aussi – pour la plupart – déployables aussi depuis le site web de Cloudwatt par « 1-clic » dans la rubrique [Applications](https://www.cloudwatt.com/fr/applications/).
En septembre 2015, nous avons publié en opensource notre *Openstack Image Factory* pour la construction des images.
Maintenant, nous allons passer dans d’autres coulisses et vous expliquer comment publier vos applications sur *votre* site web en utilisant cette « 1-clic Factory ». Suivez le guide et faites attention où vous marchez.

## L’usine 1-clic

# Sur le Github
Tout d'abord, clonez ce dossier 'setup_oneclick'. Vous avez maintenant ce dossier dans votre espace privatif Github.

Pour la publication de votre app, vous avez créé votre template d’orchestration HEAT qui est en format .yaml. Il faut le transformer en format .json. Pour ce faire « google est votre ami », vous trouverez sur le web des « traducteurs » yaml/json.
Dans le dossier, vous trouverez des exemples de syntaxe json.
Une fois votre .json généré, placez le dans le dossier setup_oneclick/stacks/

# Sur votre site web
Placez le dossier setup_oneclick/ et toute son arborescence à l'endroit de votre choix sur votre site, le chemin n'ayant pas d'importance.

Votre 1-click est maintenant prêt à être utilisé.

# Utilisation 

L’url de l’apps sur votre site est d’un format {le-chemin-de-votre-oneclick}/setup_oneclick/#/heat/lenomdufichierjson

Par exemple pour wordpress.json : www.monnomdesit.com/mesapps/setup_oneclick/#/heat/wordpress

# Bonus
Vous pouvez aussi modifiez les .css pour les aligner sur le look & feel de votre site.

## Licence
Le contenu de ce dépôt est la propriété de Cloudwatt et placé sous licence GPLv3.