---
title: "Créer une application à partir d’un prototypes sans code !"
date: 2022-01-13T15:46:49+01:00
draft: false
author: Nathan Zweifel
description: "Comprendre les différences entre ces trois concepts clés."
#featuredImage: "IMG_20210812_122248.jpg"
tags: ["Application", "Processus", "Haute-fidélité", "Mobile", "Interface"]
categories: ["Présentations de prototype", "Processus de prototypage"]
---

Il n’est pas toujours facile de réaliser un prototype haute-fidélité en html et css, et encore moins de réaliser l’application entière pour un designer. Evidemment, ce n’est pas son métier. Cependant, avec la venue du No Code, des outils nous permettant de faire tout ça à partir d’un prototype (sur Figma par exemple) apparaissent de plus en plus. Aujourd’hui, nous allons essayer l’outil [Bravo](https://www.bravostudio.app/) pour la création d’un petit prototype haute-fidélité.
# Mise en place
Tout d’abord, il faut savoir que Bravo ne fonctionne qu’avec Figma ou Adobe XD. Dans notre cas, ce sera avec Figma, en utilisant un de leur prototype de présentation déjà fait. 
Bravo fonctionne ensuite en reconnaissant les éléments des maquettes par frames. Ainsi, un écran est une frame de premier niveau, puis un autre élément comme le header doit également être sous forme de frame. Les frames étant ainsi faites, on peut les renommer un tag (comme `[container]` ou `[menu]`) qui permettra à Bravo de comprendre ce que représenter l’élément.
 
Chaque frame de notre application doit donc être décrite avec ces tags. Par exemple la page de connexion possède le tag `[intro:always]` dans son nom. Cela défini qu’à chaque utilisation de l’application, l’utilisateur arrivera sur cette page. Cela simplifie aussi le processus : plus besoin de répéter le menu sur chaque page ! Il suffit de créer une frame comportant le menu, avec le tag `[menu:tab]`. La liste complète des tags est disponible ici. Attention à ne pas oublier les liens entre les pages, Bravo s’y réfèrera aussi pour l’application finale.
# Import du design
Une fois notre fichier de design prêt, nous pouvons aller sur notre profil sur Bravo, puis dans le menu app pour en créer une nouvelle. Pour lier l’application à votre fichier, il suffit d’y mettre son lien Figma (ou d’utiliser un plugin avec Adobe XD). Une fois le design importé, il est possible d’avoir un aperçu des écrans, de pouvoir créer des notifications push selon notre envie, mais également de pouvoir publier notre application (pour android ou iOS). A savoir que nos données sont ici statiques, mais peuvent tout à fait devenir dynamiques en liant l’application à une base de données comme [Airtable](https://www.airtable.com/?utm_source=google&utm_medium=cpc&utm_extra5=kwd-98523555182&utm_extra2=11493609735&utm_extra10=120737223988&creative=475905503164&device=c&cx=row&targetid=kwd-98523555182&campaignid=11493609735&adgroupid=120737223988&utm_campaign=brand_creator&utm_content=bofu_freetrial&gclid=Cj0KCQiA6NOPBhCPARIsAHAy2zCaGGQDi99L67u8bbRjEiNHAuDlF40MRYXJ85GrQzcfeU3aahWMQKcaAm1oEALw_wcB).
# Partage de l’application
Dans notre cas, nous ne voulons pas directement publier l’application dans un store, mais d’abord l’utiliser comme prototype haute-fidélité. Pour cela, il suffit d’installer l’application (Android ou iOS) Bravo sur notre téléphone, puis de se connecter avec ses identifiants. L’application peut ensuite être lancée et utilisée en local pour des tests utilisateurs.
# Bilan de l’expérimentation
Ayant un bon bagage technique, en plus de ma passion pour le design d’interfaces et le prototypage, j’avais beaucoup d’aprioris sur les solutions de « No-code ». Cet article était vraiment l’occasion pour moi de m’y essayer. J’en ressort avec une bien meilleure vision de cela, mais seulement pour certains cas. Pour le prototypage, cela marche très bien et donne encore une meilleure expérience haute-fidélité qu’une simple interface interactive (notamment avec le lien avec une api). Pour une petite application temporaire (par exemple pour un festival) je me verrai bien pourquoi pas aussi l’utiliser. Néanmoins, le manque de visibilité dans la partie programmée de l’application me semble trop risquer pour un projet de plus grande envergure.

