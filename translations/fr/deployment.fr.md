# Deployment check

> **Partie de l’évaluation de la livraison de logiciels à plusieurs équipes** ([README](README.md))
> 
> Droit d’auteur © 2018-2021 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Sous licence [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_ 

Basé sur les questions de maturité de Mirco Hering, auteur de [*DevOps for the Modern Enterprise*](https://notafactoryanymore.com/2018/03/01/mircos-self-assessment-questions-of-devops-maturity/)

But : *Évaluer la confiance de l’équipe dans les pratiques de déploiement de ses logiciels*

Méthode : Utilisez l’approche [*Spotify Squad Health Check*](https://labs.spotify.com/2014/09/16/squad-health-check-model/) pour évaluer les réponses de l’équipe aux questions suivantes :

| **Question**                                                                                                                                 | **Inspiré (1)**                                                        | **Fatigué (5)**                                             |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------ |
| 1\. **Reconstruction d’environnement** - Que se passerait-il si nous décidions de : **vider l’environnement et le reconstruire à partir de notre configuration stockée.** | Nous ne savons pas ce qui se passerait – les environnements sont instables.         | Pas de problème – nous mettons cela à l’essai dans le pipeline de déploiement d’abord. |
| 2\. **Nouvelle configuration** - Que se passerait-il si nous décidions de : **supprimer la configuration de l’application et la redéployer.**                                 | Nous ne savons pas ce qui se passerait – le processus de configuration est instable. | Pas de problème – nous mettons cela à l’essai dans le pipeline de déploiement d’abord. |
| 3\. **Redéployer l’application** - Que se passerait-il si nous décidions de : **redéployer l’application même si rien n’a changé.**                      | Nous ne savons pas ce qui se passerait – les déploiements sont instables.          | Pas de problème – nous mettons cela à l’essai dans le pipeline de déploiement d’abord. |
| 4\. **Réexécution des essais** - Que se passerait-il si nous décidions de : **réexécuter la suite des essais, et ainsi de suite.**                                            | Nous ne savons pas ce qui se passerait – la suite d’essais est vraiment instable.     | Pas de problème – nous mettons cela à l’essai dans le pipeline de |

