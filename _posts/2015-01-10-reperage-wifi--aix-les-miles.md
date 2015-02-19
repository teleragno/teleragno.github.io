---
layout: post
title: "Repérage et étude radio du 2014-11-15 (Aix-les-Miles)"
description: "CR d'une visite pour un raccordement d'un quartier"
category: 
tags: [wifi]
---
{% include JB/setup %}

# Objectifs

L'idée de l'opération de reconnaissance réalisée est simple : déterminer les différents éléments nécessaires pour raccorder au net un quartier isolé.
En l'occurence  à proximité d'Aix-les-Miles.

# Démarche & questions

Afin de pouvoir produire une synthèse de la visite et essayer de capitaliser nos différentes visites, voici une liste des questions que l'on pose.
Elles ont pour but de faire un point rapide des éléments clefs.

Sur l'existant :

* y-t-il du net (ou une forme dégradée) qui arrive déjà ?
* si oui, quel opérateur ? quelle technologie ? (xDSL ? câble coaxial ? fibre ? 3G ? téléphone classique / 56k ? autre ?) quel tarif ?
* si non, avez vous fait des demandes de raccordement ? (si oui, cf. question précédente)

Sur une possible intervention :

* y-a-t-il plusieurs personnes intéressées par un raccordement ?
* êtes vous prêt à agir pour que les choses se fassent ?
* comprenez-vous que nous sommes bénévoles ? (-> explication des conséquences et de la relation entre membres)
* comprenez-vous que l'association est une mutualisation des ressources ? (-> implication sur la politique de coûts & des frais non masqués & d'installation)

* êtes-vous locataire du logement ? y-a-t-il un syndic ? est-il professionnel ou constitué de co-propriétaires ?
* connaissez-vous les règles locales pour les accès aux parties communes ? aux toits ?
* le batiment est-il soumis à des régles d'urbanisme particulières (ex: momument historique) ?

Avec les réponses à ces questions, nous avons une vision peu technique de l'environnement et avons une indication sur le nombre de personnes intéressées par un raccordement.
Cette information est utile car elle permet d'envisager des solutions plus complexes et coûteuses (= installer plus d'équipements pour atteindre le lieu géographiquement isolé)

# Reconnaissance du site

Dans le cas présent, il s'agit de déterminer comment réaliser un lien radio (wifi longue portée) entre le logement et un point intermédiaire pour rebondir vers un datacenter.

Faire une reconnaissance est aussi un bon prétexte pour faire une visite du département et de faire des photos :)

![panneau](/assets/files/2014/11/IMG_0014.jpg)
![pont](/assets/files/2014/11/IMG_0016.jpg)

## Point haut n°1

Un local contenant un transformateur électrique de quartier.
Intéressant pour la position et la source de courant.
A priori compliqué à utiliser pour des raisons d'autorisations.

![transformateur](/assets/files/2014/11/IMG_0055.jpg)

Des champs entourés d'arbres.
Pas de visibilité particulière.

![champ](/assets/files/2014/11/IMG_0036.jpg)

À l'arrière plan, une colline.
Le riverain indique qu'un pôle d'activité est présent dans la zone.

![colline](/assets/files/2014/11/IMG_0038.jpg)

Avec de l'attention on perçoit un château d'eau.

![colline-focus](/assets/files/2014/11/IMG_0038-focus.jpg)
![chateau d'eau](/assets/files/2014/11/IMG_0057.jpg)

## Point haut n°2

Et en se déplaçant un peu on observe la chaine de l'étoile.

![massif de l'étoile](/assets/files/2014/11/IMG_0069.jpg)

Un paire de jumelles confirme que certains pylônes installés sur le site sont visibles.

![massif de l'étoile zoom](/assets/files/2014/11/IMG_0069-focus.jpg)

Il est temps d'aller voir le château d'eau de plus près.

## Visite au Petit Arbois

![entrée petit arbois](/assets/files/2014/11/IMG_0100.jpg)

Une installation qui semble déjà bien utilisée.

![chateau d'eau complet](/assets/files/2014/11/IMG_0102.jpg)

Le site est vieillissant (le gestionnaire du site nous le confirmera par mail) et certaines précautions doivent être respectées.

![installation ancienne](/assets/files/2014/11/IMG_0106.jpg)
![consignes](/assets/files/2014/11/IMG_0107.jpg)
![consignes zoom](/assets/files/2014/11/IMG_0112.jpg)
![consignes radio](/assets/files/2014/11/IMG_0115-focus.jpg)


Une bonne surprise cependant, un local technique est présent et plusieurs opérateurs sont présents sur le site.

Orange et SFR au minimum.

Les consignes de sécurité estampillées du logo orange.
SFR identifie ses câbles.
Un logo de Bouygues Telecom est également présent mais discret. Peut être un reliquat d'installation.

![présence SFR](/assets/files/2014/11/IMG_0125.jpg)

# Pourquoi concrètement un point haut intéresse un FAI ?

Les coordonnées du point haut en place :

* `43.492447, 5.330627`
* soit 43°29'32.8"N 5°19'50.3"E
* [une vue directe](https://www.google.fr/maps/place/43%C2%B029'32.9%22N+5%C2%B019'50.2%22E/@43.49246,5.330624,148m/data=!3m2!1e3!4b1!4m2!3m1!1s0x0:0x0)


Utilisons [Hey Whats That.com ?](http://wisp.heywhatsthat.com/) pour faire une simulation de couverture radio.
Cela permettra de savoir quelle zone géographique pourrait être désservie par l'installation d'une antenne sur ce point haut.

[HWT](http://wisp.heywhatsthat.com/) utilise le relief et la portée de l'antenne (configurable) pourdéterminer la zone de couverture.

Configuration du point haut avec les coordonnées GPS

![hwt config](/assets/files/2014/11/HeyWhatsThat_WISP02.jpg)

L'antenne est positionnée sur un fond de carte

![hwt position](/assets/files/2014/11/HeyWhatsThat_WISP01.jpg)

On demande à [HWT](http://wisp.heywhatsthat.com/) de calculer et d'afficher les zones à portée radio.

Attention, toutes les zones colorées ne sont pas exploitables en réel.
Les habitations et la végétation ne sont pas prises en compte.

![hwt couverture](/assets/files/2014/11/HeyWhatsThat_WISP03.jpg)

Ça devients intéressant comme étude lorsque l'on ajoute plusieurs stations

![hwt couverure multiple](/assets/files/2014/11/HeyWhatsThat_WISP04.jpg)

--

jpierre03
