---
title: "Note #012 : L'approche modulaire en IA générative"
datePublished: Tue Apr 09 2024 12:15:26 GMT+0000 (Coordinated Universal Time)
cuid: clusch71d000908jselidh5r1
slug: note-012-lapproche-modulaire-en-ia-generative
tags: ai-hacker

---

L'une des idées fondamentales qu'a apporté la science informatique est qu'un problème complexe pouvait être découpé en modules plus gérables. C'est en grande partie sur cette **approche modulaire** que fonctionne l'informatique.

Lorsque vous appuyez sur le bouton "*Démarrer*" de votre ordinateur, lorsque vous tapez sur votre clavier pour écrire un texte à *Microsoft Word* ou lorsque vous mettez l'adresse de votre site préféré dans la barre d'adresses de votre navigateur, le résultat obtenu est d'une complexité que pour arriver à une explication cohérente, on a recours à plusieurs strates, plusieurs niveaux d'explication.

Chaque système informatique, que ce soit le *hardware* ou le *software*, est doté de plusieurs modules et chaque module a une vue **abstraite** (qu'on appelle souvent l'interface du module) et une **implémentation**. Il y a certes une **hiérarchie** entre les modules car les modules du ***haut*** sont implémentés à partir de l'abstraction des modules précédents ou modules du ***bas***.

Cette distinction, cette séparation entre l'abstraction et l'implémentation, sera au cœur de cette recherche sur l'IA générative. Prenons par exemple *Pytorch* ou *Tensorflow*. Ces *frameworks* sont des implémentations d'abstractions que peu de personnes maîtrisent et l'erreur de nombre de formateurs est de présenter uniquement les implémentations sans avoir recours aux abstractions. C'est vrai que je tire la couverture mais une ressource comme [d2l.ai](https://d2l.ai/) met en avance cette séparation abstraction-implémentation.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1712663896961/bccfaa11-81eb-4f87-ad70-fd79ca2ba51d.png align="center")

Comme vous pouvez le voir, un même concept, une "*abstraction*" a plusieurs "*implémentations*" : Pytorch, Tensorflow, Mxnet, Jax.

Si vous suivez l'actualité, vous allez résumer les modules actuels de l'IA à ceci :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1712664499025/749ef700-53ac-44f7-b2cd-0fe5ec8a4092.png align="center")

On vous parle des API proposés par OpenAI, Anhtropic, Microsoft ou Google pour intégrer les fonctionnalités d'IA dans vos applications, de la sortie de tels modèles plus puissants que les autres, de "*transformers*" qui a engendré tous les modèles d'IA générative, des achats de puces GPU Nvidia pour l'entraînement ou l'inférence des modèles...etc. Ce ne sont pas les seuls éléments de l'IA générative.

Petit à petit, les différentes abstractions et implémentations de l'IA générative se mettent en place. C'est ce que nous allons parcourir et aller plus loin car c'est l'innovation sortira forcément de là.

**<mark>CONJECTURES A RETENIR POUR CETTE NOTE :</mark>**

* L'une des idées fondamentales qu'a apporté la science informatique est qu'un problème complexe pouvait être découpé en modules plus gérables. C'est en grande partie sur cette **approche modulaire** que fonctionne l'informatique.
    
* Chaque système informatique, que ce soit le *hardware* ou le *software*, est doté de plusieurs modules et chaque module a une vue **abstraite** (qu'on appelle souvent l'interface du module) et une **implémentation**.
    
* Une abstraction, Une ou plusieurs implémentations.
    
* Les différentes abstractions et implémentations de l'IA générative se mettent en place. Une niche idéale est à cibler.