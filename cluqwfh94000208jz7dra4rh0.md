---
title: "Note #011 : Nand to Tensor"
datePublished: Mon Apr 08 2024 11:58:26 GMT+0000 (Coordinated Universal Time)
cuid: cluqwfh94000208jz7dra4rh0
slug: note-011-nand-to-tensor
tags: ai-hacker

---

Lors de ma dernière note, la note #010, j'ai dit ceci :

*Il serait mieux, au lieu de me plaindre ou passer mon temps à démontrer que tel a raison ou a tord, autant mieux "casher" là dessus, profiter de ce brouillard et me faire des sous.*

Les 10 premières notes, j'ai passé mon temps à me plaindre. Et ce n'est pas avec cela que je vais avancer. Je vais donc, à partir de cette note, lancer mon programme de recherche en m'appuyant sur le cours "[Nand To Tetris](https://www.nand2tetris.org/)".

Je pars donc d'une idée *folle* qui vise à appliquer le *framework* porté par une ressource comme “***Nand to Tetris***” aux neural networks en général et plus spécifiquement aux IA génératives en vogue aujourd'hui, notamment les nouvelles formes de représentation de données. Cette application vise à ressortir les abstractions exploitables dans le domaine des IA génératives.

“*Nand to Tetris*” part des “*bits patterns*” pour expliciter toutes les abstractions qui permettent d'entrer une information, un input que ce soit du texte, l'image, la vidéo ou l'audio pour obtenir l'output voulu après transformation.

Mon objectif est d'avoir à la fin de cette recherche un cadre de réflexion et d'action devant les innovations qui vont dans tous les sens actuellement dans l'IA générative. Avec un tel cadre, je pourrai déceler une niche sur laquelle bâtir des projets, ou encore copier une initiative jugée allant dans le bon sens.

Bien que j'affirme que l'IA générative actuelle s'appuie sur les “*matrix ou tensor patterns*”, je ne sais pas comment opérationnaliser cela en créant un pont avec “*Nand to Tetris*”. Mais pour y arriver, il faut se poser les bêtes questions, les “*childish questions*” comme le demande Rory Sutherland dans son livre “*Alchemy*” que je suis en train de lire.

Pourquoi on a eu recours aux “*bits patterns*” ? Peut être parce que le traitement, le calcul binaire était plus facile avec l'architecture du CPU… Je ne dis pas que c'est cela puisque je n'ai pas encore abordé en profondeur le cours “*Nand to Tetris*”... C'est juste une conjecture. Comme le CPU permet le calcul séquentiel, c'était plus facile.

Autre bête question : est ce que le “*matrix patterns*” n'est pas à classer dans les “*bit patterns*” ? Certainement puisque même le GPU utilisé fait aussi du calcul binaire. Mais avec un détail : au lieu du calcul séquentiel, le calcul parallèle est possible. Cette possibilité de calcul parallèle est au cœur de l'architecture même du GPU.

Y'a t-il donc contradiction entre les “*bit patterns*” et les “*matrix patterns*” ? Non. Puisque CPU et GPU répondent aux *bits patterns*. C'est plutôt calcul séquentiel contre calcul parallèle. **La question qu'on doit se poser est celle de savoir les conséquences de la normalisation du calcul parallèle sur toutes les abstractions qui ont été établies avec le calcul séquentiel.** Comment revoir ou reconfigurer ces abstractions à la lumière du calcul parallèle ? Ce sont des pistes d'exploration qui seront balayées lors de ces recherches.

Bien sûr, il est difficile de porter tout seul le poids technique d'une telle recherche et il serait prétentieux de penser que j'y arriverai aussi facilement. Néanmoins, je pourrai avoir une ouverture d'esprit sur le développement des IA génératives grâce à ces prétentions erratiques.

De quoi il est question avec les IA génératives ? Simplement de la génération de contenus à partir d'un moteur ou modèle comme le demande le jargon consacré… un modèle d'IA propulsé par les “*neural networks*”. Un modèle qui contient un ensemble d'espaces possibles (*latent space*) et c'est un seul espace qui est sélectionné comme output à partir d'un input appelé “*prompt*”.

Est ce que les abstractions liées au CPU permettaient ces “*latent space*” ? Difficile d'avoir une réponse…

**<mark>CONJECTURES A RETENIR POUR CETTE NOTE :</mark>**

* Le calcul binaire est plus facile avec l'architecture du CPU
    
* La calcul matriciel est plus facile avec l'architecture du GPU
    
* Il n y a pas de contradiction entre les “*bit patterns*” et les “*matrix patterns*”. Puisque CPU et GPU répondent aux *bits patterns*. C'est plutôt calcul séquentiel contre calcul parallèle.
    
* La question qu'on doit se poser est celle de savoir les conséquences de la **normalisation du calcul parallèle sur toutes les abstractions qui ont été établies avec le calcul séquentiel**.
    
* Comment revoir ou reconfigurer ces abstractions à la lumière du calcul parallèle ? Ce sont des pistes d'exploration qui seront balayées lors de ma recherche.
    
* L'objectif est d'avoir à la fin de cette recherche un cadre de réflexion et d'action devant les innovations qui vont dans tous les sens actuellement dans l'IA générative. Avec un tel cadre, je pourrai déceler une niche sur laquelle bâtir des projets, ou encore copier une initiative jugée allant dans le bon sens.