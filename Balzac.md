
---
title: Cahier journal d'une découverte de la lexicométrie autour de la _Comédie Humaine_ de Balzac
date: 19 avril 2022
author : Hanna Brisseau, Samy Delobel, Gabriel Christmann
avertissement : Ce texte a été écrit rapidement en avril 2022, nous vous prions d'excuser les erreurs orthographiques qui demeurent et qui doivent faire l'objet d'une correction. 
---




## Introduction

### Une œuvre littéraire

La _Comédie Humaine_ est un regroupement de textes produits par Honoré de Balzac et publié pour la première fois en 1829. C'est un projet d'écriture née très tôt dans l'esprit du romancier.
En effet, c'est une fois les premiers romans écrits qu'il pense ce grand ensemble de la "Comédie Humaine" et les trois subdivisions thématiques qui le compose. 
Balzac veut analyser en détail les rouages de sa société et en donner un tableau général qu'il pense tout au long de sa vie, corrigeant ses œuvres et pensant régulièrement de nouveaux ordres de lecture[^n3]. L'auteur se veut être un "historien des mœurs" comme il le souligne dans l'avant-propos de son œuvre, en conduisant une analyse détaillée de sa société grâce à un support et un style novateurs pour son époque : _le roman_. Lorsque Balzac commence à écrire, le roman. Lorsque Balzac commence à écrire, le roman n'est pas encore un genre littéraire majeur mais il permet de fournir des ouvrages longs et autorisant un souci du détail ainsi que de possibilités descriptives qui vaudront à Balzac le qualificatif de "réaliste"[^n1]. Cette question du réalisme balzacien est encore débattue, pour Albert Béguin par exemple il ne s'agissait chez Balzac "nullement de peindre la réalité courante, mais au contraire d'en pousser tous les détails à l'hyperbole.".
Au-delà du débat littéraire, l'importance des détails, le souci d'analyse des sentiments et des relations sociales confèrent à cette œuvre un intérêt historique.


### L'auteur et ses choix politiques

Ce début de XIXe siècle connaît de nombreux changement sociaux, techniques et politiques. Balzac traverse au cours de sa vie, près de quatre régimes différents ainsi que deux révolutions. Le puissant empire Napoléonien marque son enfance, son entrée dans l'âge adulte et sa vie d'homme évolue de la monarchie Orléane à l'autoritaire IIe République. Son œuvre imprégné de thèmes concrets ou de fond dans plusieurs de ses romans. Il assiste à l'émergence du capitalisme, de l'essor de l'industrialisation et à la structuration progressive de la société (notamment parisienne) autour de cela.
L'œuvre offre alors un regard sur cette société, son passé -lieux communs ou opinions plus personnelles de l'auteur- marqué par le souvenir de la Révolution de 1789 encore vivace et par un souvenir de la monarchie absolue faisant son retour sous Louis XVIII et Charles X.
Elle permet d'avoir une vision, certes subjective, mais néanmoins riche, d'un homme sur de son époque, politiquement incertain et poursuivi par ses créanciers, sur ce début de XIXe siècle. S'il n'est pas un observateur transparent, nous essaierons d'entrevoir comment la société de ce premier XIXe siècle saille au travers de ses textes. 




###   Nos partis pris méthodologiques


Pour conduire cette expérience d'apprentissage nous avons décidé d'utiliser une oeuvre litteraire afin d'essayer de la lire en historien, c'est-à-dire, de dégager des sens historiques derrière une écriture romanesque. Il fallait que cette oeuvre soit suffisement vaste et pour tout dire épaisse afin de décourager une  lecture linéaire et exhaustive pendant ces 10 semaines. Nous aurions pu être tenté de lire une un roman, ou un échange de correspondance, la _Comédie Humaine_ était trop grande pour une approche classique. Dans ce cadre le recours à une méthode plus quantitative nous permettait d'embrasser l'oeuvre dans sa totalité, ce qui ne signifie pas que nous avons renoncé à la lire, au contraire notre lecture n'a jamais cessée. Elle était plus réticulaire que linéaire. A charge, à présent, de réouvrir les romans. 



 
Nous avons décidé de mener notre expérience sur les 10 semaines de notre second semestre 2022 à partir du logiciel libre IRaMuTeQ[^n2], d'une écriture en Markdown exportée vers du html et quelques scipts en langage python. 
L'utilisation d'Iramuteq semblait légitime pour plusieurs raisons : 

1. un meilleur contrôle sur les algorithmes que nous utilisons par ce qu'il est _open source_

2. une facilité de ré-expérimentation (gratuité, multi-plateforme) et c'est pourquoi, nous tâcherons à présent d’écrire systématiquement, à côté de nos interprétations, les résultats et processus qui nous ont permis de les produire.


## La cohérence du corpus
 
 
Le corpus utilisé est ici composé de l'intégralité des textes de La Comédie Humaine. Cette œuvre est publiée entre 1829 et 1855 (l’auteur mourant en 1850, certains romans à titre posthume). Destiné à être lu dans un ordre précis pour donner un tableau de la société telle que la voit Balzac, l’ensemble contient 90 ouvrages et est divisé en 3 grandes catégories :

1. Les études de mœurs (68 textes, 3 454 012 occ. ,  33163 formes, 12353 hapax)

2. Les études philosophiques

3. Les études analytiques
 

Ces trois études composée commencent avec le roman _Les Chouans_ (1829) et se termine avec le roman édité à titre posthume par la veuve de l'auteur, _Les Paysans_ (1855).

Ce corpus répond aux critères mis en évidence par Antoine Prost. Il est homogène car il est la production d'un seul auteur, les variations thématiques qu'il pose dans chacun de ses romans offrent un outil pour mener une analyse contrastive. Enfin, les temps d'écriture et de publication lui confèrent une diachronicité qui permet d'observer des transformations dans le vocabulaire dont il fait usage.
 
 



 
 
### Tester la partition temporelle  

C'est un tableau permettant d'observer la distribution des occurrences, 
des formes et d'hapax en fonction d'une partition determinée. 
 
| Partie|  Occurrences|Formes|Hapax|
| :------------- |-------------:|-------------:|-------------:|
|1855|    157125|    16404|    8110|
|1848|    65687|    9202|    4979|
|1847|    313362|    23191|    11022|
|1846|    18586|    4245|    2733|
|1844|    143336|    15116|    7705|
|1843|    288876|    22301|    10387|
|1842|    480135|    26939|    11526|
|1841|    86324|    11032|    5674|
|1840|    85191|    11529|    6159|
|1839|    241409|    18430|    6979|
|1838    |158007    |12704|    2574|
|1837    |145966    |16450|    8419|
|1836|    135371|    15782|    8061|
|1835|    148995|    14886|    7569|
|1834|    94304|    12346|    6780|
|1833|    183754|    17519|    8498|
|1832|    48199|    8002|    4466|
|1831|    10285|    2820|    1899|
|1830|    117430|    13223|    6513|
|1829|    104923|    11553|    5643|
| Total |    3027265|    62071|    21377|
 
le premier tableau est une comparaison par année, 
Cette partition des textes fait apparaitre des
oscillations très fortes entre les années ne permettant pas d'observers une evolution sur le temps long.
Le temps n'etait pas une structure choisi par l'auteur, on ne peut l'utiliser pour etudier la Comédie Humaine. [^n4].
 
 
### Une distribution thématique
 
| Thèmes  | Occurrences |Formes|Hapax |
| :------------- |-------------:|-------------:|-------------:|
 | scene de la vie privée|    868283|    35742|    14113|
 | scene de la vie politique    |198581|    17277|    8093|
 | scene de la vie parisienne|    860203|    37373|    14739|
 | scene de la vie militaire|    109699|    11931|    5786|
 | scene de la vie de province|    612192|    31644|    13347|
 | scene de la vie de campagne|    378307|    24873|    9705|
 
La comparaison par thématiques,refléte la structure que Balzac 
a donnée à son oeuvre.
Cette comparaison montre la forte importance accordé par l'auteur aux
catégories sur «  la scène de la vie privée » et « scène de la vie
parisiennes ». En effet, ces catégories couvrent 57% de l'ensemble des
occurrences du corpus. C'est dans la "scène de la vie politique" et
celle de "la vie militaire" que le nombre de forme est relativement plus
élevée (respectivement 9 et 11%), dans l'ensemble de ces parties les
hapax oscillent entre 39 et 42%.l
 
 
Alors que dans les thèmes « scène de la vie politique » et «  scène de
la vie militaire » l’occurrence , donc la répétition des mots est
inférieur a 200000 avec notamment la vie militaire qui comporte a peine
plus de 100000 occurrences , ce qui montre peut être que ces domaines
ont leur mots propres.
C’est d’autant plus marquant car l’hapax c’est a dire la seul
occurrence est plutôt faible pour les deux même thèmes déjà évoquer,
ainsi « scène de la vie politique » en comporte que 5786 et « scène de
la vie militaire » en comporte que 8093 tandis que « scène de la vie
privé » en comporte 14113 et « scène de la vie parisienne » 14739 ce qui
montre que contrairement aux thème politique et militaire, il y a plus
de mots unique dans les texte qui concerne ces thèmes qui donc montre soit que
ce thèmes contrairement aux thèmes militaire ou vie politique ne comporte pas de vocabulaire propre
ou que ce thémes sont plus riche par l'interet porter a l'auteur a ces thèmes. 


 
 
Pour les formes la comparaison reste la même , une supériorité dans les
thèmes de la vie prive et paris contrairement aux thèmes militaire et
politique.
Pour les deux derniers thèmes, « scène de la vie de province » et «
scène de la vie de campagne », l'oeuvre est tournée vers Paris et  les
textes s’intéressant plus à la provinces à  la campagne sont les moins
nombreux. Peut-être, y a t-il une différence de traitement dans son
étude des caractères ? 

 
 
## Repérer les principales thématiques dans la Comédie Humaine



### L'analyse factorielle des correspondances


Les méthodes d`analyse factorielle sont des outils qui mettent en évidence des relations entre des variables.
Nous utiliserons ici l'analyse factorielles des correspondances sur un tableau lexical. Elle permet de structurer l'ensemble des « formes » en fonction de leur
répartition dans les unités textuelles[^n8]. 
Il devient possible de hiérarchiser la contribution des formes à chaque axe dans le tableau. Le graphique propose de croiser deux facteurs et positionne les formes suivant les coordonnées ainsi obtenues. 

La lecture des axes se fait en observant les principales oppositions entre les lignes et les colonnes. 

Afin d'être au plus proche du projet balzacien nous avons croisé les formes et les "scènes de vie", l'une des structure de la comédie humaine.

Le croisement des axes 1 et 2, plus de 57% de l'inertie faisait apparaitre une forme en "idéal type"[^n10], la question se posait de mettre en complémentaire tous les noms 





### La méthode Reinert
Il s'agit d'une analyse de contenu dont l'objectif est d'obtenir un classement des « phrases » du corpus étudié en fonction de
la ressemblance ou de la dissemblance des formes dans ces « phrases » et d'ordonner les
textes en cernant les homologies et les oppositions. L'idée est
présentée de cette façon par Max Reinert son créateur : 

> "rappelons que notre méthodologie consiste à découper un texte en petits morceaux relativement arbitraires et à  étudier la  distribution des mots pleins dans ces unités afin de les rassembler  dans des classes en fonction de leur ressemblance et dissemblance." [^n5]



Mise au point en 1983[^n6], cette 
méthode est itérative : Après avoir composé un tableau
Présence/absence, les unités textuelles sont regroupées en une seule
classe ; à chaque étape, on fait ressortir les deux classes les plus différentes entre elles, en
termes de vocabulaire.
Le critère de décomposition s'appuie sur une mesure du Khi2.

Cette méthode, à la différence de l'AFC, permet d'observer des proximités entre des vocables et de dégager ainsi des thématiques 

#### Les résultats que nous obtenons 

Les deux analyses que nous proposons s'appuie sur deux réglages
différents de la méthode implémentée dans le logiciel Iramuteq[^n7].


![Classification1](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/ClassifReinert/dendrogramme.png?raw=true)
![Classification2](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/ClassifReinert/dendrogramme_1.png?raw=true)


Le logiciel produit au moins trois types de résultats que nous allons exploiter pour naviguer dans les classes obtenus :

1. Des graphiques présentant les principaux mots associés aux classes organisés sous forme de dendogrammes. L'attachement des formes à chaque classe est hiérarchisé par une valeur du khi2, ce qui se traduit sur le graphique par une un grossissement de la forme sur le graphique. Par exemple dans la troisième classe la forme "aller" est déformée pour témoigner de sa plus forte contribution à cette classe (voir graphique2). 

2. des fichiers présentant l'ensemble du vocabulaire dans chaque classe 

3. une organisation en réseau de chaque classe

Évidemment, l'utilisation de ces résultats doit être accompagné d'un retour aux concordances, afin d'éclaircir le sens que l'on peut donner aux formes que l'on repère dans la classification.

Sur les 112 423 segments isolés par Iramuteq 94 808 ont été classés ici, soit 84,3%. 
La classification obtenue nous permet d'observer 7 classes réparties en 3 grands ensembles thématiques bien identifiables sur le dendogramme (cf, graphique 7 classes) : 

1. un ensemble comprenant les classes 2 (14.1%) et 6 (14.7%) représentant 28,8% des formes. L’attachement aux détails si caractéristique du travail de Balzac et contribuant à un certain ‘réalisme’, émerge à travers la description des personnes avec la classe 2 et celle des environnements et objets dans la classe 6. Chacune de ces classes couvre des ensembles lexicaux très large, ainsi la classe 2 rassemble des termes liés au corps, à la vue mais aussi aux sons et à la voix, elle semble recouvrir l’ensemble des sens. La classe 6 aborde différents environnements de la personne parfois liés à l’intérieurs de logements ou bien aux mondes urbains ou ruraux, mais elle touche aussi aux vêtements par exemple.  

2. un second composé des classes 3 (15.8%), 5 (11.1%) et 7 (12%) représentant 48.9% des formes. La classe 3 regroupe plutôt des formes liées aux interactions et à la sociabilité, on y retrouve les termes descriptifs de situations dans lesquels les personnages sont amenés à interagir et dans lesquels s’insèrent les dialogues, les éléments de narration, mais aussi la description des statuts des relations interpersonnelles et leur temporalité. La classe 5 est ici celle de l’argent, de la fortune ou de l’infortune, qui peut prendre les formes de la rente, du capital ou de la créance.  La classe 7, enfin, reflète le système politique qui structure cette société de la restauration.  On y trouve toute la hiérarchie du « roi », des « pairs »  et des « princes » mais aussi des termes liés à l’ordre comme la « police », « procureur » et la « préfecture » qu’il faudra analyser plus en détail.

3. un dernier, enfin, constitué des classes 4 (14.6%) et 1 (17.7%) représentant 32.3% des formes. Les deux classes abordent une dimension plus abstraite du caractère humaine, celui de l’esprit et des sentiments. 

##### Classe 2 

La classe 2 rassemble des formes liées à la description de personnages ; un certain nombres de celle-ci envoi a des parties précises du corps comme œil ou main. Très associées a cette classe (khi2 ?) ce sont également des formes structurante sur le réseau. Ainsi Œil est la forme centrale du graphe, elle est la source d’un grand nombre de chemin lexicaux. De l’œil on va vers voir. Elle conduit aussi a la voix, au regard et à la main. Iramuteq permet de parcourrir plus aisément les relations entre les termes[^n9]. Sans doute les spécialistes de la littératures ne seront pas surpris de ces résultats mais cela oblige l'historien à tenir compte des phénomènes généraux, avant d'aller plus avant dans une recherche pointue et fouillée. 


![Graphe réseau de la classe 2](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/ClassifReinert/graph_simi_classe2.png?raw=true)

##### Classe 6


La classe 6 est celle de la description des endroits intérieurs et extérieur. C’est celle du promeneur qui regarde ce qu’il l’entoure.
Nous trouvons dans un premier temps des objets ou lieu de la maison comme « porte, fenêtre, salle, escalier, mur, cheminée, table » présent dans une majorité de roman il sont plus fréquent dans les scènes de la vie privée, vie de province ou la vie de campagne. 
Il y a ensuite quelques élément de la description extérieur comme « jardin, cheval, arbre, chemin, pierre, route » la figure du promeneur est très visible dans ce champ lexical.
Les formes « cheval, cocher, traverser, parc » nous indique le déplacement que l’on retrouve dans les vies politiques, privée et parisienne. Ici c’est d’avantage la déplacement d’un point A à un point B qui est illustré par rapport à la forme « promener » qui elle ne possède pas forcément d’objectif dans sa trajectoire. On retrouve ici le regard attentif aux détails et à la description d'un environnement.



##### Classe 4 

La classe 4 est celle des sentiments dont on retrouve la forme. Il y a un champ lexical de la famille est « femme, fille, mère, enfant, mari, mariage, époux » que l’on retrouve dans la plupart des cas dans les vies privée, parisienne et de province.
En contradiction il y a le lexique de l’amour charnel « femme, passion, plaisir, désir, amant, plaisir, créature, jalousie, tromper » plutôt dans les vies parisienne, privée et philosophique
Il y a également le lexique des sentiments à proprement parler comme « aimer, heureux, tendresse, affection, dévouement, vanité, jalousie, amitié, délicatesse »

![Graphe réseau de la classe 4](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/ClassifReinert/graph_simi_classe4.png?raw=true)



##### La classe 3 

La classe 3 composant 15,8% des formes, recouvre principalement l’interaction, la sociabilité et ce que l’on peut supposer être le monde des soirées qui en est l’un des principaux lieux de rencontres dans les romans de Balzac.
On retrouve plusieurs grandes catégories de termes :
Dans un premier temps des verbes : "Aller", "répondre", "venir", "demander", "reprendre", "écrier", "parler", "écrire".  Ils sont présents dans pratiquement tous les romans, ce sont des verbes d'action qui régissent les rapports entre les personnages ou précisent leur activité. Aller et venir donnent par ailleurs une indication de déplacement, aller/venir chez une personne ou en un lieu. [cooccurrences CSV] + concordances ?


Ensuite, viennent les termes évoquant la temporalité des actions notamment simplement les formes « matin » et « soir ».
Le soir marquant la fin de journée et les activités qui y sont associées, le moment des retrouvailles ou des rencontres, une temporalité attendue, un certain nombre de concordances marquent le fait de faire quelque chose « ce soir ». [insérer concordances]
On peut y lier le « dîner » qui recouvre à la fois le dîner privé et le dîner en groupe, mais c'est dans la majorité des cas le dîner "de" quelqu'un, ou celui "avec" quelqu'un, donc un élément de sociabilité, ressort narratif pour les discussions, on pourra consulter les coocurences de [dîner](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/coocurences_diner.csv).

A l'inverse le [matin](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/coocurences_matin.csv), est moins évoqué comme une perspective que comme un moment passé, mais il est à la fois le matin de la nouvelle journée où se sont déroulés de nouveaux événements qui marquent un tournant dans la narration, et à la fois le matin dans la nuit, "2 heures du matin"[^n11].
On retrouve également des appellations familiales avec « père », « cousin », « oncle »
Comme on peut s’y attendre c’est dans leur usage le plus classique qu’ils sont employés, pour désigner ce rapport à la famille mais également dans une moindre mesure la sociabilité que ce rapport permet « le vieil ami de mon père »[^n12]. Père a cependant cette particularité de pouvoir également être une référence à un clerc.
Quelques termes sortent du lot avec « lettre », « Baron » ou « docteur »
Lettre recouvre principalement le sens de correspondance, ce sont des lettres écrites d'une personne à une autre, prétexte au récit. Mais c'est aussi l'intérêt pour les lettres de l'alphabet qui ressortent sur le papier pour les personnages qui écrivent. Les Lettres au sens de littérature ne ressort pas outre mesure[^n13]. 
Baron, avec Baronne aussi très présent dans les concordances, c'est la petite noblesse, sa présence dans cette classe ci plutôt que dans la classe 7 peut laisser à penser que les barons ont un caractère récurrent dans les interactions sociales et celles avec les personnages principaux issus de milieux hors noblesse. Ou que l'auteur s'y intéresse davantage dans le cadre d'une intimité qui ne serait pas propre au reste de la noblesse.
Docteur pour sa part tient une place discutable, ce n'est ni plus ni moins en majorité que le médecin mais sa présence est principalement due au roman Ursule Mirouet dans lequel il a beaucoup d'occurrences.
En somme la classe en elle-même est assez hétéroclite dans les mots qu’elle recouvre, avec de nombreux qualificatifs s’appliquant à des personnages et des éléments de dialogue. Il ne semble pas qu’il y a ait proprement de cohérence dans le type de lexique ou dans un thème spécifique, on peut donc y voir peut être la variété de personnages, de caractères et de condition socio-professionnelle. Qui peut, comme dit au début et ceci appuyé par la présence des premières occurrences, correspondre à une sociabilité générale mais aussi plus particulièrement des soirées et des dîners où se côtoie toute la société.

![Graphe réseau de la classe 3](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/ClassifReinert/graph_simi_classe3.png?raw=true)


##### La classe 7 

La classe 7 avec 12% des formes est la classe exposant la structure hiérarchique et institutionnelle de la société de la Restauration. Une société d’ordre dominée par un premier terme : le « roi » (Khi2 = 4960). Evoqué directement pour sa personne, « le général a obtenu la grâce du roi », il est le plus régulièrement Louis XVIII mais aussi parfois Charles X ou encore dans une évocation du passé un des souverains plus anciens tels que Charles VII. On retrouve également ce titre pour une personne royale étrangère « le roi de Prusse ». « Le roi » est aussi celui dont on est le serviteur ou le représentant « le procureur du roi ». Il est enfin le fantasme honorifique, l’ultime position de supériorité, enfin presque : « Oui, madame, apprenez, si vous ne le savez pas, qu'un grand artiste est un roi, plus qu'un roi : d'abord il est plus heureux, il est indépendant, il vit à sa guise ; puis il règne dans le monde de la fantaisie. »    
Suivent ensuite divers titres : « duc », « prince », « reine » « marquis ». Qui évoquent une grande noblesse proche de ce pouvoir royal. Le mot « prince » (Khi2 = 1814) désigne cependant une large catégorie d’individus de la noblesse, princes de leur maison en France ou ailleurs, ou titre accordé comme le prince-prévôt « Prince de Wissembourg » (dans le Saint Empire romain germanique) [concordances]  [note] dans les Parents pauvres de La Cousine Bette + L'envers de l'histoire contemporaine. Les personnages peuvent également avoir des « allures de prince », on peut être « égoïste comme un prince ».
Parmi ce lexique des grands personnages, « empereur » (Khi2 = 1065), dénote, car bien qu’aristocratique il sort du cadre royal pour évoquer principalement Napoléon Bonaparte et pour beaucoup sa gloire militaire « il avait reçu de l’empereur Napoléon une magnifique paire de pistolets » [note] Les Parents pauvres de La Cousine Bette . On retrouve également des allusions à « l’empereur de Russie », [concordances]  ou enfin à l’époque antique avec notamment des évocations de Tibère ou de César ou des empereurs romains en général : « L’empereur n’était plus à Rome, quand la Ville éternelle tomba sous les Barbares. » [note] Le Médecin de campagne.
On retrouve un vocabulaire de « l’armée » (Khi2 = 579) avec des grades tels que « général », « maréchal », « lieutenant ». « Général » (Khi2 = 2970) ressortant davantage par rapport aux autres grâce à l’emploi sous le sens d’une généralité, notamment « la convocation des Etats Généraux » (les représentants des trois ordres de la société monarchique) ou « conseiller général de son département ». Cette polysémie entraîne une présence accrue dans le texte qui ne se retrouve pourtant pas forcément dans un rapport au pouvoir.    
Mais au-delà des nobles et des gradés, restent encore deux catégories : celle principale des représentants politique et de l’administration, ainsi que celle, plus mineure, du clergé.
Tout d’abord pour l’administration on retrouve les termes de « gouvernement », « député » « ministre ». « Gouvernement » (Khi2 = 688), étant entendu à la fois comme une entité on parle d’avoir « l’appui du gouvernement », mais aussi comme gestion avec le fait d’avoir une personne s’occupant du « gouvernement de ses affaires ». « Député » comme « ministre » sont pour leur part les titres de gouvernants. « Député » (Khi2 = 757), membre du Parlement dans la Chambre des Députés, est pour beaucoup évoqué pour les personnes que l’on « nomme », ou qui veulent « devenir », c’est un statut qui semble reconnu bien en vue voire enviable dans l’œuvre de Balzac. On retrouve de même le mot « pair » (Khi2 = 1153), évoquant les membres du Parlement membres de la Chambre des pairs créée par Louis XVIII en 1814 et perdurant toute la Restauration, « Il a été nommé pair de France à cause de sa conduite dans les émeutes ».

D’un point de vue plus administratif, on retrouve les entités « juge », « procureur », « tribunal », « police », « préfet », qui exécutent ou rendent justice. Tous ces thèmes étant souvent reliés ensemble dans des cooccurrences classiques telles que « préfecture de police ». De manière générale même, les termes de cette classe son en fait souvent interdépendants étant donné l’obligatoire référence hiérarchique qui est faite pour les décisions judiciaires : « Un ordre du grand-juge, transmis au procureur impérial près le tribunal de première instance de Troyes, ordonnait la mise en liberté sous caution des gentilshommes en attendant la décision de l’Empereur et Roi » (ici Napoléon Bonaparte).    

Enfin le clergé, se démarque avec notamment « cardinal », dans les premières formes (Khi2 = 864), mais ne se concrétise pas comme très présent dans le reste des fortes valeurs de Khi2 de la classe. On peut supposer que le « cardinal » est un personnage extrêmement intégré dans les jeux de pouvoir et dans son rapport à la politique ou la grande noblesse. Plus encore que dans son propre appareil religieux ou du moins pour ce qu’en laisse transparaître Balzac.



##### La classe 1 

La classe 1 regroupe les termes qui semblent s’articuler autour de « homme » bien que ce ne soit pas le premier terme à apparaître. 
« homme » s’il s’agit de caractériser les personnages masculins, est aussi le moyen de spécifier une qualification reconnue c’est un « homme politique », « homme d’esprit ». 
« grand » est utilisé comme qualificatif pour divers lieux un « plus grand théâtre », mais également pour qualifier une « grande renommée », un « grand artiste », la « grande bourgeoisie ». Il y a une caractérisation des choses physiques mais aussi une expression de la valeur de personnes ou du groupe. « grand » permet une mise en avant de certains personnages ou de certaines catégories.
On retrouve le « génie », qui caractérise encore plus l’homme qui se démarque mais surtout est présenté comme une qualité « cela procédait d’un génie particulier ».
On retrouve les diverses activités auxquelles l’esprit se dévoue alors, la « loi », la « science » n’étant pas forcément entendue comme objet de scientificité « l’immense progrès que font en ce moment les sciences naturelles », mais également comme activité à laquelle un personnage s’est dévolu ou pour laquelle il s’est spécialisé, « la science à laquelle il avait sacrifié le repos de sa vie ».
La « nature » est une référence à l’environnement, force créature « que la nature avait fait si ravissante », mais également l’essentialisation d’éléments « sont de nature à intéresser les esprits sérieux.
Il s’agit de la manière dont la pensée, l’esprit est représenté autour de l’homme de société.



##### La classe 5
 
la classe 5 est celle qui concerne  l'argent  :  
Ainsi on peut  voir une dominance des forme qui concerne le numéraire.
dans la sous division économie j’ai pris 15 formes , les 15 premières qui apparaissent.
Il y a plusieurs groupement d’abord tout ce qui ce rapporte aux payement monétaire, ainsi les formes  «livres» , «francs», «payer», «prix», «acheter» , «écu» ici on a l’idée de transaction quotidienne. Il y a aussi «prix» : avec une idée de variabilité des prix   : «vil», «bas» , «au-dessus»
Ensuite celui des échanges «vendre» , «revendre», «payer» qui est précéder de «vous» + de 10 fois.

Ensuite le groupement qui concerne la finance et la rente:
Il y a des formes qui sont liées  aux besoin monétaires  : «argent», «fortune» et «fonds»
liée aux système financier ,«banques» liée a «billets» «payer» avec «dettes» , «créancier» et «intérêt»
il y a ainsi la forme "rente"qui est souvent précédé de "francs" qui montre que nous somme bien dans une société bourgeoise. 
ce qui se rapproche de la bourgeoisie: «capital» suivis dans les phrases de «intérêts» , «énorme» et «rentes» d’ailleurs beaucoup de forme superlatif « énorme» , «colossale», «immense» et «considérables» suivent ces groupe de formes. Mais aussi héritage avec notamment «viagère» on voit ici une classe qui concerne la bourgeoisie et la finance parisienne. 

quelques forme remarquable :
 la forme «capital» qui lui est liée a «argent» mais aussi «intellectuel».
La forme «fortune» est aussi souvent précéder de  «sa» , «ma» , «votre» , la désignation de la fortune d’autre.
D’autre forme comme «capital» suivit de plusieurs formes comme «rente» , «intérêt», «énorme».


Donc on un groupement purement économique liée aux échanges quotidiens mais aussi une partie qui concerne plutôt la grande bourgeoisie liée a la finance , aux capital, on voit ici donc que l’univers de Balzac montre les échanges du quotidien mais aussi le monde bourgeois du XVIII , constituer de grande fortune , capital liée a la finance et la rente.  


## Identifier les espaces dans Balzac


### Adopter un protocole pour identifier les lieux 

Le rapport d'honoré de Balzac à la géographie et à Paris à été de nombreuses fois mis en évidence et étudier[^n29]. L'objectif, ici, consistait à partir des textes, pour en extraire directement les lieux, les localisations et les représenter. Il s'agissait d'utiliser la notion d'étiquetage des formes que nous avons pu déjà rencontrer lors de la lemmatisation, pour extraire directements les lieux, ici les villes et rues, du texte. Nous aurions pu suivre une démarche différente dans la mesure où il existe une des ressources déjà constituées pour mettre en place un répertoire des lieux dans l'oeuvre.

## A Une première tentative autour des villes 
La reconnaissance d’entités nommées consiste à rechercher des objets textuels dans des corpus, qui peuvent être des noms d’organisations, des dates, ou bien des noms de lieux. Dans le cadre de l’oeuvre de Balzac nous avons rechercher tous les lieux afin de réaliser un _atlas_ des scènes de la _Comédie humaine_ . Le protocole que nous avons choisi d’appliquer peut se décomposer en sept points et en utilisant la bibliothèque [Spacy](https://spacy.io/)  :

1. _parsing_ de chacune des scènes. Chacun des termes se trouve étiquette (tokenisation).

2. on charge le modèle "fr_core_news_sm", il y a quatre tags : LOC (Locations), MISC, ORG(Organisations), PER (Persons)

3. Séléction des _tag_ ‘LOC’ pour Location

4. On compare les LOC avec la liste des villes françaises pour s’assurer qu’il n’y a pas d’erreur

5. On extrait le numéro d’identifiant pour trouver la géolocalisation. On utilise la bibliothèque _geocoder_.

6. Ensuite on va dénombrer pour chaque scène le nombre de fois que chaque lieu (ville) apparaît dans chaque scène.

7. on produit une carte par scène en utilisant les bibliothèques _pandas_ et _matplolib_



Le premier problème que nous avons rencontré concerne la bibliothèque _geocoder_ qui nécessite de s’inscrire sur une api [geonames](http://www.geonames.org/) et qui limite son utilisation à 1000 crédits. Nous avons donc du utiliser plusieurs connexions.


Les résultats que nous produisons pour chacune des scènes à partir des textes ne surprendra pas le spécialiste, mais il nous permettait de mieux hiérarchiser les villes françaises. 

- [Scènes de la vie de campagne](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_campagne.html) 
- [Scènes de la vie militaire](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_militaire.html)
- [Scènes de la vie parisienne](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_parisienne.html)
- [Scènes de la vie politique](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_politique.html)
- [Scènes de la vie privée](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_privee.html)
- [Scènes de la vie de province](https://rawcdn.githack.com/PirehP1/L3_Balzac/main/annexe/Villes/mapscene_vie_province.html)






## Rechercher le réseau urbain parisien 

Un des avantages de TXM réside, sans aucun doute, dans les fonctions CQL que ce logiciel abrite. Nous pourrions retrouver ces fonctions à l'aide du logiciel R, mais l'avantage graphique de TXM était pour nous évident. En ce qui concerne Paris au XIX<sup>e</sup> siècle un protocole d'analyse à été fixé dans (Montcla,2018)[^n30]. Le protocole est le suivant : 

1. Isoler dans le texte les concordances contenant les occurrences des segments de phrases répondant aux expressions rationnelles suivantes : 

```
> [frlemma = "rue|voie|passage|avenue|place|faubourg|boulevard|quartier|hôtel"][]{0,1}[frlemma = "de|le|du"][]{0,1}[frpos = "NAM"]

```

La première phase d'expression rationnelle conduit à 1150 retours, ce qui pour une oeuvre aussi importante semble peu important.

2. Nous avons utilisé la couche Vasserot Voies (1810-1836) extraite de l'application en ligne [Alpage](https://alpage.huma-num.fr/donnees-vasserot-version-1-2010-a-l-bethe/)

3. La réconciliation des données n'était pas très bonne et c'est la raison pour laquelle nos cartes ne représentent qu'une partie de l'information.
Ainsi manque t-il des lieux précis comme les hôtels particuliers, les maisons, les places. Une des solutions consiste à utiliser l'API (_Application Programming Interface_)[^n32] PERDIDO[^n31] qui permet de faire de la *Reconnaissance d'Entité Nommées* à partir de textes brutes. 









### Quelques essais de [Perdido](http://erig.univ-pau.fr/PERDIDO/)
Dans le cadre de cette expérimentation universitaire, Ludovic Moncla nous a aimablement donné une connexion à l'API pour l'utiliser. Cette méthode consiste essentiellement à soumettre chaque concordance à l'interface et de récupérer un tableau intégrant, les thèmes (vie de province, etc...), le type d'élément géographique (ville, rue, place) ainsi que le géoréférencement. 
De fait, l'identification du réseau _viaire_ demeure difficile à identifier. 
Afin d'identifier au mieux ces espaces nous avons utilisé les données fournies par Alpage. 
C'est évidemment peu, mais c'est une première approche de ce que pourrait être un atlas parisien Balsazien.  Pour cette étape nous avons du programmer un petit script en langage python pour automatiser le mieux possible ce processus. 


Il faudrait étendre ces recherches à présent en reprenant les lieux cités comme forme pôle et analyser leurs cooccurrents. 

## Annexes 


### Concordance classe 3 


### Le verbe "aller" 

[Lire les concordances dans le fichier](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/concordance_aller.csv)

 
[^n1]: Cf, https://fr.wikipedia.org/wiki/La_Com%C3%A9die_humaine  [consulté le 01/02/2022]
[^n2]: Pour une présentation et des prises en main du logiciel : http://www.iramuteq.org/ [consulté le 25/01/2022]
[^n3]: A. BEGUIN, Balzac lu et relu, Editions du Seuil, Paris, 1965, p. 117
[^n4]: En revanche, il serait possible d'étudier toute l'oeuvre de Balzac en suivant le temps de publication  cela reviendrait a accroitre le corpus. Selon la page wikipedia sur la comédie humaine il apparaît qu’en 1830 il publia 7 textes, on peut voir pour les texte ou les formes sont les plus basses comme en 1831 ne comporte que peut de texte 4 texte puis en 1832 3 textes pareil en 1846 4 textes et enfin en 1848 un seul texte, ainsi ces variations ne montre que la variation par années de ces écrits mais cela serait sortir de notre analyse.
[^n5]: Cf, Max Reinert, « La tresse du sens et la méthode Alceste. Application aux Réveries du promeneur solitaire », _JADT 2000_, 1993. http://lexicometrica.univ-paris3.fr/jadt/jadt2000/pdf/31/31.pdf [consulté le 25/01/2022]
[^n6]: Max Reinert, "Une méthode de classification descendante hiérarchique : application à l'analyse lexicale par contexte", /Cahiers de l'analyse des données/ Volume: 8, Issue: 2, 1983, pp. 187-198. La méthode a été intégrée au développement du logiciel Alceste.
[^n7]: Description du paramétrage.... 
[^n8]: Benzecri Jean-Paul, _L'analyse des Données_ (tome 1 et 2), Dunod, Paris, 1973.
[^n9]: Pour une présentation de plusieurs méthodes de coocurrences, William Martinez, " Au-delà de la cooccurrence binaire… Poly-cooccurrences et trames de cooccurrence ", _Corpus_ [En ligne], 11 | 2012, mis en ligne le 18 juin 2013, consulté le 19 avril 2022. URL : http://journals.openedition.org/corpus/2262 ; [DOI](https://doi.org/10.4000/corpus.2262)
[^n10]: Pour l'analyse factorielle sa présentation et son exploitation le manuel de Philippe Cibois, _Les méthodes d’analyse d’enquêtes_, « Que sais-je »,PUF, 2007  [Ici](https://books.openedition.org/enseditions/1443)
[^n11]: Voir les concordances de "heures du matin" [Ici](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/concordances_heures_du_matin.csv)
[^n12]: Voir les concordances de père [Ici](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/coocurences_matin.csv)
[^n13]: Voir les concoradance de lettres [Ici](https://github.com/PirehP1/L3_Balzac/blob/main/annexe/Concordances/coocurences_lettre.csv)
[^n29]: Christophe Morhange, Nathanaël Gobenceaux et Patrick Pentsch, "Géographie de Balzac. Portrait impressionniste de la France ?" , MappeMonde, 2018, http://mappemonde.mgm.fr/124as4/
[^n30]: Ludovic Moncla, Mauro Gaio, Thierry Joliveau, Yves-François Le Lay, "Automated Geoparsing of Paris Street Names in 19th Century Novels", _1st ACM SIGSPATIAL Workshop on Geospatial Humanities_,
Nov 2017, Redondo Beach, CA, United States. 10.1145/3149858.3149859. hal-01633344. Cette étude à été produite dans une large diachronie entre 1830 et 1913. Cet outil est évalué dans d'autres projets, comme : https://citedesdames.hypotheses.org/files/2020/02/Presentation-seminaire-29_01-Eleni-Kogkitsidou.pdf 
ou encore  Denis Vigier1,*, Ludovic Moncla2, Alice Brenon1, Katherine McDonough,3 et Thierry Joliveau4, "Classification des entités nommées dans l’Encyclopédie ou dictionnaire raisonné des sciences des arts et des métiers par une société de gens de lettres (1751-1772)",  SHS Web of Conferences 78, 11008 (2020) DOI : https://doi.org/10.1051/shsconf/20207811008
[^n31]: Cf, http://erig.univ-pau.fr/PERDIDO/ et http://erig.univ-pau.fr/PERDIDO/PERDIDO_API_specifications.pdf
[^n32]: Les interfaces de programmation d’applications, sont des applications internet qui offrent des services pour d'autres applications internet. 
 
 





