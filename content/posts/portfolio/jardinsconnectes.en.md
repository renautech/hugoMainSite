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

# Web Application Connected Gardens / [Les Jardins Connectés](http://jardinsconnectes.renautech.fr/)

{{< youtube doV8TvNGKbE >}}
[French video only]

This application has a great story. It started in my head in 2019. I imagined to develop it in Python to have a unique language with... connected objects. I teached Python at school, coded a bit on Raspberry and Arduino, so it was the most natural for me.
In 2018 I developed in PHP with the [Laravel](https://laravel.com/) framework, I could have use PHP too...

Finally Connected Gardens is written in Javascript in 2020 during a 6 months Javascript training at [O'clock](https://oclock.io/).

## Why Javascript ?
Javascript is used both on the [Front]({{< ref "posts/glossary">}}) and [Back]({{< ref "posts/glossary">}}) end. But I am interested in the user interface, the business logic and the databases at the same time. Javascript was an ideal candidate for me.

Javascript is perfectly adapted to this type of Web application. Connected Garden is :
- a dynamic application on the browser
- an application on a remote server that hosts the application logic and database. It is a [REST API]({{< ref "posts/glossary">}}).

## What about Front end ?

React is a nice Javascript library. React has been chosen for the Front. The reason is simple: it is the specialty during my training! React is very popular and very efficient.
React sees the user interface as a set of components. Each component has a state that represents its characteristics at a given time. 

For example in Connected Gardens, a component manages the display of the families of vegetables grown in the vegetable garden. When the user sows a new vegetable, the state of this component changes and React updates the interface with this new vegetable.

The complexity with React comes precisely from the management of the component state. In order to manage the state of many components, it is necessary to use [Redux]({{< ref "posts/glossary">}}).

## And Back end?

Back in Javascript is [NodeJS]({{< ref "posts/glossary">}}) domain. NodeJS executes code, but it is not basically a web server.

The Web server chosen for the Connected Gardens Backbone is [Express](https://expressjs.com/fr/) server. It is a module to be installed on NodeJS. In the first approach, it provides the possibility to define routes to react to user requests on a specific URL. For example http://www.myapp.com/article/sneakers-discount should return the list of discounted sneakers to the user's browser. Express will intercept this request and execute the right code in the application. Express offers many methods to then format the response and send it to the user.


