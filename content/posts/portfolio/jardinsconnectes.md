+++ 
draft = false
date = 2020-12-21T14:32:17+01:00
title = "Les Jardins Connectés"
description = "L'application Les Jardins Connectés"
slug = ""
authors = []
tags = []
categories = []
externalLink = ""
series = []
+++

# Application Web [Les Jardins Connectés](http://jardinsconnectes.renautech.fr/)

{{< youtube doV8TvNGKbE >}}

Cette application est une belle histoire. Elle a commencé dans ma tête en 2019. J'imaginais la développer en Python pour avoir un langage unique avec... des objets connectés. J'avais donné des cours en Python, codé un peu sur des Raspberry et Arduino, c'était le plus naturel pour moi.
En 2018 je développais en PHP avec le framework [Laravel](https://laravel.com/), j'aurais pu tenter aussi...

Finalement c'est en Javascript qu'elle s'écrit en 2020 dans le cadre d'une formation de 6 mois en Javascript chez [O'clock](https://oclock.io/).

## Pourquoi Javascript ?

Javascript est utilisé à la fois côté [Front]({{< ref "posts/glossary">}}) et côté [Back]({{< ref "posts/glossary">}}). Or je suis attiré à la fois par l'interface utilisateur, par la logique métier et les bases de données. Javascript était un candidat idéal pour moi.

Javascript est tout à fait adapté à ce type d'application Web. Les Jardins Connectés c'est :
- une application dynamique sur le navigateur
- une application sur un serveur distant qui héberge la logique de l'application et la base de données. C'est une [API REST]({{< ref "posts/glossary">}}).

## Côté Front alors ?

React est une belle librairie Javascript. React a été choisi pour le Front. La raison est simple : il s'agit de la spécialité lors de ma formation ! React est très populaire et très efficace.
React voit l'interface utilisateur comme un ensemble de composants. Chaque composant possède un état qui représente ses caractéristiques à un moment donné. 

Par exemple dans Les Jardins Connectés, un composant gère l'affichage des familles de légumes cultivées dans le potager. Lorsque l'utilisateur sème un nouveau légume, l'état de ce composant change et React met à jour l'interface avec ce nouveau légume.

La complexité avec React vient justement de la gestion de l'état des composants. Pour permettre la gestion de l'état de nombreux composants, il faut utiliser [Redux]({{< ref "posts/glossary">}}).

## Et côté Back ?

Le Back en Javascript est le domaine de [NodeJS]({{< ref "posts/glossary">}}). NodeJS exécute du code, mais il n'est pas de base un serveur Web.

Le serveur Web choisi pour le Back des Jardins Connectés est le serveur [Express](https://expressjs.com/fr/). Il s'agit d'un module à installer sur NodeJS. En première approche, il fournit la possibilité de définir des routes pour réagir aux demandes de l'utilisateur sur une URL spécifique. Par exemple http://www.monapplication.com/article/baskets-promo doit renvoyer la liste des baskets en promotion au navigateur de l'utilisateur. Express va intercepter cette demande et exécuter le bon code dans l'application. Express propose de nombreuses méthodes pour ensuite mettre en forme la réponse et la transmettre à l'utilisateur.
