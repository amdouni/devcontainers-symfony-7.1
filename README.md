Bienvenue à ce Devsecops Labs

Contexte : 

Vous formez une équipe Devsecops chez un acteur leader en e-commerce en France. Vous êtes résponsables de l'accompagnement 
de l'ensemble des équipes de développement et métiers dans la diffusion d'une culture Devsecops et la mise en place d'une Pipeline CI/CD
afin d'améliorer le delivery. 

Installation : 

1 - Connectez-vous à votre compte github
2 - Allez sur le repository : https://github.com/amdouni/devcontainers-symfony-7.1/
3 - Fork le repository et vérifiez qu'il est bien sur votre espace Github

Activités : 

1 - Dans le cadre de la préparation de la Road Map annuelle, votre Delivery Manager Anis a besoin de faire une proposition d'amélioration du processus de delivery. 
Il vous adresse donc un besoin à travers votre Product Owner. Le besoin est inscrit dans le ticket suivant : https://github.com/amdouni/devcontainers-symfony-7.1/issues/1
Apportez les réponses nécessaires à ce besoin. Pour toute question, demandez à votre représentant de l'équipe de l'adresser au métiers. 

Temps estimé de réalisation : 60 minutes


2 - Dans le cadre de l'accueil de Marc, le nouveau stagiaire rattaché à l'équipe de développement, il vous est demandé de lui expliquer notre infrastructure Docker et Docker Compose. Le besoin est exprimé ici : https://github.com/amdouni/devcontainers-symfony-7.1/issues/2

Temps estimé de réalisation : 45 minutes

3 - Myriam est le techlead de l'équipe de développement. Elle cherche une méthode simple de lancer l'application Symfony dans des environnements éphémères. Montrez-lui comment on peut utiliser Github Codespaces pour lancer des applications dans des environnements Dockerisés. 
Pour ce faire : 
a - Allez sur l'onglet Code de votre repository Github. 
b - cherchez le bouton "Use this template" (ou son équivalent en français). Choissez "Open in a codepsace". 
c - Vérifiez que le code space se lance et attendez quelques minutes. Un éditeur de code apparaitra et en quelques minutes votre environnement est en exécution. 

Explorez librement l'éditeur et les options.

Préparer un slide PPT pour décrire ce processus à Myriam.

Temps estimé de réalisation : 45 minutes

4 - Anis, le Delivery Manager a fini par valider l'approche CI/CD à travers Github Actions. L'équipe devsecops de la filiale "Monde" vous a fourni le script Github Actions pour s'en servir comme base. Vous trouverez ce script ici : https://github.com/amdouni/devcontainers-symfony-7.1/blob/main/.github/workflows/ci.yml

Ce script représente les étapes de la pipeline CI/CD qui contient une étape Build et une Etape Analyses et checks. Dans l'étaps analyse et check, trois jobs se lancerons en parallèle : Analyse Statique, lancement des tests unitaires et le security check. 

Pour lancer la pipeline, il faut stimuler un push pour déclencher le processus. Une simple modification de ce ReadMe peut faire le nécessaire par exemple. 

- Commentez le fichier ci.yml pour faciliter à Anis la compréhension de la pipeline.
- Lancez la pipeline en stimulant un push et rapportez les résultats de la pipeline dans un slide PPT.

  Temps estimé : 45 minutes

A terme de ce labs, vous pouvez supprimer le codespace créé et envoyer vos documents PPT et vos fichiers commentés par email à raouf.amdouni@intervenants.efrei.net.

Bon courage,
Raouf AMDOUNI




