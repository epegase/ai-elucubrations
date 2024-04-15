---
title: "Note #16 : AI et transformation des inputs"
datePublished: Mon Apr 15 2024 10:52:34 GMT+0000 (Coordinated Universal Time)
cuid: clv0u5qu8000g08l17bipdm3m
slug: note-16-ai-et-transformation-des-inputs
tags: ai-hacker

---

Le NN peut être un bon candidat pour être "*building block*" de base... Après tout, j'ai constaté que même les CNN, RNN et Transformers ont un bloc NN. Mais pour respecter les principes de l'approche modulaire, il faut que les modules aient une certaine indépendance et surtout qu'on comprenne quel est rôle de tel ou tel module, ce qu'il apporte, quelle abstraction il porte,...etc.

C'est un gros travail qu'il faudra faire d'autant plus que la plupart des tutoriels présentent les choses "magiquement"... On peut bien vous expliquer ce qu'est un transformer et cela peut avoir du sens à force de les suivre. Mais le transformer est une abstraction et comment on a fait pour en arriver à cette abstraction ? C'est en comprenant ce processus qu'on peut mieux ressortir les forces et les faiblesses et ainsi avoir un bon champ d'innovations.

Et l'innovation paie aujourd'hui dans l'IA et ça va être le cas au moins ces 2 prochaines années de mon point de vue. Lorsque les "standards" techniques seront arrêtés, la phase de commercialisation battra son essor et c'est la conquête et le contrôle des marchés qui va prendre le relais. Aujourd'hui, aucun marché n'est garanti et du jour au lendemain, tout peut s'écrouler. Une course à la maturité technologique est lancée et le champ est actuellement bien ouvert pour se faire une place techniquement parlant.

J'ai parcouru tout à l'heure un livre, "***Demystifying Deep Learning***" de Douglas J. Santry et l'image ci-bas m'a interpellé :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1713178057362/1be76aec-56d4-4c97-b2db-3a224154c200.png align="center")

(Figure 6.5, page 121, ***Demystifying Deep Learning***, Douglas J. Santry, Wiley, 2024).

On voit bien qu'on a notre bloc NN à la fin et **tout ce qui vient avant est juste une ingénierie sur les inputs** car les valeurs du *tensor* ne sont pas indépendantes et que cette indépendance est une condition pour le bloc NN.

Pour le CNN, les inputs ont une structure puisque ce sont des images. Pareil pour le RNN qui prend en inputs des valeurs séquentielles. Il faut donc réfléchir quels sont les blocs qui interviennent pour transformer par exemple des valeurs séquentielles en valeurs indépendantes prises en charge par le NN... C'est tout l'enjeu du travail de recherche que j'entrevois. Si je réussis à ressortir ces blocs et leur "*pourquoi*" et "*comment*", je pourrai à partir d'une approche comparative essayer de ressortir des similarités utiles pour la suite.

Je n'en suis qu'aux débuts et je ne sais pas où cela va me mener mais je vais continuer dans cette voie.