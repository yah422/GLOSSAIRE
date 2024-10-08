# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)


## Général

1. Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte
Un ensemble de logiciels libres facilitant l'installation d'un serveur web local. Il comprend Apache (le serveur web), MySQL (la base de données), PHP.
Par exemple XAMPP et WAMPSERVER.

2. Qu’est-ce qu’un algorithme ?
Un algorithme est une série d'étapes précises pour accomplir une tâche ou résoudre un problème, souvent utilisé en informatique.

3. Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?
Une variable est un conteneur pour stocker des données, comme des nombres, des chaînes de caractères ou des tableaux, identifiés par un nom précédé du signe "$".

4. Qu’est-ce que la portée d’une variable ?
La portée d'une variable indique où cette variable peut être utilisée dans votre code. 
Une variable peut être accessible uniquement à l'endroit où elle est créée (portée locale) ou disponible partout dans le script (portée globale).

5. Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?
Une constante est un identifiant associé à une valeur fixe qui ne change pas. 
Elle diffère d'une variable qui peut varier pendant l'exécution et a des portées locales ou globales.


6. Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation
Une superglobale est une variable prédéfinie utilisée pour accéder à des données globales. 
Il existe neuf superglobales, dont `$_GET`, `$_POST`et `$_SESSION`. 
Par exemple, `$_GET` est utilisée pour récupérer des données depuis l'URL dans un formulaire HTML.

7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)
En PHP, les types primitifs associables à une variable sont les entiers INT, nombres à virgule FLOAT, chaînes de caractères STRING, booléens, tableaux ARRAY, objets et NULL.

8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?
En PHP, il existe plusieurs types de tableaux, notamment les tableaux numériques (indexés), les tableaux associatifs (utilisant des clés associatives) et les tableaux multidimensionnels (contenant des tableaux à plusieurs niveaux).

9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles
Les différentes structures de contrôle en algorithmie sont : la structure conditionnelle (ex: if-else), la boucle (ex: for, while), et la structure de séquence (ex: exécution linéaire)

10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?
La fonction PHP permettant de demander la longueur d'une chaîne de caractères est strlen()

11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP
Une session en PHP est un moyen de stocker des données utilisateur sur le serveur. La fonction PHP permettant de démarrer une session est session_start()

12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP
Un cookie en PHP est un petit fichier stocké sur l'ordinateur client, contenant des informations sur l'utilisateur.
exemple : setcookie("prefered_language", "fr", time() + (24 * 3600), "/");

13.	Quelle est la différence entre les instructions « require » et « include » en PHP
La différence entre les instructions "require" et "include" en PHP est que "require" génère une erreur fatale si le fichier inclus n'est pas trouvé, tandis que "include" génère seulement un avertissement.

14.	Comment effectuer une redirection en PHP ?
Pour effectuer une redirection en PHP, on utilise la fonction header() avec l'en-tête "Location"

15.	Définir la partie « front-end » et « back-end » d’une application
La partie "front-end" d'une application se réfère à la partie visible et interactive que l'utilisateur voit et utilise directement, tandis que la partie "back-end" se réfère à la partie du système qui gère les fonctionnalités en arrière-plan et interagit avec le serveur.

16.	Définir le contrôle de version ? Qu’est-ce que Git ?
Le contrôle de version est un système qui enregistre les modifications apportées à un projet au fil du temps. Git est un logiciel de contrôle de version populaire utilisé pour suivre les modifications du code source

17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples
Un CMS (Content Management System) est une application logicielle permettant de créer, gérer et organiser le contenu d'un site web sans nécessiter de compétences techniques avancées en programmation. Deux exemples de CMS sont WordPress et Drupal.


## Front-end

18.	Définir HTML
HTML (HyperText Markup Language) est un langage de balisage utilisé pour structurer et présenter le contenu sur le Web. Il permet de définir la structure des documents en utilisant des balises pour marquer différents types de contenu, tels que du texte, des images, des liens, etc.

19.	Définir CSS
CSS (Cascading Style Sheets) est un langage de feuilles de style utilisé pour styliser et mettre en forme les documents HTML. Il permet de contrôler l'apparence des éléments HTML en définissant des règles de style telles que la couleur, la taille, la police, la disposition, etc.

20.	Définir Javascript
Javascript est un langage de programmation de scripts principalement utilisé pour rendre les pages web interactives et dynamiques. Il est souvent utilisé pour manipuler le contenu HTML, interagir avec l'utilisateur, et effectuer des actions en réponse à des événements.

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 
JSON (JavaScript Object Notation) est un format léger d'échange de données utilisé pour stocker et échanger des données structurées entre un serveur et un client. Il est souvent utilisé dans les applications web pour transférer des données entre le serveur et le navigateur
On utilise JSON dans le contexte des échanges de données entre le serveur et le client, comme les réponses aux requêtes AJAX, les configurations de l'application, etc

22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?
Non, Javascript est principalement un langage de programmation côté client, exécuté par le navigateur web. Cependant, avec l'utilisation de moteurs d'exécution de Javascript côté serveur tels que Node.js, il est possible d'exécuter du Javascript côté serveur.

23.	Qu’est-ce qu’un sélecteur CSS ?
Un sélecteur CSS est une expression qui permet de cibler des éléments HTML spécifiques pour leur appliquer des styles. Les sélecteurs CSS peuvent être basés sur différents critères tels que les balises HTML, les classes, les id, les attributs, etc.

24.	Quelle balise HTML permet de créer un lien hypertexte ?
La balise HTML <a> permet de créer un lien hypertexte

25.	Qu’est-ce qu’une requête AJAX ?
Une requête AJAX (Asynchronous JavaScript and XML) est une technique de développement web qui permet d'envoyer et de recevoir des données du serveur en arrière-plan, sans avoir à recharger toute la page web. Cela permet de créer des applications web plus dynamiques et interactives

26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?
Pour sélectionner tous les éléments d'une classe spécifique en CSS, on utilise le sélecteur de classe ".". Pour sélectionner un élément par son identifiant, on utilise le sélecteur d'identifiant "#"

27.	Définir le responsive design
Le responsive design signifie simplement concevoir des sites web qui s'adaptent à différents appareils et tailles d'écrans en utilisant des techniques flexibles de mise en page et des règles CSS spécifiques

28.	Qu’est-ce que le templating ?
Le templating est un processus de création de modèles de conception réutilisables pour générer dynamiquement des pages web. Il permet de séparer la structure et le contenu d'une page en utilisant des modèles pré-définis dans lesquels le contenu est injecté dynamiquement.

29.	Qu’est-ce qu’une fonction anonyme en Javascript ?
Une fonction anonyme en Javascript est une fonction qui n'a pas de nom et qui est définie de manière littérale. Elle est souvent utilisée comme argument pour d'autres fonctions ou pour créer des expressions de fonction

30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?
La méthode JavaScript utilisée pour ajouter un élément à la fin d'un tableau est "push()"

31.	Qu’est-ce qu’un « media query » ?
Un media query en CSS ajuste les styles en fonction des caractéristiques du périphérique utilisateur comme la taille de l'écran, permettant des mises en page adaptatives et réactives

32.	Qu’est-ce qu’un pseudo élément en CSS ?
Un pseudo-élément en CSS permet de styliser une partie spécifique d'un élément HTML en utilisant des mots-clés tels que :before et :after pour ajouter du contenu ou modifier son apparence

33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent
Bootstrap est un framework front-end populaire pour les sites web réactifs, offrant des outils CSS et JavaScript pré-stylisés. D'autres alternatives incluent Foundation, Materialize et Bulma

34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes
Lorsqu'un formulaire HTML est créé, les deux méthodes qui peuvent lui être associées sont GET et POST. La méthode GET envoie les données du formulaire dans l'URL, tandis que la méthode POST envoie les données du formulaire dans le corps de la requête HTTP, ce qui les rend invisibles dans l'URL et plus appropriées pour l'envoi de données sensibles


## UX UI

35.	Quelle est la différence entre UX Design et UI Design ?
UX Design se concentre sur l'expérience globale de l'utilisateur, tandis que UI Design se focalise sur l'apparence et l'interaction de l'interface utilisateur

36.	Qu’est-ce qu’un wireframe ?
Un wireframe est comme un croquis basique de l'apparence d'un site web ou d'une application, utilisé pour organiser les éléments sans se préoccuper des détails graphiques

37.	Qu’est-ce qu’un prototype ? 
Un prototype est une version initiale d'un produit ou d'une partie de produit utilisée pour tester des idées et des fonctionnalités avant le développement complet

38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?
La hiérarchie visuelle en UI Design consiste à organiser les éléments de manière à ce que les plus importants soient mis en avant, permettant aux utilisateurs de naviguer facilement dans l'interface

39.	Qu’est-ce que l’accessibilité en UX Design ? 
L'accessibilité en UX Design consiste à rendre les produits numériques faciles à utiliser pour tous, y compris les personnes handicapées ou ayant des besoins spéciaux, en concevant des interfaces adaptées à leurs besoins

40.	Qu’est-ce qu’une grille de mise en page ?
Une grille de mise en page est un système de lignes utilisé pour organiser visuellement le contenu sur une page web ou une application

41.	Qu’est-ce que la notion d’affordance en UX Design ?
L'affordance en UX Design fait référence à la capacité d'un élément d'interface à suggérer sa fonction ou son utilisation

42.	Qu’est-ce qu’un « mobile first design » ?
Le "mobile first design" est une approche de conception qui consiste à créer d'abord une expérience utilisateur optimisée pour les appareils mobiles, puis à l'adapter aux écrans plus grands


IV. Programmation orientée objet (POO)

43.	Donner une définition de la programmation orientée objet 
La POO organise un programme autour d'objets représentant des entités réelles, avec des caractéristiques et des actions

44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?
Une classe est un modèle pour créer des objets, déclarée avec le mot-clé class

45.	Qu’est-ce qu’un objet ?
Un objet est une instance d'une classe, possédant des attributs et des méthodes

46.	Définir la notion de propriété / attribut / méthode
Propriété/Attribut : caractéristique d'un objet 
Méthode : action que l'objet peut effectuer

47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité
La visibilité d'une propriété ou d'une méthode définit son accessibilité depuis d'autres parties du programme. Les différents types de visibilité sont : "public", "protected" et "private"

48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?
Pour créer un nouvel objet à partir d'une classe, on utilise la méthode spécifique appelée le constructeur, qui porte le même nom que la classe

49.	Qu’est-ce que l’encapsulation ?
L'encapsulation est le principe qui consiste à regrouper les données (propriétés) et les méthodes qui les manipulent au sein d'un même objet.
Cela permet de contrôler l'accès aux données et de les protéger de toute modification non autorisée

50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple
Étendre une classe signifie créer une nouvelle classe en se basant sur une classe existante, en héritant de ses propriétés et de ses méthodes. Le concept clé mis en œuvre est l'héritage (extends). Par exemple, une classe Voiture peut étendre une classe VoitureElectrique

51.	Définir l’opérateur de résolution de portée
L'opérateur de résolution de portée "(::)" est utilisé pour accéder aux méthodes et aux propriétés statiques d'une classe

52.	Définir une méthode / propriété statique
Une méthode ou une propriété statique est associée à la classe elle-même plutôt qu'à une instance spécifique de la classe. Elles sont accessibles sans nécessiter une instance de la classe

53.	Définir le polymorphisme en POO
Le polymorphisme en POO fait référence à la capacité d'objets de différentes classes à être traités de manière uniforme s'ils partagent une interface commune

54.	Définir une méthode / classe abstraite ?
Une méthode ou une classe abstraite est une classe qui ne peut pas être instanciée elle-même mais qui peut servir de modèle pour d'autres classes

55.	Définir le chaînage de méthodes
Le chaînage de méthodes consiste à appeler plusieurs méthodes d'un objet successivement sur la même ligne de code

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »
La méthode __toString() est une méthode magique qui est automatiquement appelée lorsqu'un objet est utilisé dans un contexte de chaîne de caractères. D'autres méthodes magiques incluent __construct(), __get(), __set(), etc

57.	Qu’est-ce qu’un « autoload » ?
L'autoload est un mécanisme qui permet de charger automatiquement les classes PHP lorsqu'elles sont utilisées pour la première fois dans un script

58.	Comment appelle-t-on en français les « getters » et les « setters » ?
En français, les getters sont appelés des "accesseurs" et les setters sont appelés des "mutateurs"

59.	Qu’est-ce que la sérialisation en PHP ?
La sérialisation en PHP est le processus de conversion d'objets en une représentation de chaîne de caractères


## Architecture 

60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence
L'architecture client/serveur est un modèle dans lequel les tâches sont réparties entre les ordinateurs client et un serveur central. 
Les requêtes sont utilisées pour interroger le serveur. L'acronyme de ce type de requête est HTTP (Hypertext Transfer Protocol). 
En ajoutant un "S" à cet acronyme, cela signifie HTTPS, où la communication est sécurisée par un protocole SSL/TLS

61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern
Un design pattern est une solution réutilisable à un problème récurrent dans le développement logiciel. 
Trois exemples de design pattern sont : Singleton, Factory Method, et Observer

62.	Qu’est-ce que l’architecture MVC ?
L'architecture MVC (Modèle-Vue-Contrôleur) est un modèle de conception utilisé dans le développement logiciel pour séparer les responsabilités des différentes parties d'une application

63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?
Dans l'architecture MVC, le rôle de chaque couche est le suivant :

Le Model représente les données et la logique métier de l'application.
La View est responsable de l'affichage des données et de l'interface utilisateur.
Le Controller agit comme un intermédiaire entre le Model et la View, traitant les requêtes de l'utilisateur et mettant à jour les données en conséquence

64.	Quels sont les avantages de l’architecture MVC ?
Les avantages de l'architecture MVC sont : 
- la séparation claire des préoccupations
- la facilité de maintenance et de test
- la réutilisabilité du code
- la possibilité de travailler en parallèle sur les différentes parties de l'application

65.	Existe-t-il des variantes à l’architecture MVC ?
Oui, il existe des variantes à l'architecture MVC, telles que MVVM (Modèle-Vue-VueModèle), MVP (Modèle-Vue-Présentateur), et HMVC (Hierarchical Model-View-Controller), qui s'adaptent à différents besoins et contextes

66.	Qu’est-ce qu’une API ? Définir l’architecture REST
Une API (Interface de Programmation Applicative) est un ensemble de règles et de protocoles qui permettent à différents logiciels de communiquer entre eux. 
L'architecture REST (Representational State Transfer) est un style d'architecture pour la conception de systèmes distribués, où les ressources sont représentées par des URI (Uniform Resource Identifier) et manipulées à travers des méthodes standardisées (GET, POST, PUT, DELETE)


## Modélisation - Base de données

67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise
La modélisation de données est le processus de conception et de représentation des données et de leurs relations dans un système d'information. 
La méthode Merise est une méthode de modélisation de données utilisée pour structurer les processus de développement de systèmes d'information

68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation ==> Bonne réponse 
b.	Planification, exécution et contrôle
c.	Création, modification et suppression


69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?
Un modèle conceptuel de données (MCD) en Merise représente les entités, leurs attributs et leurs relations dans un système d'information

70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?
Un modèle logique de données (MLD) en Merise est une représentation des données prenant en compte les contraintes de stockage et d'optimisation, telles que les types de données, les index et les clés

71.	Donner la définition des mots suivants :
a.	Entité
Une entité représente un objet ou un concept du monde réel qui peut être identifié et décrit dans un système d'information

b.	Relation
 Une relation représente une association entre deux entités dans un modèle de données

c.	Cardinalité
La cardinalité indique le nombre d'occurrences d'une entité qui peuvent être associées à une occurrence d'une autre entité à travers une relation

d.	Clé primaire / clé étrangère
Une clé primaire est un attribut ou un ensemble d'attributs qui identifie de manière unique chaque occurrence d'une entité. 
Une clé étrangère est un attribut qui fait référence à la clé primaire d'une autre entité, établissant ainsi une relation entre les entités


72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?
Une relation de type "Many To Many" dans le modèle logique de données devient une table de liaison (ou table associative) contenant les clés primaires des entités associées, permettant de gérer efficacement les associations multiples entre les entités

73.	Qu’est-ce qu’une base de données ?
Une base de données est un ensemble organisé de données structurées, généralement stockées électroniquement dans un système informatique. 
Elle permet de stocker, de manipuler et de récupérer des informations de manière efficace

74.	Définir les notions suivantes : 
a.	SQL
SQL (Structured Query Language) est un langage de requête standardisé utilisé pour communiquer avec les bases de données relationnelles

b.	MySQL
MySQL est un système de gestion de base de données relationnelle open source largement utilisé

c.	SGBD (donner 2 exemples de SGBD)
SGBD (Système de Gestion de Base de Données) est un logiciel qui permet de gérer des bases de données. Deux exemples de SGBD sont Oracle et PostgreSQL

75.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___
-1- table
-2- enrengistrements ou tuples
-3- attributs

76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?
Une base de données relationnelle organise les données en tables liées les unes aux autres par des relations définies, 
tandis qu'une base de données non relationnelle stocke les données d'une manière plus flexible, souvent en utilisant des structures telles que des documents ou des graphes

77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?
Une jointure dans une base de données permet de combiner les données de deux tables en fonction d'une condition spécifiée. 
Il existe plusieurs types de jointures, notamment les jointures internes INNER, externes (gauche LEFT, droite RIGHT et complète FULL), et les jointures croisées

78.	A quoi sert une vue dans une base de données ?
Une vue dans une base de données est comme une table virtuelle préparée à l'avance. 
Elle simplifie la façon dont vous accédez aux données en fournissant une vue spécifique sans changer la structure principale de la base de données. 

79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?
L'intégrité référentielle dans une base de données assure que les liens entre les tables restent cohérents. 
En d'autres termes, une valeur dans une table doit correspondre à une valeur existante dans une autre table, souvent via des clés étrangères.

80.	Quelles sont les fonctions d’agrégation en SQL ?
Les fonctions d'agrégation en SQL permettent de calculer des valeurs résumées à partir d'un ensemble de lignes. 
Elles incluent des fonctions telles que SUM, AVG, COUNT, MAX et MIN

81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?
CRUD est un acronyme pour Create (Créer), Read (Lire), Update (Mettre à jour) et Delete (Supprimer). 
Il représente les opérations de base effectuées sur les données dans une base de données

82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
INSERT INTO

b.	Modifier un enregistrement dans une table
UPDATE

c.	Supprimer un enregistrement dans une table
DELETE FROM

d.	Supprimer la base de données
DROP DATABASE

e.	Filtrer les résultats d’une requête SQL
WHERE

f.	Trier les résultats d’une requête SELECT
ORDER BY

g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
GROUP BY

h.	Concaténer 2 chaînes de caractères 
CONCAT

83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?
Pour se connecter à une base de données en PHP, on utilise généralement la classe native 'PDO' (PHP Data Objects) ou 'mysqli' (MySQL Improved). 
Avec PDO, on peut se connecter à différents types de bases de données en utilisant des pilotes spécifiques à chaque base de données.


## Symfony

84.	Qu’est-ce que Symfony ? 
Symfony est un framework PHP utilisé pour développer des applications web. Il offre une structure solide et des outils pour simplifier le développement.

86.	Sur quel langage de programmation et design pattern repose Symfony ? 
Symfony repose sur le langage de programmation PHP et suit principalement le design pattern MVC (Modèle-Vue-Contrôleur).

87.	Quelle est la dernière version en date de Symfony ?
La dernière version stable de Symfony est la version 7.1.4, publiée le 30 août 2024. Elle fait partie de la branche 7.1 et nécessite PHP 8.2 ou une version ultérieure pour fonctionner

89.	Qu’est-ce qu’un bundle ? 
Un bundle est un ensemble de fichiers (code, templates, configuration) qui fournit des fonctionnalités spécifiques dans un projet Symfony. C'est l'équivalent d'un module ou d'un plugin.

90.	Quel est le moteur de template utilisé par défaut dans Symfony ?
Le moteur de template utilisé par défaut dans Symfony est Twig.

91.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
Un ORM (Object-Relational Mapping) est un outil qui permet de gérer les bases de données en manipulant des objets PHP au lieu d'écrire des requêtes SQL. Dans Symfony, l'ORM utilisé est Doctrine.

92.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
L'injection de dépendances est une technique où les dépendances (services, objets) d'une classe sont passées directement à celle-ci, plutôt que d'être créées à l'intérieur de la classe. L'outil utilisé pour gérer cela dans Symfony est le container de services. Le fichier services.yaml contient la configuration des dépendances du projet.

93.	Que permet le bundle Maker au sein de Symfony ? 
Le bundle Maker permet de générer du code de manière automatisée dans Symfony, comme des contrôleurs, des entités ou des formulaires, facilitant ainsi le développement.

94.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
Le langage de requêtage exploité est DQL (Doctrine Query Language), qui est utilisé pour interagir avec la base de données via Doctrine.

95.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?
Le composant qui garantit l'authentification et l'autorisation des utilisateurs dans Symfony est le Security Component.


## Sécurité

94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
Injection SQL : C'est une attaque où un pirate insère du code SQL malveillant dans une requête pour accéder ou modifier les données d'une base de données.
Se prémunir : Utiliser des requêtes préparées avec des paramètres, valider et échapper les entrées utilisateur.

95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
Faille XSS (Cross-Site Scripting) : C'est une attaque où un pirate injecte du code JavaScript malveillant dans une page web, qui est ensuite exécuté par les utilisateurs.
Se prémunir : Échapper les données affichées, désactiver les balises HTML dangereuses dans les entrées utilisateur.

96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
Faille CSRF (Cross-Site Request Forgery) : C'est une attaque où un pirate force un utilisateur à exécuter une action non désirée sur un site où il est authentifié.
Se prémunir : Utiliser des tokens CSRF pour valider les requêtes, vérifier l'origine des requêtes (en-têtes Referer).

97.	Définir l’attaque par force brute et l’attaque par dictionnaire
Force brute : Essayer toutes les combinaisons possibles de mots de passe jusqu'à trouver le bon.
Attaque par dictionnaire : Essayer une liste de mots de passe courants ou pré-compilés (dictionnaire) pour deviner le mot de passe.

98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
Failles de sécurité :
Failles de type RCE (Remote Code Execution) : Permet à un pirate d'exécuter du code malveillant à distance sur un serveur.
Failles de type DoS (Denial of Service) : Saturer un service ou un serveur pour le rendre indisponible.
Failles de type LFI/RFI (Local/Remote File Inclusion) : Permet à un pirate d'inclure des fichiers locaux ou distants dans une application.

99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
Authentification : Vérifier l'identité d'un utilisateur (ex : login/mot de passe).
Autorisation : Déterminer les actions ou ressources auxquelles un utilisateur authentifié a accès.

100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
Hachage d’un mot de passe : Transformer un mot de passe en une chaîne de caractères (empreinte) à sens unique, difficilement réversible.
Algorithmes de hachage : bcrypt, SHA-256, Argon2.

101.	Qu’est-ce qu’une politique de mots de passe forts ?
Politique de mots de passe forts : Imposer des critères pour les mots de passe (longueur minimale, mélange de majuscules, minuscules, chiffres et symboles) pour augmenter leur sécurité.

102.	Qu’est-ce que l’hameçonnage ?
Hameçonnage (Phishing) : Une attaque où un pirate se fait passer pour une entité légitime pour tromper les utilisateurs et obtenir leurs informations sensibles (mots de passe, numéros de carte de crédit).

103.	Définir la « validation des entrées »
Validation des entrées : Vérifier et filtrer toutes les données fournies par les utilisateurs pour s'assurer qu'elles sont conformes aux attentes avant de les traiter, évitant ainsi des comportements inattendus ou dangereux.


## RGPD
104. Qu’est-ce que le RGPD ? 
Le RGPD (Règlement Général sur la Protection des Données) est une réglementation de l'Union Européenne visant à protéger les données personnelles des citoyens
105. Quel est son objectif principal ? 
Son objectif principal est de protéger la vie privée des individus en réglementant la collecte, l'utilisation, et le stockage de leurs données personnelles
106. Quelle est la date d’entrée en vigueur du RGPD ? 
Le RGPD est entré en vigueur le 25 mai 2018
107. Quelles sont les sanctions possibles en cas de non-respect du RGPD ? 
Les sanctions peuvent aller jusqu'à 20 millions d'euros ou 4 % du chiffre d'affaires annuel mondial de l'entreprise, selon le montant le plus élevé
108. En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ? 
C'est la CNIL (Commission Nationale de l'Informatique et des Libertés)

109. Quel est le consentement valide selon le RPGD ? 
Le consentement doit être libre, éclairé, spécifique et univoque. L'utilisateur doit donner son accord de manière claire et affirmative
110. Qu’est-ce qu’une politique de confidentialité ?
 C'est un document qui explique comment une organisation collecte, utilise, partage et protège les données personnelles des utilisateurs
111. Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
Le RGPD ne fixe pas de durée maximale spécifique, mais les données ne doivent être conservées que le temps nécessaire aux finalités pour lesquelles elles ont été collectées
112. Quels sont les droits des utilisateurs selon le RGPD ? 
Les utilisateurs ont plusieurs droits, dont le droit d'accès, de rectification, d'effacement, à la limitation du traitement, à la portabilité des données, et d'opposition
113. Qu’est-ce que le principe de minimisation des données selon le RGPD ? 
C'est le principe selon lequel seules les données personnelles nécessaires à la finalité pour laquelle elles sont traitées doivent être collectées et conservées

## SEO
114.	Qu’est-ce que le SEO ? 
Le SEO (Search Engine Optimization) est l'ensemble des techniques visant à améliorer le positionnement d'un site web dans les résultats des moteurs de recherche.
115.	Quel est l’objectif principal du SEO ? 
L'objectif principal du SEO est d'augmenter la visibilité et le trafic d'un site web en le positionnant mieux dans les résultats de recherche.
116. Existe-t-il plusieurs types de référencement ? Lesquels ?
Oui, il existe plusieurs types de référencement : le référencement naturel (SEO), le référencement payant (SEA), et le référencement local.
117. Qu’est-ce que la densité de mots-clés en SEO ?
La densité de mots-clés en SEO est le pourcentage de fois qu'un mot-clé apparaît par rapport au nombre total de mots dans un contenu.
118. Qu’est-ce qu’une balise « alt » ?
Une balise "alt" est une description textuelle d'une image utilisée pour améliorer l'accessibilité et aider les moteurs de recherche à comprendre le contenu de l'image.
119. Qu’est-ce que la balise « meta description » ?
La balise "meta description" est un court texte descriptif d'une page web affiché dans les résultats de recherche pour inciter les utilisateurs à cliquer.
120. Qu’est-ce que le « nofollow » en SEO ?
Le "nofollow" est un attribut qui indique aux moteurs de recherche de ne pas suivre un lien spécifique ou de ne pas transmettre d'autorité à la page liée.
121. Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
Un contenu de qualité est essentiel pour le référencement car il aide à retenir les utilisateurs, à améliorer l'engagement, et à montrer aux moteurs de recherche la pertinence de votre site.
122. Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
L'utilisation structurée des balises de titre (h1, h2, h3, etc.) permet d'organiser le contenu et d'améliorer l'accessibilité et le SEO d'une page web.
123. Quelle est la recommandation pour les URL d'un site web bien référencé ?
Les URL d'un site bien référencé doivent être courtes, lisibles, et contenir des mots-clés pertinents.
124. Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
Le maillage interne consiste à lier différentes pages d'un même site pour faciliter la navigation et aider les moteurs de recherche à explorer et indexer le site.
125. Qu'est-ce que l'optimisation des images pour le référencement ?
L'optimisation des images pour le référencement inclut la réduction de leur taille, l'utilisation de balises "alt", et des formats adaptés pour améliorer la vitesse du site et le SEO.
126. Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?
126. Un plan de site (sitemap) est un fichier qui liste toutes les pages d'un site pour faciliter leur indexation par les moteurs de recherche.

## GESTION DE PROJET - DevOps
127. Qu’est-ce que la gestion de projet ?
La gestion de projet consiste à planifier, organiser et superviser un projet pour atteindre des objectifs définis.
128. Qu’est-ce qu’une méthode Agile de gestion de projet ? 
Une méthode Agile est une approche flexible de gestion de projet qui permet des ajustements rapides en cours de développement.
129. Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
La méthode MoSCoW classe les priorités d'un projet en Must have (essentiel), Should have (important), Could have (souhaitable), et Won't have (non prioritaire), pour mieux gérer les attentes et les ressources.
130. A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
La méthodologie MVP (Minimum Viable Product) permet de créer une version simplifiée d'un produit pour tester rapidement sa viabilité, en mettant l'accent sur les fonctionnalités essentielles.
131. Qu’est-ce que la planification itérative ?
La planification itérative divise un projet en cycles courts pour permettre des améliorations continues en fonction des retours.
132. Citer 3 méthodes Agiles dans le cadre d’un projet informatique
Trois méthodes Agiles en informatique sont Scrum, Kanban, et Extreme Programming (XP).
133. Qu’est-ce qu’une réunion de revue de projet ?
Une réunion de revue de projet évalue les progrès réalisés, discute des problèmes rencontrés et ajuste le plan si nécessaire.
134. Qu’est-ce qu’un livrable dans un projet ? 
Un livrable est un produit ou un résultat final d'un projet remis aux parties prenantes.
135. Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
Les trois piliers de Scrum sont la transparence (rendre l'information visible), l'inspection (examiner le travail régulièrement), et l'adaptation (ajuster si nécessaire).
136. Qu’est-ce que le DevOps et quel est son objectif principal ?
Le DevOps est une pratique qui unifie le développement et les opérations pour accélérer les livraisons et améliorer la qualité logicielle.
137. Qu’est-ce que l’intégration continue ? 
L'intégration continue est une pratique consistant à tester et valider automatiquement le code à chaque modification pour détecter rapidement les erreurs.
138. Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
Docker est une plateforme de conteneurisation qui permet d'isoler les applications et leurs dépendances, facilitant le déploiement et l'intégration dans DevOps.
139. Qu’est-ce qu’un test unitaire ? 
Un test unitaire vérifie qu'une petite partie de code fonctionne correctement indépendamment des autres.
140. Quelle est l'unité de code testée lors d'un test unitaire ?
L'unité de code testée lors d'un test unitaire est généralement une fonction ou une méthode.
141. Quelles sont les caractéristiques d'un bon test unitaire ?
Un bon test unitaire est rapide, indépendant, répétable, et couvre différents cas possibles.
142. Qu'est-ce qu'une assertion dans un test unitaire ?
Une assertion dans un test unitaire vérifie si le résultat d'un test correspond à l'attendu.

 
## English

1)	What does JavaScript enable you to do on a website ?
a.	Add interactive behavior and dynamic content ==> right answer
b.	Define the layout and design of web pages
c.	Handle server-side operations

2)	Which programming language is primarily used for server-side web development ?
a.	PHP ==> right answer
b.	JavaScript
c.	HTML

3)	What is the purpose of a web browser ?
a.	To render and display web pages ==> right answer
b.	To execute serve-side code
c.	To manage databases

4)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server ==> right answer
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable

5)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development ==> right answer
b.	To optimize website loading speed
c.	To handle server-side scripting

6)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications ==> right answer
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites

7)	What does NoSQL stand for ?
a.	Not Only SQL ==> right answer
b.	Non-Structured Query Language 
c.	New Object-Oriented Language

8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models ==> right answer
