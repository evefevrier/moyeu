# Bilan du cours intégration 2
Édition <time>2021</time>

## Notions et compétences
### Environnements de travail et de déploiement, outils
* Brackets et PHPStorm
* [Extension *Live Edit*](https://www.jetbrains.com/help/phpstorm/live-editing.html#ws_live_edit_activate_procedure)  
:see_no_evil:  __vidéo__: [crs02_installer-live-edit-pour-phpstorm](https://web.microsoftstream.com/video/16b291dd-2882-4721-b224-707604587bf4?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)
* Filezilla comme premier outil de mise en ligne FTP, et en fait: SFTP.  
:see_no_evil:  __vidéo__: [crs01_connexion-sftp-timunix2](https://web.microsoftstream.com/video/0b013dc2-1a37-4eb1-bc40-b1f9bffa0f6a?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)
* Terminal sur Mac ou Invite de commande sur Windows pour connexion SSH  
On réutilise les [notes du cours Profession intégrateur pour les commandes UNIX](documents/notes-de-cours/professionIntegrateur_notes_UNIX-ssh.pdf)  
:see_no_evil:  __vidéo__: [crs01_connexion-ssh](https://web.microsoftstream.com/video/40d7bc3b-3d3f-40e4-9434-26cb70df7615?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)
* Configuration serveurs local et distant dans PHPStorm comme outil de mise en ligne ftp  
:see_no_evil:  __vidéo__ [crs08_configs-serveurs-local-et-distant](https://web.microsoftstream.com/video/b9a9c1b9-0285-48c8-80f9-14033432d63f?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)
* Github comme serveur de versionnage
* Github comme hébergeur Web sécurisé avec https
* Navigateur Chrome, bouton *toggle devices*, inspecteur de code, barre d'outils de développement de Chris Pederick

### Méthodes de travail

#### 1. Approche en amélioration progressive
* Baliser les contenus en HTML <span style="color:red">avant</span> même que le Design ne soit créé
* Schématiser les stratégies d'intégration
* Ajouter les éléments HTML et les classes indispensables à la mise en page
* Ajouter les styles
* Ajouter les comportements (le JavaScript)

#### 2. Intégrer *Mobile First*
Vérifier l'ordre et la disposition des contenus sur l'écran étroit 
avant d'ajouter au fur et à la mesure les variantes pour l'écran large.

#### 3. HTML structurel et sémantique
Voir le [Guide HTML](https://github.com/evefevrier/guide-developpement-web/blob/main/guide-html.md)

#### 4. Schématiser les stratégies d'intégration
Il y aurait une page à ajouter ici pour retracer les méthodes et les exemples selon l'évolution des stratégies d'intégration. 
En gros, il faut identifier graphiquement les conteneurs de centrage, de rangées et de blocs, les conteneurs *flex* ou *grid*.
La syntaxe des sélecteurs CSS, qui est aussi la syntaxe pour générer du HTML avec Emmet, est utilisée pour identifier les éléments HTML qui servent de conteneurs.

#### 5. Utiliser les classes comme sélecteurs
L'objectif est de découpler la structure HTML des CSS en minimisant le recours aux sélecteurs simples.  
La méthode BEM est *adaptée* et *élargie*: les classes de *bloc* peuvent être des composants __ou__ des contextes.  
Voir l'exemple du menu principal et ses modificateurs pour l'entête et le pied de page dans le [Guide CSS](https://github.com/evefevrier/guide-developpement-web/blob/main/guide-css.md).

#### 6. Architecture des fichiers CSS
Voir les explications et les fichiers dans le [cadriciel du guide de développement](https://evefevrier.github.io/guide-developpement-web/cadriciel/index.html), les fichiers se présentent dans l'ordre suivant: 
* reset ou normalize, 
* utilitaires, 
* charte typographique responsive en base décimale, 
* système de grille fluide en flexbox   


### Styles CSS
Notions | Démos, exercices ou TPs
--- | ---
Cascade, spécificité, héritage | Démos et exercices formatifs, test 2
Différence des modèles de boîte, rôle de la propriété box-sizing | Démos, exercices formatifs, test 2 
Flottants et positionnement | Démos, exercice formatif
Mise en page avec des Flexbox | [Jeu](https://flexboxfroggy.com/#fr), Katas, TP2, test 3
Mise en page avec des Flexbox avec système de grille fluide | Démos, TP3, TP4 et TP5, P2
CSS Grids | [Jeu](https://cssgridgarden.com/#fr), [démos](https://github.com/abookapart/new-css-layout-code), P1
Transitions et animations | démos [1](https://codepen.io/evefevrier/pen/mdRvzVB) [2](https://codepen.io/evefevrier/pen/yLgZRKB) [3](https://codepen.io/evefevrier/pen/ZELwmXK) [4](https://codepen.io/evefevrier/pen/poRGQvj) [5](https://codepen.io/evefevrier/pen/qBRgvgQ), TP5, P1 et P2  


### Intégrer des svg 
[Trois manières d'intégrer des svg](documents/notes-de-cours/c16-integrer-des-svg.pdf): balise img, image d'arrière-plan en CSS ou en ligne, c'est-à-dire, le code SVG dans le HTML.


### Accessibilité
Notions | Documents | Exercices ou TPs
--- | --- | ---
Contenus accessibles | [Intro à l'accessibilité](documents/notes-de-cours/c13-notes-intro-a11y.pdf) | exercice formatif, test 4
Contenus accessibles | [Arbre de décision pour texte alternatif](documents/notes-de-cours/c13-arbre-de-decision-pour-alt.pdf) | exercice, test 4
Formulaires accessibles | [Accessibilité des formulaires](documents/notes-de-cours/c14-formulaires-acces-2019.pdf) | [TP4](enonces/enonce-TP4.pdf), [vidéo du corrigé du TP4](https://web.microsoftstream.com/video/d8cc58f7-1028-44f5-a05a-23ae18015549?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844), test 4
Navigation accessible | [Accessibilité de la navigation](documents/notes-de-cours/c17-notes-navigation-accessible.pdf) | [TP5](enonces/enonce-TP5.pdf)


### Optimisation des CSS (concaténation et minification)
#### Méthode de base avec outils en ligne: [autopréfixeur](https://autoprefixer.github.io/) + [cssminifier](https://cssminifier.com/)
:see_no_evil:  __vidéo__: [crs26_optimisation-des-css](https://web.microsoftstream.com/video/f2384057-cb5f-4ff8-a6d6-1f0ff9f8e405?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)  
#### Méthode alternative: avec __sass__ 
:see_no_evil:  __vidéo__: [sass pour optimiser les CSS](https://web.microsoftstream.com/video/52f0997c-7777-46bc-8175-93f79adb0e65?channelId=c6d91a1b-127c-44e9-a6f0-5e15d1b58844)


## Projets synthèses 
La conception et les maquettes des deux projets ont été réalisés dans le cours de Design.
Le traitement des médias et l'optimisation des images d'Anticoste ont été *coachés* principalement dans le cours de Design et complété dans le cours d'intégration.
Le projet Anticoste était aussi arrimé avec le cours d'animation pour la conception et la réalisation d'animations vidéos dans la page titre de chaque récit.

### Anticoste (20%)
Projet collaboratif: chaque groupe classe = une branche du projet.  
Compétences acquises:
* inclure le versionnage dans une routine de travail
* faire relire son code et le partager par des *pull request*
* exprimer un bloquant ou un défi d'intégration en publiant une *issue*  

Voir la doc [Contribuer](https://github.com/evefevrier/anticoste/blob/main/_docs/CONTRIBUER.md)  

### Grilles festives (20%)
Projet individuel.    
Compétence acquise:      
* Expérimenter les grilles css pour intégrer une *Tim Actu*  

Réalisations des étudiant.e.s:  
* [camillemarceau07](https://camillemarceau07.github.io/p1-grille-festive/)
* [amelielarouche](https://amelielarouche.github.io/p1-grille-festive/)
* [olivierlemay](https://olivierlemay.github.io/p1-grille-festive/)
* [lounaparron](https://lounaparron.github.io/p1-grille-festive/)
* [lauryannbelanger](https://lauryannbelanger.github.io/p1-grille-festive/)
* [tristanbernard](https://tristanbernard.github.io/p1-grille-festive/)
* [itsoliroy](https://itsoliroy.github.io/P1-Grilles-Festives/)
* [jeffduval](https://jeffduval.github.io/p1_grilles-festives/)
* [mtrubert](https://mtrubert.github.io/p1-grille-festive/)
* [ferlandalex](https://ferlandalex.github.io/p1-grille-festive/)
* [larochellegabriel](https://larochellegabriel.github.io/p1-grille-festive/)
* [daphneemartel](https://daphneemartel.github.io/p1-grille-festive/)
* [vincent-hebert](https://vincent-hebert.github.io/p1-grille-festive/)
* [wahza](https://wahza.github.io/p1-grille-festive/)
* [leonardoog](https://leonardoog.github.io/p1-grille-festive/)
* [thomaschevarie](https://thomaschevarie.github.io/p1-grille-festive/)

 
