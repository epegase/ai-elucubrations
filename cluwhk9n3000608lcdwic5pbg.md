---
title: "Note #015 : Fonctions, vecteurs et matrices"
datePublished: Fri Apr 12 2024 09:48:52 GMT+0000 (Coordinated Universal Time)
cuid: cluwhk9n3000608lcdwic5pbg
slug: note-015-fonctions-vecteurs-et-matrices
tags: ai-hacker

---

L'approche modulaire fait toujours une séparation entre l'abstraction et l'implémentation. Un module est une abstraction, indépendant des autres modules. On n'a pas besoin de savoir comment cela a été implémenté pour l'utiliser. On a juste besoin de savoir ce qu'il a besoin en entrée et ce qu'il produit en sortie.

De façon triviale, on a besoin de savoir ce qu'il faut faire et le résultat une fois que ça donne. C'est lorsque le résultat ne donne pas comme cela doit donner qu'on jette un coup d'oeil à l'intérieur du module, qu'on regarde l'implémentation. Sur les détails de cette tension entre l'abstraction et l'implémentation, vous pouvez lire l'article populaire de Joël Spolsky “[The Law of Leaky Abstractions](https://www.joelonsoftware.com/2002/11/11/the-law-of-leaky-abstractions/)” et tout ce qui est apparenté à ce thème en faisant une petite recherche à Google...

On dit souvent que les NN (*Neural Networks*, réseaux neuronaux) sont des fonctions ou composition de fonctions. Bien sûr que cela est réducteur mais si on reste au niveau de l'abstraction, c'est exactement cela. C'est parce que lorsqu'on parle de fonction, on pense à nos fonctions étudiées en mathématiques, et pour mon cas, je pensais à nos fameuses fonctions linéaires, les plus simples. Et je me disais quel est le lien entre une fonction linéaire et les NN ?

Une fonction est un modèle, un simple modèle mathématique d'un phénomène réel. Si je prend l'exemple du livre "*No Bullshit Guide to Mathematics*" d'[Ivan Savov](https://minireference.com/), supposons que vous voulez modéliser un phénomène réel comme les revenus que vous voulez obtenir d'un concert. Appellons R ces revenus. Les revenus d'un concert dépendent du nombre de tickets vendus. Si chaque ticket coûte 25 Francs, les revenus de ce concert peuvent être modéliser avec la fonction suivante :

<mark>R(n) = 25n</mark>

où n est le nombre de tickets vendus.

Résoudre dans *n* dans l'équation R(n) = 7 000 nous indique le nombre de ventes de billets nécessaires pour générer 7 000 Francs revenus. Il s'agit d'une simple fonction ; Au fur et à mesure que vous glanez les informations, vous pouvez faire "évoluer" la fonction.

Par exemple, si vous devez inclure 5% comme frais d'émission des tickets, vous pouvez mettre à jour la fonction des revenus du concert ainsi :

<mark>R(n) = 0.95 x 25 x n</mark>

Pour revenir à notre thème, une fonction est un objet mathématique qui prend des nombres en inputs et nous donne des nombres en outputs. Vous donnez en *input* le nombre de tickets vendus et vous obtenez en *ouput* les revenus générés par le concert.

Les NN prennent des vecteurs ou matrices en *inputs* et donne des matrices ou vecteurs en *outputs*. Ce sont ces vecteurs ou matrices qui sont appelés “*tensors*” dans les frameworks de machine learning (Tensorflow ou PyTorch).Pourquoi les NN sont concernés par les vecteurs ou matrices ? Simplement parce que les phénomènes modélisés par les NN ont des caractéristiques qui ne peuvent pas être captés par un nombre.

L'intelligence de tout ce qui a conduit à l'IA générative a été de trouver des moyens de modéliser des inputs qui, au départ, étaient non “*consommables*” par les NN pour les rendre “*input-ables*”. Les différentes modifications architecturales des NN avec les propositions de RNN, CNN, LSTM et Transformers visaient à adapter cette architecture à la structure des données.

Par une série d'essais et d'erreurs, les implémentations ont donné de très bons résultats. Et le succès est présent avec l'IA qui fait l'actualité depuis pratiquement deux (02) ans sans interruption. Néanmoins, **je reste convaincu que si je parviens à modulariser une bonne partie de ses avancées, à la manière d'un jeu de Lego, je pourrai déceler plus facilement des foyers d'innovation qui me permettront de percer dans ce sens en y sortant avec une grosse prime d'avant-gardiste**. C'est ce à quoi je m'attellerai toute l'année 2024.

Conséquemment, il faut modulariser les NN, les CNN, les RNN et Transformers. Quels sont les sous-modules, pourquoi ce sous-modules, qu'est ce qui prend en inputs et donne en outputs. C'est cette dissection qui permettra aussi de séparer l'abstraction de l'implémentation. Il faudra toujours garder en tête cette séparation car il n'y a qu'**<mark>une seule abstraction et de multiples implémentations</mark>**.

Un livre comme [d2l.ai](http://d2l.ai) met en exergue très facilement cette séparation entre abstraction et implémentation avec un même concept, une abstraction où elle propose l'implémentation en Tensorflow, PyTorch et autres. Néanmoins, je trouve la présentation de l'abstraction un peu trop abstraite, trop mathématique… Seule une présentation fluide, proche du sens commun permettra de dresser des ponts, des connections utiles pour innover. Voilà mon approche. Sans plus tarder, je me mettrai au travail dans ce sens.