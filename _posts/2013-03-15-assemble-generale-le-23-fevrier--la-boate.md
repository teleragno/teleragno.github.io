---
layout: post
title: "Assemblée générale le 23 Février 2013 à la La Bo[a]te"
description: ""
category:
tags: []
---
{% include JB/setup %}

# Point de l'outillage

* uniquement du PDF
* documents de travail texte en brut : présentation de Markdown et de Pandoc
* outil de travail collaboratif & de gestion de version : GIT

# Markdown

* texte brut :
	Fichier MKD qui peut se traduire en PDF, TXT, HTML, Word, docx avec utilisation pandoc
* Pour les titres

		# Titre 1
		## Titre 2

* Pour sauter une ligne laisser une ligne blanche
* Pour l'afficher il faut

		$ pandoc -s toto.mkd -o toto.pdf

* Sous-titre

		## Titre

* Liste

		*<espace><texte>

* Liste de définitions

		titre en maj
		~tab+texte

* Liste numérotée

		1.space+texte
		tab+a.+texte

* Tableaux
	pour réaliser le caractère |, utilisez la combinaison de touches < alt gr > + < 6 >

		| nom | qualité | signature |
		| - | - | - |


| nom | qualité | signature |
| - | - | - |


* Ajouts de pandoc à markdown

		% titre du truc - titre
		% toto - auteur
		% date - date

* Ajout d'une image

		![texte](chemin du doc)

* Note bas de page

	^[note bas de page]

# GIT

* commandes usuelles

		$ git init (créer un dossier, dépôt,local)
		$ git status (voir les dossiers)
		$ git ad toto.mkd (ajout ds la liste des fichiers du dossier)
		$ git commit -m "premier commit" (indiquer la modif faite pour ne pas avoir à ouvrir le doc à chaque fois)
		$ vim .gitignore (exclure certains types de fichiers par leur extension/nom)

* commit le gitignore pour que tout le monde ait accès à la liste de fichiers à exclure:

		$ git add .gitignore
		$ git commit -m "ajout de gitignore"

* clone d'un dépôt

		$ git clone + adresse dépôt

* modification de fichier

		$ vim toto.mkd
		+ commit

* push de la branche vers origin:

		$ git push origin

