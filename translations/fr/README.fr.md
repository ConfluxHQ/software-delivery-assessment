# Évaluation de la livraison de logiciels à plusieurs équipes

L’évaluation de la livraison de logiciels à plusieurs équipes est une approche simple et facile à exécuter pour évaluer la livraison de logiciels dans de nombreuses équipes différentes dans une organisation. Conçue par [Matthew Skelton](https://github.com/matthewskelton) de [Conflux](https://confluxdigital.net/), elle est utilisée comme élément clé de Software Delivery Assessment à Conflux, mais peut être utilisé librement par n’importe qui (sous réserve de la licence CC BY-SA ci-dessous).

L’évaluation utilise et met à profit le modèle bien connu et éprouvé de [Spotify Squad Health Check model](https://labs.spotify.com/2014/09/16/squad-health-check-model/). 

> Traductions: [Japanese (ja 🇯🇵)](../ja/README.ja.md), [English (en)](/README.md)

L’évaluation porte sur huit dimensions au total :

1. [Santé de l’équipe](team-health.md)
2. [Déploiement](deployment.md)
3. [Flux](flow.md)
4. [Livraison continue](continuous-delivery.md)
5. [Exploitabilité](operability.md)
6. [Essais et testabilité](testability.md)
7. [Fiabilité et IFS](reliability.md)
8. [Sur appel](on-call.md)

Ces huit dimensions couvrent les aspects clés de la livraison de logiciels modernes sous une forme qui permet aux équipes d’évaluer eux-mêmes leurs forces et leurs pratiques.

**🚀 Aperçu**: voir Diapositives 32-38 dans [Continuous Delivery at scale](https://www.slideshare.net/matthewskelton/continuous-delivery-at-scale-matthew-skelton-nhs-digital-agile-cop-march-2019)

**🃏 Jeu de cartes**: Rendre l’évaluation amusante et interactive à l’aide de [the 66-card Software Delivery Assessment printed card deck from Agile Stationery](https://agilestationery.co.uk/pages/software-delivery-assessment). Élaboré en collaboration avec Conflux, le jeu de cartes comporte des indicateurs Fatigué et Inspiré pour chacun des critères d’évaluation, ainsi que des cartes émoticônes pour le vote rapide des membres de l’équipe. Le jeu de cartes fonctionne aussi pour les évaluations à distance!

<img alt="Cartes d'évaluation d'Agile Stationery" title="Cartes d'évaluation d'Agile Stationery" src="../../images/Agile-Stationery-card-deck-MSDA.jpg" width="200" /> <img alt="Cinq cartes de vote emoji" title="Cinq cartes de vote emoji" src="../../images/SDA_Emojis_image2.png" width="200" /> 

> Droit d’auteur © 2018-2021 © 2018-2021 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Sous-licence [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_

## But des évaluations

L’objectif des évaluations est de promouvoir et de maintenir un environnement de travail positif pour le développement et la gestion de systèmes logiciels où :

  - les modifications apportées aux logiciels sont élaborées, testées et déployées en production **rapidement et en toute sécurité** grâce aux pratiques de livraison continue;
  - les processus et les pratiques sont **optimisés pour le flux de changement** vers la production;
  - le logiciel est conçu et développé pour permettre des **déploiements indépendants et découplés** pour des familles séparées de systèmes;
  - le logiciel est conçu et développé de manière à répondre aux exigences **d’exploitabilité**, **de testabilité**, **de capacité de libération** et **de fiabilité**;
  - les problèmes de production sont toujours **détectés par les équipes** avant que les clients et les utilisateurs ne s’en rendent compte;
  - la responsabilité et **l’obligation de rendre compte** des changements logiciels mènent à l’autonomisation et à la propriété;
  - travailler avec un logiciel est **gratifiant** et intéressant;
  - être sur appel et appuyer le logiciel sont **durables et précieux**;
  - les gens se sentent **confiants de contester les mauvaises pratiques** et approches.

Fondamentalement, les évaluations devraient aider à **débloquer et à permettre aux équipes** de réussir. Les évaluations doivent **aider les équipes à améliorer la façon dont elles développent, testent et déploient des systèmes logiciels** en identifiant différents types d’améliorations :

1.  Améliorations axées sur l’équipe.
2.  Améliorations axées sur le produit et sur le service.
3.  Améliorations à l’échelle de l’organisation.

Les évaluations NE doivent PAS être utilisées pour pénaliser les équipes, mais pour fournir une volonté commune d’améliorer les pratiques et la qualité.

## Équipes incluses dans les évaluations

Chaque équipe qui écrit du code, des scripts ou une configuration pour les logiciels d’application ou l’infrastructure bénéficiera de l’inclusion dans les évaluations :

  - Équipes élaborant des **sites Web et des services destinés aux utilisateurs et aux clients**.
  - Équipes élaborant des **services internes.**
  - Équipes élaborant l’**infrastructure** pour appuyer d’autres systèmes (y compris les équipes de plateforme).
  - Équipes élaborant des outils et des scripts de **développement et de déploiement**.
  - Équipes **configurant et testant les produits LCPE** dans le cadre du domaine logiciel et d’infrastructure.
  - Toute autre équipe qui mise principalement sur **l’élaboration, la configuration et la mise à l’essai des logiciels et de l’infrastructure**.

Par « équipe », on entend un groupe de 6 à 10 personnes qui travaille en étroite collaboration, généralement appelé Équipe, Équipe du Scrum, Équipe de produit ou Équipe harmonisée par flux. 

## Critères d’évaluation

Les critères de chaque dimension sont tirés des ouvrages et des sources en ligne existants :

* **Santé de l’équipe** - Fondée sur les critères de [_Spotify Squad Health Check_](https://labs.spotify.com/2014/09/16/squad-health-check-model/) avec quelques ajouts.
* **Déploiement** - Fondé sur les questions clés du livre [_DevOps for the Modern Enterprise_](https://itrevolution.com/book/devops_modern_enterprise/) de Mirco Hering comme abordé dans l’article [Mirco’s self assessment questions of DevOps Maturity](https://notafactoryanymore.com/2018/03/01/mircos-self-assessment-questions-of-devops-maturity/) du blogue de Mirco. 
* **Flux** - Fondé sur les critères du livre [_Accelerate_](https://itrevolution.com/book/accelerate/) de Nicole Forsgren, Jez Humble, et Gene Kim, en plus de certains détails de [_The Principles of Product Development Flow_](https://www.amazon.com/Principles-Product-Development-Flow-Generation/dp/1935401009) de Don Reinertsen.
* **Livraison continue** - onction sur des critères sélectionnés du livre [_Continuous Delivery_](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912) de Jez Humble et Dave Farley et le résumé du livre à [CDchecklist.info](http://CDchecklist.info/)
* **Exploitabilité** - Fondée sur des critères sélectionnés dans le livre [_Team Guide to Software Operability_](http://operabilitybook.com/) de Matthew Skelton, Alex Moore, et Rob Thatcher, ainsi que quelques questions de [OperabilityQuestions.com](http://OperabilityQuestions.com/)
* **Essais et testabilité** - Selon les critères sélectionnés dans les livres [_Agile Testing_](https://wordery.com/agile-testing-lisa-crispin-9780321534460) de Lisa Crispin et Janet Gregory, [_Continuous Delivery_](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912) de Jez Humble and Dave Farley, [_Growing Object-Oriented Software_](https://wordery.com/growing-object-oriented-software-guided-by-tests-steve-freeman-9780321503626) de Steve Freeman et Nat Price, [_Working Effectively with Legacy Code_](https://www.amazon.co.uk/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052) de Michael Feathers, [_Team Guide to Software Testability_](http://testabilitybook.com/) de Ash Winter et Rob Meaney, et [TestabilityQuestions.com](http://TestabilityQuestions.com/).
* **Fiabilité et IFS** - Selon les critères sélectionnés dans les livres [_Site Reliability Engineering_](https://sre.google/sre-book/table-of-contents/) de Betsy Beyer, Chris Jones, Jennifer Petoff, et Niall Murphy, [_The Site Reliability Workbook_](https://sre.google/workbook/table-of-contents/) édité par Betsy Beyer, Niall Richard Murphy, David K. Rensin, Kent Kawahara, et Stephen Thorne, [_Seeking SRE_](https://www.oreilly.com/library/view/seeking-sre/9781491978856/) édité par David N. Blank-Edelman, [_Team Guide to Software Operability_](http://operabilitybook.com/) de Matthew Skelton, Alex Moore, et Rob Thatcher.
* **Sur appel** - Selon les critères sélectionnés des livres [_Site Reliability Engineering_](https://sre.google/sre-book/table-of-contents/) de Betsy Beyer, Chris Jones, Jennifer Petoff, et Niall Murphy, [_The Site Reliability Workbook_](https://sre.google/workbook/table-of-contents/) édité par Betsy Beyer, Niall Richard Murphy, David K. Rensin, Kent Kawahara, et Stephen Thorne, [_Team Guide to Software Operability_](http://operabilitybook.com/) de Matthew Skelton, Alex Moore, et Rob Thatcher.

## Comment exécuter les évaluations

La séance d’évaluation elle-même devrait ressembler à une séance rétrospective d’équipe. La principale différence par rapport à une séance rétrospective normale est que, lors de la séance d’évaluation de l’équipe, l’animateur oriente plus fermement la discussion. Il y a beaucoup de questions à aborder, et il est important que l’équipe discute de tous les critères dans le temps disponible.

À la fin de la séance d’évaluation, l’équipe devrait se sentir encouragée et habilitée à décider des mesures qu’elle souhaite prendre pour améliorer ses processus et ses pratiques en se fondant sur les discussions.

### Fréquence

De nombreuses organisations jugent que l’évaluation des équipes **tous les trois mois** donne de bons résultats.

### Préparation

1.  Trouvez quelqu’un pour faciliter l’évaluation. Il devrait s’agir de quelqu’un de l’extérieur de l’équipe, qui connaît bien les rétrospectives de l’équipe d’exécution.   
2.  Réservez un créneau horaire de deux ou trois heures : pour les séances en ligne, vous pouvez les répartir sur deux séances d’appel vidéo ou plus, et pour les séances en personne, réservez une salle assez grande pour l’équipe.
3.  Pour les séances en ligne, utilisez le jeu de cartes de Agile Stationery et la capture d’écran ou notez les résultats dans une feuille de calcul, ou utilisez un outil de sondage en ligne pour consigner les réponses des personnes à la séance. Pour les **séances en personne**, utilisez le jeu de cartes de Agile Stationery, ou imprimez les feuilles d’évaluation pour chaque ensemble de critères, soit en utilisant le PDF A1 prêt à l’emploi (voir Versions), soit les pages d’évaluation individuelles de taille A1 si possible (utilisez de petites marges) :
	* [Santé de l’équipe – fiche d’évaluation](print/print-team-health.md)
	* [Déploiement – fiche d’évaluation](print/print-deployment.md)
	* [Flux – fiche d’évaluation](print/print-flow.md)
	* [Livraison continue – fiche d’évaluation](print/print-continuous-delivery.md)
	* [Exploitabilité – fiche d’évaluation](print/print-operability.md)
	* [Essais et testabilité – fiche d’évaluation](print/print-testability.md)
	* [Fiabilité et IFS – fiche d’évaluation](print/print-reliability.md)
	* [Sur appel – fiche d’évaluation](print/print-on-call.md)
4.  Pour **les séances en ligne**, affichez les critères Fatigué et Inspiré à l’écran en même temps que la question. Pour **les séances en personne**, imprimez les pages de détails comme guide ou ouvrez-les à l’écran pour comprendre le contexte et les détails de chacun des critères d’évaluation :
	1. [Santé de l’équipe](team-health.md)
	2. [Déploiement](deployment.md)
	3. [Flux](flow.md)
	4. [Livraison continue](continuous-delivery.md)
	5. [Exploitabilité](operability.md)
	6. [Essais et testabilité](testability.md)
	7. [Fiabilité et IFS](reliability.md)
	8. [Sur appel](on-call.md)
5.  Il est utile de saisir les détails et les nuances des discussions entourant chaque question. Pour **les séances en ligne**, demandez à quelqu’un de prendre des notes dans un document ou un tableau blanc partagé. Pour **les séances en personne**, apportez beaucoup de stylos marqueurs ou de marqueurs de tableau blanc : le rouge, le bleu et le vert sont les meilleures couleurs.
6.  Incluez dans la séance une **personne qui sait animer des rétrospectives** (peut-être un maître du scrum). Ils suivront l’animateur pendant la séance afin que la personne de votre équipe puisse animer d’autres séances d’évaluation plus tard.

Assurez-vous que l’animateur comprend le but de la séance et qu’il connaît bien les pages et les questions de l’évaluation.

> **Animateurs**
> 
> L’animateur doit se familiariser avec l’approche [Spotify Squad Health Check](https://labs.spotify.com/2014/09/16/squad-health-check-model/) avant d’exécuter la séance. Voir [How I Used the Spotify Squad Health Check Model](http://www.barryovereem.com/how-i-used-the-spotify-squad-health-check-model/) our un bon rapport sur l’expérience, [Squad Health Checks](https://engineering.skybettingandgaming.com/2017/02/01/squad-health-checks/) de SkyBet, et téléchargez les instructions de Spotify ([PDF](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model2.pdf)).
>
> Au cours de l’évaluation :
> 
> *	tenez l’équipe à l’heure prévue en demandant que certaines discussions se tiennent en dehors de la séance;
> * rédigez les notes et les commentaires de l’équipe sur les fiches d’évaluation imprimées ou assurez-vous que les notes et les commentaires sont saisis dans un outil numérique;
> * prenez des photographies des fiches d’évaluation remplies pour **les séances en personne**;
> * obtenez la rétroaction de l’équipe sur la VALEUR et l’EXÉCUTION de l’évaluation technique – les émoticônes souriants sont assez!
> 

### Horaire

Chaque évaluation de l’équipe dure deux à trois heures, et l’animateur dirigera l’équipe au moyen de huit séries de questions :

1.  Vérification de la santé de l’équipe - **35 mins**
2.  Vérification de l’état du déploiement  - **10 mins**
3.  Vérification du flux - **10 mins**
4.  Vérification de livraison continue  - **20 mins**
5.  Vérification de l’exploitabilité - **20 mins**
6.  Vérification de la couverture des essais - **20 mins**
7.  Fiabilité et IFS - **30 mins**
8.  Sur appel - **15 mins**

Cet horaire laisse place à une **pause de 10 minutes** pendant l’évaluation.

### Exécution de la séance d’évaluation

Chaque section comporte plusieurs questions. On doit répondre à chaque question comme suit :

  - L’équipe (soit à titre individuel, soit à titre d’équipe) évalue chacun des critères à l’aide de TRISTE (1 OU 2)/PFFF (3)/OUAIS (4 OU 5) selon les directives ***Fatigué* et *Inspiré***.
    
      - *Fatigué* correspond à une faible cote (1), et *Inspiré* correspond à une cote élevée (5).
    
      - Si vous avez utilisé des évaluations individuelles, regroupez les évaluations ou décidez d’une note d’équipe unique entre 1 et 5. Vous pouvez trouver utile d’utiliser différents stylos colorés sur la fiche imprimée pour indiquer visuellement les différentes évaluations.

  - La **tendance** depuis la période précédente est indiquée (en hausse, en demeurant à peu près la même, en baisse), le cas échéant.

  - Une **mesure** convenue pour améliorer la note à cette question au cours des prochains mois.

  - Utilisez la colonne **Notes** pour indiquer d’autres renseignements que vous pensez utiles pour l’équipe de coordination.

  - Assurez-vous de remplir les détails **Date/Nom/Animateur**.

  - Pour les séances en personne, prenez une photo de chaque fiche remplie et envoyez-la à la personne qui coordonne les évaluations.

  -  Demandez aux membres de l’équipe d’évaluer la séance d’évaluation elle-même en fonction des éléments suivants : **Valeur**, **Exécution** (visages triste, agacé, heureux).

### Animation virale

Chaque séance d’évaluation de l’équipe présente une personne qui suit l’animateur afin qu’elle puisse faciliter elle-même les séances futures. Chaque nouvel animateur devrait animer au moins deux séances avec d’autres équipes. De cette façon, le nombre d’animateurs augmente rapidement, ce qui permet un fardeau minimal pour les animateurs initiaux.

## Coordination et interprétation des résultats

Une fois que les équipes ont organisé une séance d’évaluation et envoyé leurs résultats, le groupe de coordination doit recueillir les résultats des différentes équipes afin d’identifier les domaines qui doivent être améliorés dans l’ensemble de l’organisation. Posez des questions comme les suivantes :

* Pourquoi l’équipe ABC se note-t-elle à 1 pour la couverture des essais? Qu’est-ce qui les gêne?
* Que pouvons-nous faire en tant qu’organisation pour aider plus d’équipes à effectuer des déploiements?
* Y a-t-il un aspect de la Plateforme qui doit être amélioré pour que les équipes puissent aller plus vite?

N’essayez pas de classer ou de comparer directement les équipes. Au lieu de cela, utilisez les signaux des équipes pour mieux comprendre la dynamique organisationnelle, puis prioriser les améliorations à l’échelle de l’organisation.