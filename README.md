Mémoire Technique - Projet Réseau
1.	Introduction
________________________________________
Présentation du projet et de son contexte
Ce projet répond à un appel d'offres fictif dans lequel il est demandé de concevoir un réseau informatique pour un bâtiment d’entreprise. L’objectif est de fournir une solution qui inclut l’intégration de matériel réseau, la gestion des VLANs, et la mise en place de plusieurs services essentiels tels que la vidéosurveillance, la gestion de la sécurité incendie, et un accès réseau Wi-Fi pour les invités, tout en assurant une performance optimale à travers le bâtiment.
La solution proposée inclura des équipements de la société Meraki, une filiale de Cisco spécialisée dans les solutions de réseau sans fil, les systèmes de sécurité et la gestion des infrastructures réseau en cloud.


Objectif de la réponse à l'appel d'offres fictif
L'objectif est de répondre à cet appel d’offres en proposant une architecture réseau adaptée aux besoins de l’entreprise, avec des solutions sécurisées et performantes. Le projet vise à fournir une infrastructure réseau fiable, avec une prise en compte des contraintes de sécurité, de performance, et d’évolutivité. Nous proposerons une solution adaptée aux différents usages du bâtiment, en tenant compte de l'optimisation de l’utilisation des équipements.

Choix de la configuration Mesh pour l'architecture réseau
Dans le cadre du projet de conception réseau pour le bâtiment, il a été décidé d'opter pour une architecture Mesh afin d'assurer une connectivité fiable, redondante et évolutive. Cette approche est particulièrement adaptée aux environnements professionnels exigeants où la disponibilité du réseau et la résilience sont des priorités.

Qu'est-ce qu'une configuration Mesh ?
Une configuration Mesh implique l’interconnexion de plusieurs équipements réseau de manière que chaque appareil soit connecté à plusieurs autres, formant ainsi un réseau maillé. Cette topologie permet une circulation fluide des données, où les informations peuvent prendre plusieurs chemins pour atteindre leur destination, offrant ainsi une résilience accrue en cas de défaillance d'un lien ou d'un périphérique.
________________________________________
Raisons du choix du Mesh
1.	
Redondance et fiabilité : Le Mesh assure une tolérance aux pannes en permettant aux données de trouver un autre chemin en cas de défaillance d’un switch, garantissant une continuité de service sans impact majeur.
2.	
Optimisation de la bande passante : Le Mesh permet une gestion dynamique de la bande passante, évitant les goulets d'étranglement et réduisant la latence, ce qui optimise la performance du réseau avec de nombreux équipements connectés.
3.	
Flexibilité et évolutivité : L’architecture Mesh permet d’ajouter facilement de nouveaux équipements sans perturber le réseau, offrant ainsi une grande flexibilité et scalabilité pour répondre aux besoins futurs.
4.	
Haute disponibilité : Le Mesh assure une disponibilité maximale en auto-réparant le réseau, réduisant les risques de coupures ou de dégradation des performances.

Les switches Meraki MS425-32-HW, configurés en Mesh, assurent une connectivité redondante et une gestion optimisée du trafic. Grâce à leurs 32 ports 10 Gigabit Ethernet, ces switches offrent une performance ultra-rapide et une capacité de gestion élevée pour les réseaux d'entreprise. Leur capacité à fournir PoE+ permet d'alimenter des équipements tels que des points d'accès, des caméras de surveillance et d'autres périphériques compatibles, tout en garantissant une infrastructure évolutive et robuste pour répondre aux besoins futurs de l'entreprise.
________________________________________
2. Estimation des Coûts
Présentation du DPGF
Le DPGF contient la liste détaillée des équipements nécessaires, incluant les switches, bornes Wi-Fi, caméras, câblage RJ-45, etc. Les coûts estimés pour chaque équipement sont les suivants :

1.	MS125-48LP-HW : Switch de distribution PoE conçu pour alimenter les équipements réseau tels que les points d'accès et caméras.
o	Quantité : 27
o	Prix public total : 56 862,75 €
o	Prix remisé total : 98 697,49€


Le Meraki MS425-32-HW est un switch Layer 3 (L3) hautes performances conçu pour les réseaux d'entreprise nécessitant un débit élevé et une connectivité fiable. Il est idéal pour une utilisation comme switch de distribution ou switch cœur de réseau dans des environnements complexes. Ce modèle offre 32 ports SFP+ (10 Gbps) pour des connexions à haut débit, ce qui le rend parfait pour gérer des volumes importants de trafic réseau.
Quantité : 2
15 179,00 €
50% 7 589,50 €


2.	CW9164I-MR : Point d'accès Wi-Fi haut débit offrant une couverture optimale dans l’ensemble du bâtiment.
o	Quantité : 74
o	Prix public total : 81 409,99 €
o	Prix remisé total : 109 903,49 €

3.	LIC-MS250-48LP-5YR : Licence de 5 ans pour les switches MS250, garantissant un accès continu aux fonctionnalités cloud et aux mises à jour.
o	Quantité : 2
o	Prix public total : 1 333,00 €
o	Prix remisé total : 3 599,10 €


4.	LIC-MS125-48LP-5Y : Licence de 5 ans pour les switches MS125, incluant des mises à jour et la gestion centralisée via le cloud.
o	Quantité : 27
o	Prix public total : 187,5€
o	Prix remisé total : 20 503€

5.	LIC-ENT-5YR : Licence Wi-Fi de 5 ans pour gérer les points d'accès CW9164I-MR avec des fonctionnalités avancées.
o	Quantité : 74
o	Prix public total : 375,00 €
o	Prix remisé total : 37 462,50 €
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
Analyse Bâtiment –
En vu de la taille du bâtiment et de tous les étages, il a fallu calculer le nombre de Watts et les équipements/Port pour chaque étages afin de répondre a la demande sans abus pour la répartition des switch , routeurs …

Voici le résultat final de nos calculs,
(peut contenir des erreurs de calculs minimes )

Watts par étage :

SS5 = 31
SS4 = 61
SS3 = 78
SS2 = 105
SS1 = 280
RDC = 723
1 = 167
2 = 219
3 = 225
4 = 226
5 = 202
6 = 172
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

PORT/EQUIPEMENT par étage:

Exemples de Listes des équipements :
1.	Détecteur auto d’incendie
2.	Déclencheur Manuel Incendie
3.	Diffuseur Sonore
4.	Diffuseur Sonore avec message
5.	Flash lumineux
6.	Détecteur Flamme
7.	Détecteur Emetteur Récepteur
8.	Lecteur Badge 
9.	Détecteur bris de vitre
10.	Détecteur d’intrusion

SS5 = 15
SS4 = 21
SS3 = 29
SS2 = 34
SS1 = 78
RDC = 130
1 = 52
2 = 73
3 = 76
4 = 75
5 = 66
6 = 47
TOTAL EQUIPEMENT : 696
________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________



 
Justification des Choix des Équipements et Licences
MS125-48LP-HW : Switch de distribution PoE
Rôle : Ces switches sont utilisés pour connecter les différents équipements réseau, tels que les points d'accès et les caméras de surveillance. Ils assurent une alimentation via PoE (Power over Ethernet) pour simplifier le déploiement et réduire les coûts d'infrastructure électrique.
Avantages :
Gestion efficace du réseau local pour les équipements connectés.
Alimentation PoE pour minimiser l'utilisation de câbles supplémentaires.
Flexibilité pour une expansion future du réseau grâce à ses 48 ports.
Prix remisé total : Prix remisé total : 98 697,49€


MS425-32-HW : Switch cœur haut de gamme
Rôle : Ces switches jouent le rôle de backbone du réseau, reliant les switches de distribution et assurant la gestion des flux de données au sein de l'infrastructure. Le MS425-32-HW offre des performances accrues avec 32 ports SFP+ (10 Gbps) pour des connexions ultra-rapides et une capacité de traitement de données élevée.
Avantages :
Fonctionnalités avancées pour le routage et la gestion centralisée via Meraki Cloud.
Haute disponibilité grâce à la possibilité de redondance avec des alimentations et des ventilateurs remplaçables à chaud.
Optimisation des performances réseau grâce à une connectivité 10 Gbps et une gestion fine du trafic.
Idéal pour un backbone réseau fiable et performant.
Prix remisé total : 7 589,50 € (1 unité).
CW9164I-MR : Point d'accès Wi-Fi haut débit

Rôle : Ils assurent une couverture Wi-Fi optimale dans l’ensemble du bâtiment, permettant une connectivité sans fil stable et rapide.
Avantages :
Support des normes Wi-Fi 6 pour des performances élevées et une densité utilisateur accrue.
Facilité de gestion via le cloud pour une surveillance et un dépannage centralisé.
Large couverture, adaptée aux besoins d'un bâtiment d’entreprise.
1.	LIC-MS125-48LP-5Y : Licence pour switches MS125

o	Rôle : Fournit les mêmes avantages que la licence MS250 mais adaptée aux switches de distribution MS125.
o	Avantages :
	Centralisation de la gestion des switches via le cloud.
	Garantie d’un service de qualité sur le long terme.
o	Prix remisé total : Prix remisé total : 20 503 (27 unités).
o	Justification du coût : Essentiel pour maintenir les switches de distribution fonctionnels et performants sur 5 ans.
2.	LIC-ENT-5YR : Licence Wi-Fi pour CW9164I-MR

o	Rôle : Cette licence permet la gestion des points d’accès via le cloud et offre des fonctionnalités avancées telles que l'analyse réseau et la sécurité renforcée.
o	Avantages :
	Surveillance en temps réel de l'état des points d’accès.
	Mise en œuvre de politiques de sécurité adaptées au réseau Wi-Fi.
	Support pour l’optimisation de la bande passante en fonction des usages.
o	Justification du coût : Requis pour tirer pleinement parti des capacités des points d'accès et garantir une connectivité stable sur 5 ans.
________________________________________

3. Timeline du Projet
Dates clés à respecter :
•	Présentation du projet : 29 octobre.
•	Session de Questions & Réponses (Q&R) : Jusqu'au 19 novembre.
•	Date limite pour les demandes de prix des équipements : 26 novembre à 23h59.
•	Remise des documents : 1er décembre à 23h59.
•	Soutenance finale : 10 décembre.


________________________________________

4.Objectif et Livrables

Détails des livrables attendus :
•	Document explicatif du projet : Un document détaillant la solution réseau proposée, comprenant des explications sur les choix techniques, les besoins du client, et la conception du réseau.
•	DPGF (Détail Quantitatif Estimatif) : Une liste exhaustive des équipements nécessaires avec des estimations de coûts détaillées.
•	Schémas logique et physique du réseau : Représentations graphiques du réseau dans son architecture logique et physique, mettant en évidence les VLANs, la structure du câblage, et les équipements.
•	Maquette fonctionnelle sur Packet Tracer : Un modèle simulé du réseau dans Packet Tracer, permettant de tester la configuration et de valider la conception avant le déploiement réel.

________________________________________

5. Analyse des Besoins
Identification des besoins exprimés dans le CCTP
Le CCTP (Cahier des Clauses Techniques Particulières) décrit les principaux besoins de l'entreprise, et permet ainsi de cerner les attentes pour la mise en place du réseau. Voici les besoins clés identifiés :
•	Segmenter le réseau en VLANs distincts : Il est nécessaire de séparer les différents types de trafic réseau afin d’assurer la sécurité et la gestion de la bande passante. Les VLANs permettront de définir des zones spécifiques du réseau (par exemple : VLAN pour les employés, VLAN pour la sécurité, VLAN pour les invités).
•	Sécurisation de l’accès au réseau : L'entreprise doit mettre en place une solution de sécurité robuste pour protéger l'accès au réseau. Cela inclut la gestion des utilisateurs, le contrôle d'accès, et la protection des informations sensibles via un réseau sécurisé, notamment avec des pares-feux, des dispositifs de surveillance, et un système de gestion centralisé des accès.
•	Wi-Fi pour invités et employés : Une couverture Wi-Fi performante et sécurisée est essentielle pour l’entreprise. Le CCTP exige que l’infrastructure réseau soit capable de supporter un grand nombre d’utilisateurs simultanés dans le bâtiment, tout en garantissant la sécurité des connexions invitées, sans compromettre l’intégrité du réseau principal de l’entreprise.
•	Optimisation de l'infrastructure pour l'évolutivité : L'entreprise souhaite pouvoir faire évoluer son réseau facilement dans le futur. Il est donc crucial que l'architecture réseau proposée permette l'ajout de nouveaux équipements (points d'accès Wi-Fi supplémentaires, caméras, etc.) sans impacter les performances du réseau.



________________________________________

Schéma logique
Le réseau sera conçu autour d'un Switch L3 Meraki central, qui interconnecte les différents VLANs et assure la gestion du routage entre eux. Le réseau sera segmenté en plusieurs VLANs distincts pour garantir la sécurité et la performance. Chaque étage du bâtiment sera raccordé à un Switch L2 Meraki, qui sera relié au Switch L3 central.
Les VLANs seront organisés comme suit :
•	VLAN Contrôle d'accès : pour la gestion des dispositifs de sécurité et d'accès.
•	VLAN Vidéosurveillance : pour la gestion des flux vidéo.
•	VLAN Administration/Supervision : pour les équipes de gestion du réseau.
•	VLAN RH, VLAN Dev, VLAN Direction, etc. : pour chaque département de l'entreprise.

________________________________________

Schéma physique
Le placement des équipements dans les différents étages du bâtiment sera stratégique, avec des Switches L2 positionnés à chaque étage pour une couverture réseau optimale. Les bornes Wi-Fi seront installées dans les zones de passage et de travail pour maximiser la couverture. Les caméras de surveillance seront réparties en fonction des besoins de sécurité.
Voici 3 exemples dans notre cas
Placement et Organisation dans votre Schéma Physique
Switch Cœur (MS250-48-HW)
•	Connexion au routeur principal :
o	Les deux switches cœur (MS250-48-HW) sont connectés au routeur principal situé dans la salle réseau du rez-de-chaussée. Cette connexion se fait via des liens en fibre optique pour garantir une bande passante élevée et une faible latence.
o	Les switches cœur gèrent l’agrégation des flux réseau provenant de tous les étages et assurent une redondance en cas de défaillance de l’un d’eux.
________________________________________

6ᵉ Étage
•	Nombre de switches L2 : 2 switches L2 (MS125-48LP-HW).
•	Utilisation et placement :
o	Ces switches distribuent le réseau aux équipements du 6ᵉ étage, notamment les points d'accès Wi-Fi, les caméras de surveillance, et les postes de travail.
o	Positionnés dans une armoire de câblage centrale, ils sont interconnectés avec les switches cœur via des uplinks en fibre optique.
________________________________________
SSL3 (Sous-Sol 3)
•	Nombre de switches L2 : 1 switch L2 (MS125-48LP-HW).
•	Utilisation et placement :
o	Le switch unique au SSL3 gère les équipements spécifiques à cet étage (par exemple, zones de stockage, équipements de sécurité, ou salles techniques).
o	Ce switch est connecté aux switches cœur via un lien montant (uplink) en fibre optique.
________________________________________
Rez-de-chaussée
•	Nombre de switches L2 : 3 switches L2 (MS125-48LP-HW).
•	Utilisation et placement :
o	Les switches du rez-de-chaussée gèrent un plus grand nombre d’équipements, car cet étage abrite généralement des zones à forte densité d’équipements, comme le hall d’accueil, les salles de réunion, les espaces de coworking, et les postes de sécurité.
o	Répartis dans deux armoires de câblage, les switches sont connectés aux points d'accès Wi-Fi, caméras, et postes de travail du rez-de-chaussée.


Conclusion : 
Pour la répartition dans tout le bâtiment nous avons opté de les répartir de cette manière-là :


SWITCH LAYER 2 par etage :
SS5 = 1
SS4 = 1
SS3 = 1
SS2 = 2
SS1 = 3
RDC = 4
1 = 2
2 = 3
3 = 3
4 = 3
5 = 2
6 = 2
________________________________________________________________________________________________________________________________________________________________
8. Conclusion :


En conclusion, la solution réseau proposée repose sur une architecture claire et bien définie, adaptée aux besoins spécifiques de l'entreprise. Grâce aux équipements Meraki,
nous garantissons une gestion centralisée et une grande facilité d’administration, tout en répondant à des exigences de sécurité strictes. Voici les principaux points qui soulignent l’importance de cette solution :
Sécurité et performance : La segmentation du réseau par VLANs et l’intégration des dispositifs de sécurité (caméras, Wi-Fi sécurisé) assurent non seulement la protection des données sensibles, mais aussi la gestion optimale du trafic,
 afin de garantir des performances réseau stables et rapides.
Évolutivité et flexibilité : L'architecture proposée permet à l'entreprise de se développer en toute sérénité, avec des équipements évolutifs et faciles à intégrer dans le réseau. Que ce soit pour ajouter des bornes Wi-Fi ou des caméras supplémentaires,
 la solution proposée peut répondre à de futures demandes de manière fluide et sans interruption de service.
Simplicité d’administration : L’utilisation de solutions Meraki pour la gestion centralisée via le cloud facilite l’administration du réseau, réduisant ainsi les coûts et le temps liés à la gestion locale des équipements.
 Cela permet aux équipes IT de se concentrer sur des tâches à plus forte valeur ajoutée, tout en maintenant une surveillance continue du réseau.
Adaptation aux besoins spécifiques du client : Cette proposition prend en compte non seulement les besoins de connectivité et de sécurité, mais aussi la gestion de la vidéosurveillance et des dispositifs de sécurité incendie.
 Le réseau est conçu pour répondre de manière exhaustive aux besoins fonctionnels et techniques du client, tout en offrant un niveau de sécurité élevé et une connectivité sans faille.
En somme, la solution proposée est une réponse complète, sécurisée et évolutive qui permettra à l’entreprise de fonctionner de manière optimale, tout en s’adaptant facilement aux évolutions futures.

