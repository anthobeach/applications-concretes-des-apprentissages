# Des applications déjà possibles en Licence MIASHS
Vous trouverez dans cette section quelques exemples d'applications qu'il est possible de faire, avec les connaissances et compétences acquises au cours des années de la Licence.

## Programmation de la Régression Linéaire Multiple (RLM)

> [!NOTE]
> Sa réalisation nécessite la manipulation d'outils mathématiques, statistique et Informatique. <br>
> La régression linéaire multiple permet d'estimer une variable quantitive à partir de variables explicant celle-ci.

### Diagramme des compétences à maitriser

```mermaid
flowchart LR
		subgraph le1[L1]
				subgraph se1[S1]
					subgraph stat1[Statistique]
				    id1(  Bases en probabilités <br> et statistique  )
			    end
			    subgraph info1[Informatique]
					id2(  Informatique 1: <br> programmation, <br> bases de l'algorithmique et <br> logique  )
				    id3((Ou))
				    id4(  Informatique 2: <br> algorithmique, <br> structures de données <br> élémentaires et introduction <br> à la complexité  )
			    end
			    subgraph math1 [Mathématiques]
         			id5(  Outils mathématiques  )
					id6((Ou))
					id7(  Mathématiques générales  )
					end
		    end
		    subgraph se2[S2]
			    subgraph math2[Mathématiques]
				    id8(  Algèbre  )
				  end
				  subgraph info2[Informatique]
					  id9(  Programmation et <br> Applications interactives  )
				  end
		    end
    end
    subgraph le2 [L2]
	    subgraph se4[S4]
		    subgraph stat2[Statistique]
			    id10(  Tests d'Hypothèses <br> et Régression  )
			  end
			end
    end
    subgraph le3 [L3]
	    subgraph se5 [S5]
		    subgraph info3 [Informatique]
			    id11(  Sciences des données  )
			  end
			end
	  end
    id12@{ shape: dbl-circ, label: Programmation d'une <br> régression linéaire multiple }
    %% clickable links
	    %% S1
	    click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27784"
	    click id2 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
	    click id4 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38899"
	    click id5 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38891"
	    click id7 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    %% S2
	    click id8 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27954"
	    click id9 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
	    %% S4
	    click id10 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=73987"
	    %% S5
	    click id11 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28193"
	 %% knowledge transfer
		 id1 -- Modélisation Statistique <br> d'une régression <br> linéaire simple --> id10
		 info1 -- Fondamentaux <br> algorithmiques  --> id9
		 math1 -- Bases algébriques --> id8
		 id8 -- Méthodes de résolution <br> d'un système linéaire --> id10
		 id9 -- Fonctions courantes --> id11
		 id10 -- Modélisation Statistique <br> d'une régression linéaire <br> multiple --> id11
		 id11 -- Modélisation informatique <br> d'une régression linéaire <br> multiple --> id12
```

### Exemple 
On cherche à déterminer le salaire d'un joueur de Basket en NBA en fonction de ses performances.<br>
Pour cela, on possède un tableau regroupant quelques statistiques sur des joueurs. <br>
**Voici un extrait du tableau :** <br>

| Nom           | Prénom     | Nationalité    | Moyenne de points par match  | Moyenne de rebonds captés par match  | Moyenne de passes décisives par match  | Score d'efficacité du joueur  | Salaire annuel (USD) |
| ------------- | ---------- | -------------- | ---- | ---- | ---- | ---- | -------------------- |
| Antetokounmpo | Giannis    | Grec           | 33.0 | 11.8 | 5.4  | 28.4 | 54 126 450 $         |
| Curry         | Stephen    | Américain      | 25.0 | 4.4  | 6.0  | 24.6 | 55 761 216 $         |
| James         | LeBron     | Américain      | 24.4 | 7.8  | 8.2  | 25.8 | 51 415 938 $         |
| Jokic         | Nikola     | Serbe          | 27.9 | 12.7 | 9.2  | 29.8 | 55 224 526 $         |
| Wembanyama    | Victor     | Français       | 22.4 | 10.8 | 3.6  | 21.7 | 12 160 800 $         |

Ainsi, la variable à estimer est `Salaire annuel (USD)`.

Les variables permettant d'expliquer le salaire sont : 
- `Moyenne de points par match`
- `Moyenne de rebonds captés par match `
- `Moyenne de passes décisives par match`
- `Score d'efficacité du joueur`

## Programmation de tests Statistique

> [!NOTE]
> Sa réalisation nécessite la manipulation d'outils mathématiques, probabiliste et informatique. <br>
> Le test statistisque permet de trancher entre une hypothèse nulle (H0) et une hypothèse alternative (H1).

### Diagramme des compétences à maitriser
```mermaid
flowchart LR
		subgraph le1 [L1]
			subgraph se1 [S1]
				subgraph statproba1[Probabilités & Statistique]
					id1( Bases en probabilités <br> et statistique )
				end
				subgraph info1 [Informatique]
			    id2( Informatique 1: <br> programmation, <br> bases de l'algorithmique et <br> logique )
				id3((Ou))
				id4( Informatique 2: <br> algorithmique, <br> structures de données <br> élémentaires et introduction <br> à la complexité )
			  end
		  end
		  subgraph se2[S2]
		   subgraph info2[Informatique]
			  id5( Programmation et <br> Applications interactives )
			 end
			end
		end
		subgraph le2[L2]
			subgraph se3[S3]
				subgraph info3 [Informatique]
					id6( Techniques d'enquêtes ) 
				end
				subgraph statproba2 [Probabilités & Statistique]
					id7( Probabilités #0040;A#0041; et <br> Statistique Inférentielle #0040;B#0041; )
				end
			end
		end
		id8@{ shape: dbl-circ, label: Programmation d'un <br> test statistique }
		
		%% clickable links
			%% S1
			click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27784"
	    	click id2 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
	   	 	click id4 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38899"
	    	%% S2
	    	click id5 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
	   	 	%% S3
	    	click id6 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28124"
	    	click id7 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27578"
	    
	  %% kwnoledge transfer
	  id1 -- Lois usuelles et <br> Statistique descriptives --> id7
	  info1 -- Bases <br> algorithmiques --> id5
	  id5 -- Fonctions <br> courantes --> id6
	  id7 -- Théorie des tests <br> statistiques --> id8
	  id6 -- Bases en langage <br> de programmation R --> id8
```
### Exemple
On cherche à savoir s'il existe une différence générationnelle dans la reconnaissance de styles musicaux différents. 

**Pour cela, on réalise un blindtest évalué selon 3 conditions :** 
- Retrouver le titre de la musique parmi 54 références musicales
- Retrouver le nom de l'artiste parmi 50 références musciales
- Retrouver le titre et le nom de l'artiste parmi 80 références musciales

**3 groupes sont constitués :** 
- Groupe A (Etudiant)
- Groupe B (Actif)
- Groupe C (Retraité)

**Les hypothèses suivantes sont établies :** 
1. Le groupe A reconnaitra mieux les chansons que le groupe B et C 
2. Le groupe B et C reconnaitront de façon équivalente les chansons

**Voici les résultats obtenus :**
![](https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/e2add63b6ea2e6db4582e3b94bdc17bc916d6207/images/moyenne_de%20scores_au_blindtest.svg)

> [!IMPORTANT]
> - Les étoiles qui sont présentes sur le graphique désignent le niveau de significativité de la comparaison d'un groupe par rapport à un autre. En d'autres termes, plus il y a d'étoiles, plus la différence est forte entre les deux groupes comparés. <br> 
> - L'intervalle que vous pouvez observé au niveau de chaque bar qui représente la moyenne, est un intervalle de confiance. Il permet de savoir dans le cas de cet intervalle, si la valeur observée se trouve bien dans la moyenne des valeurs recueillies. En d'autres termes, si la valeur observée ne se trouve pas dans cet intervalle, cela veut dire qu'elle ne fait pas partie des valeurs majoritairement observées.

<details>
	<summary> <strong> Pour la première hypothèse </strong>  </summary>
On constate qu'il existe à chaque fois, une différence significative entre le groupe A et les autres groupes. <br> 
Ce qui veut dire que l'hypothèse nulle globale (H0) selon laquelle il n'existe pas de différence entre le groupe A et les deux autres groupes est rejetée. On admet donc l'hypothèse alternative globale (H1) selon laquelle le groupe A est différent des deux autres groupes. <br>
Plus précisement, les différences sont plus marquées avec le groupe B que le groupe C. <br>
On peut conclure que l'hypothèse est validée. <br> <br>
</details>

<details>
	<summary> <strong> Pour la deuxième hypothése  </strong> </summary>
On constate alors, qu'il existe 2 fois sur 3, aucune différence significative entre les deux groupes. <br>
Pour le cas où la différence est présente, elle est sur le nombre de titres trouvés. <br>
Ce qui veut dire que l'hypothèse nulle globale (H0) selon laquelle il n'existe pas de différence entre le groupe B et C est admise. L'hypothèse alternative globale (H1) selon laquelle il existe une différence entre le groupe B et C est rejetée. <br>
On peut conclure que l'hypothèse est validée.
</details>


## Modélisation biomathématique
> [!NOTE]
> Sa réalisation nécessite l'utilisation d'outils mathématiques, informatique et de notions en biologie. <br>
> Elle permet de représenter des phénomènes biologiques sous une forme quantifiable afin d'extraitre des informations complémentaires.
### Digramme des compétences à maitriser

```mermaid
flowchart LR
		subgraph le1 [L1]
			subgraph se1 [S1]
				subgraph math1 [Mathématiques]
					id1( Outils mathématiques )
					id2((Ou))
					id3( Mathématiques générales )
		    	end
		    	subgraph info1 [Informatique]
					id4( Informatique 1: <br> programmation, <br> bases de l'algorithmique et <br> logique )
		    		id5((Ou))
			  		id6( Informatique 2: <br> algorithmique, <br> structures de données <br> élémentaires et introduction <br> à la complexité )
			  	end
	    end
	    subgraph se2[S2]
		    subgraph math2[Mathématiques]
			    id7( Analyse appliquée )
			    id8( Algèbre )
			  end
			  subgraph info2 [Informatique]
				  id9( Programmation et <br> Applications interactives )
				end
	    end
    end
    subgraph le2 [L2]
	    subgraph se3 [S3]
		    subgraph math3 [Mathématiques]
			    id10( Fonctions de plusieurs <br> variables et optimisation )
			  end
			end
		end
		subgraph le3 [L3]
			subgraph se5 [S5]
				subgraph math4 [Mathématiques]
					id11( Méthodes Numériques <br> Linéaires et Non linéaires )
				end
			end
			subgraph se6 [S6]
				subgraph math5 [Mathématiques]
					id12( Systèmes dynamiques et <br> Modélisation <br>  Biomathématique ) 
				end
			end
		end
		id13@{ shape: dbl-circ, label: Résolution de modèles <br> biomathématique }
		
    %% clickable link
	    %% S1
	    click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38891"
	    click id3 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    click id4 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
	    click id6 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38899"
	    %% S2
	    click id7 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27957"
	    click id8 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27954"
	    click id9 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
	    %% S3
	    click id10 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28020"
	    %% S5 
	    click id11 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77922"
	    %% S6
	    click id12 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77953"
    %% knowledge transfer
    math1 -- Base de l'analyse <br> des fonctions --> id7
    math1 -- Bases algébriques --> id8
    info1 -- Fondamentaux <br> algorithmiques  --> id9
    id7 -- Dérivations de fonctions --> id10
    id7 -- Suites numériques --> id12
    id8 -- Méthodes de résolution <br> d'un système linéaire --> id12
    id9 -- Fonction courantes --> id11
    id10 -- Dérivations partielles et <br> équations différentielles --> id12
    id11 -- Modélisation <br> mathématiques <br> et informatique --> id12
    id12 -- Méthodes pour modéliser <br> des phénomènes <br> biologiques --> id13
```
### Exemple

On cherche à modéliser la transmission des gènes entre les abeilles. <br>
Pour cela, on s'appuie sur l'illustration suivante : <br> <br>
![](https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/56ef74f67f3b49ac5c79f586eaf2535dfdceaa45/images/Asym%C3%A9tries%20g%C3%A9n%C3%A9tiques.jpg)

Cette illustration est extraite d'un [article de revue](https://www.erudit.org/fr/revues/ms/2003-v19-n4-ms517/006497ar/) paru dans médecine sciences. 

Comme on peut le voir sur cette illustration, la reine transmet la moitié de ses chromosomes alors que le mâle lui, la totalité. 
Cela s'explique par le fait que le mâle est issu directement de la reine (pas de fécondation de l'oeuf par un mâle). Il ne possède que pour partrimoine génétique, la moitié des gènes de la reine. 
Ses chromosomes sont tous identfiques. 
Ce qui a pour conséquence, une diversité génétique plus restreinte entre les mâles issu d'une même reine. <br> <br>

On constacte que par ce procédé, on a des différences de transmission de gènes qui conduisent alors à des liens de parenté différencié selon le sexe.
En prennant l'exemple de la *Fille a* issu de la reine et du mâle, elle a 25 % de gènes en commun avec son frère (*Fils*) contre 75 % de gènes en commun avec sa soeur (*Fille b*). 
La *Fille b* a même plus de gènes en commun avec son neveu (37,5 %) que son propre frère (25 %). <br> <br>
Ce phénomène que l'on appelle la dillution génétique, est un comportement qu'adopte la reine afin de réguler sa descendance. 
En faisant cela, la reine s'assure que ses filles s'occupent plutôt de sa propre descendance (leurs soeurs) que de la leur. 
La reine garde ainsi le contrôle sur la distribution génétique entre les générations, et indirectement, protége son statut de reine. 

# Les applications possibles en poursuivant en Master
Vous trouverez dans cette section quelques exemples d'applications qu'il est possible de faire, avec les connaissances et compétences acquises au cours des années de la Licence et du Master.
## Ergonomie des applications
> [!NOTE]
> Sa mise en oeuvre nécessite l'utilisation d'outils informatique et de connaissances spécifiques en sciences cognitives[^1]. <br>
> Elle permet d'évaluer et d'améliorer les interactions entre les utilisateurs et les ordinateurs, en se basant sur la cognition humaine[^2].
[^1]: Elles sont impliquées dans la description, l'explication et quand cela le nécessite, dans la simulation des principales dispositions et capacités de l'esprit humain (comme le langage, le raisonnement, la perception, la coordination motrice, la planification, ...).
[^2]: C'est l'ensemble des processus psychologiques et physiologiques qui permettent à un individu d'avoir une connaissance de son environnement et de lui-même.
### Digramme des compétences à maitriser

```mermaid
flowchart LR
		subgraph le1 [L1]
			subgraph se1 [S1]
				subgraph sc1 [Sciences Cognitives]
		    		id1( Introduction à la gestion <br> des organisations et <br> aux sciences cognitives )
		    	end
		    	subgraph info1 [Informatique]
                    id2( Informatique 1: <br> programmation, <br> bases de l'algorithmique et <br> logique )
					id3((Ou))
					id4( Informatique 2: <br> algorithmique, <br> structures de données <br> élémentaires et introduction <br> à la complexité )
               end
	    end
	    subgraph se2[S2]
			  subgraph info2 [Informatique]
				  id5( Programmation et <br> Applications interactives )
              end
	    end
    end
    subgraph le2 [L2]
	    subgraph se3 [S3]
		    subgraph sc2 [Sciences Cognitives]
			    id6( Bases de neurobiologie et <br> neuroanatomie, <br> fondamentaux cognitifs et <br> apprentissage )
			   end
			end
	    subgraph se4 [S4]
		    subgraph info3 [Informatique]
			    id7( Systèmes de gestion <br> de bases de données,<br> conception de sites <br> web dynamiques )
			  end
			end
		end
		subgraph le3 [L3]
			subgraph se6 [S6]
				subgraph sc3 [Sciences Cognitives]
					id8( Facteur Humain et <br> Ergonomie) 
				end
			end
		end
		subgraph mr1 [Master]
			subgraph sc4 [Sciences Cognitives]
				id9(Modélisation en <br> psychologie)
			end
			subgraph info4 [Informatique]
				id10(Technologies web avancées)
			end
		end
		id11@{ shape: dbl-circ, label: Création d'applications <br> ergonomiques}
		
    %% clickable link
	    %% S1
	    click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27787"
	    click id2 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    click id4 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
	    %% S2
	    click id5 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
	    %% S3
	    click id6 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27994"
	    %% S4
	    click id7 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=52819"
	    %% S6
	    click id8 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77961"
    %% knowledge transfer
    info1 -- Bases <br> algorithmiques  --> id5
    id1 -- Base du traitement <br> de l'information --> id6
    id5 -- Fonctions courantes et <br> interface graphique --> id7
    id6 -- Composants cognitifs <br> impliqués dans <br> une tâche --> id8
    id7 -- Langage web et <br> gestion de <br> bases de données --> id10
    id8 -- Connaissances générales <br> sur l'ergonomie --> id9
    id9 -- Concepts fondamentaux <br> en ergonomie <br> des applications --> id11
    id10 -- Framework de <br> développement web <br> et application mobile --> id11
```
### Exemple

Une entreprise fait appel à nos services afin d'améliorer son expérience utilisateur[^3].
Elle souhaite que nous lui fassions un retour sur les différentes nouveautés qu'elle pourrait inclure pour compléter son offre déjà existante. <br> <br>
Pour cela, nous commençons par analyser les applications déjà disponibles actuellement sur le marché. <br>
Voici l'une des applications analysées : <br> <br>
![](https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/02d2556a58ccf17c1fe21c95667d6f4faa1dc052/images/Ecrans%20principaux%20de%20l'application%20Helpilepsy.png)

Cette analyse se fait selon 3 axes : 
- Le design[^4]
- La navigation[^5]
- Les fonctionnalités[^6]

**Pour le design :** 
<details>
	
<summary> + </summary>

- Lisibilité des informations de suivi (prise de médicaments, espacement des crises, ...) et de celles à renseigner (ajout ou modification du traitement, d'une crise, ...)
- Représentation graphique épurée (visibilité des crises sur la semaine, le mois ou l'année)  
  
</details>

<details>
	<summary> - </summary>
	
- Bouton pour accéder aux graphiques plus détaillés un peu grossié (sur l'écran d'accueil)
- Impression d'une liste interminable (sur l'écran paramètres)

</details>

**Pour la navigation :** 
<details>
	
<summary> + </summary>

Fluidité de passage entre les différents éléments de l'écran (pour ajouter, modifier ou consulter des traitements, ...)
  
</details>

<details>
	<summary> - </summary>

- Avoir la possibilité de revenir automatiquement sur le jour actuel si on change d'écran (sur l'écran journal)
- Devoir swiper vers le haut ou le bas longtemps pour accéder à une date éloignée (sur l'écran journal)

</details>

**Pour les fonctionnalités :** 
<details>
	
<summary> + </summary>

- Affichage de représentations graphiques compréhensibles (crises survenues dans la semaine, humeurs, ...)
- Gestion de tous les événements courants (traitement, crise, note, effet secondaire, rendez-vous, rappels)
- Gestion de l'application (compte, notifications et assitance)
- Gestion d'un bracelet connecté pour détecter les crises nocturnes
  
</details>

<details>
	<summary> - </summary>

- Renseigner la cause d'un effet secondaire (sur l'écran journal)
- Avoir la possibilité de revenir en arrière si on s'est trompé

</details>


[^3]: Elle désigne l'interaction entre un utilisateur (qui a des attentes, des besoins, ...), un système (qui a des fonctionnalités, une esthétique, ...) et un contexte (utilisation du système à la maison, au travail, ...).
[^4]: Il fait référence aux différents éléments visuels qui composent l'application (la mise en page, l'équilibre des couleurs, la cohérence graphique, ...).
[^5]: Il désigne la manière dont l'utilisateur parcours les différents contenus de l'application (le menu, les listes déroulantes, les boutons, ...).
[^6]: Elles se définissent comme les différentes actions qui sont intégrées dans l'application (ajouter, supprimer, modifier, ...).

## Interface Cerveau Ordinateur (ICO)
> [!NOTE]
> Sa réalisation nécessite des outils mathématiques, probabiliste et informatique mais également des connaissances spécifiques en sciences cognitives.<br>
> Il permet d'améliorer ou d'explorer des fonctions du système nerveux central[^7] afin d'assurer principalement le contrôle et la communication.

### Diagramme des compétences à maitriser

```mermaid
flowchart LR
		subgraph le1 [L1]
			subgraph se1 [S1]
				subgraph sc1 [Sciences Cognitives]
			    id1( Introduction à la gestion <br> des organisations et <br> aux sciences cognitives )
		    end
		    subgraph info1 [Informatique]
				id2( Informatique 1: <br> programmation, <br> bases de l'algorithmique et <br> logique )
			    id3((Ou))
				id4( Informatique 2: <br> algorithmique, <br> structures de données <br> élémentaires et introduction <br> à la complexité )
			  end
			  subgraph math1 [Mathématiques]
					id5( Outils mathématiques )
					id6((Ou))
					id7( Mathématiques générales )
				end
				subgraph proba1[Probabilités]
					id8( Bases en probabilités <br> et statistique )
				end
	    end
	    subgraph se2[S2]
			  subgraph info2 [Informatique]
				  id9( Programmation et <br> Applications interactives )
				end
				subgraph math2[Mathématiques]
				  id10( Algèbre )
				  id11( Analyse appliquée )
				end
	    end
    end
    subgraph le2 [L2]
	    subgraph se3 [S3]
		    subgraph sc2 [Sciences Cognitives]
			    id12( Bases de neurobiologie et <br> neuroanatomie, <br> fondamentaux cognitifs et <br> apprentissage )
			   end
			  subgraph math3 [Mathématiques]
				  id13( Séries et <br> intégrales multiples )
				  id14( Fonctions de plusieurs <br> variables et optimisation )
				end
				subgraph proba2 [Probabilités]
					id15( Probabilités #0040;A#0041; et <br> Statistique Inférentielle #0040;B#0041; )
				end
			end
	    subgraph se4 [S4]
			  subgraph sc3 [Sciences Cognitives]
				  id16( Perception, action, <br> mémoire et <br> fonctions exécutives )
				end
				subgraph math4 [Mathématiques]
					id17( Algèbre 2 #0040;A#0041; et <br> Espaces Euclidiens #0040;B#0041; )
				end
			end
		end
		subgraph le3 [L3]
			subgraph se5 [S5]
				subgraph sc4 [Sciences Cognitives]
					id18( Neuropsychologie, <br> neuropathologie <br> et imagerie cérébrale )
				end
				subgraph math5 [Mathématiques]
					id19( Méthodes Numériques <br> Linéaires et <br> Non linéaires )
				end
				subgraph info3 [Informatique]
					id20( Apprentissage machine <br> et Imagerie numérique )
				end
			end
		  subgraph se6 [S6]
				subgraph sc5 [Sciences Cognitives]
					id21( Psychophysiologie, <br> Neuroergonomie <br> / Traitement du Signal <br> et Neurosciences <br> Computationnelles ) 
					id22( Connaissances et <br> représentations, <br> langage et TAL )
				end
				subgraph proba3 [Probabilités]
					id23( Processus Aléatoires <br> et Séries Chronologiques </ul>)
				end
				subgraph math6 [Mathématiques]
					id24( Systèmes dynamiques <br> et Modélisation <br> Biomathématique </ul>)
				end
		  end
		end
		subgraph mr1 [Master]
			subgraph info4 [Informatique]
				id25(Interfaces <br> Cerveau-Ordinateur)
				id26(Réseaux de neurones)
			end
		end
		id27@{shape: dbl-circ, label: Création d'une interface <br> cerveau ordinateur}
		
    %% clickable link
	    %% S1
	    click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27787"
	    click id2 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    click id4 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
	    click id5 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38891"
	    click id7 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    click id8 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27784"
	    %% S2
	    click id9 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
	    click id10 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27954"
	    click id11 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27957"
	    %% S3
	    click id12 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27994"
	    click id13 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28115"
		click id14 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28035"
	    click id15 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27578"
	    %% S4
	    click id16 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77959"
	    click id17 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77922"
	    %% S5
	    click id18 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77963"
	    click id19 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77922"
	    click id20 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77923"
	    %%S6
	    click id21 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77963"
	    click id23 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77951"
	    click id22 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77957"
	    click id24 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77953"
    %% knowledge transfer
    info1 -- Bases <br> algorithmiques  --> id9
    math1 -- Bases <br> algébriques --> id10
    math1 -- Base de l'analyse <br> de fonctions --> id11
    id1 -- Base du traitement <br> de l'information --> id12
    id8 -- Lois uselles --> id15
    id9 -- Fonctions courantes et <br> interface graphique --> id20
    id12 -- Composants cognitifs <br> impliqués dans <br> une tâche --> id16
    id11 -- Base de <br> l'integration --> id13
    id11 -- Base de <br> la dérivation --> id14
    id10 -- Méthodes de résolution <br> d'un système <br> linéaire --> id17
    id14 -- Dérivation partielle --> id19
    id17 -- Caractéristiques <br> d'un système <br> linéaire --> id19
    id19 -- Méthodes de résolution <br> numérique --> id24
    id24 -- Stabilité d'un système --> id26
    id16 -- Processus cognitifs <br> à l'oeuvre <br> pour différentes <br> conditions --> id18
    id18 -- Base de l'anayse <br> cérébrale <br> pathologique et <br> non pathologique --> id21
    id13 -- Analyse avancée <br> d'intégrales et <br> de séries --> id21
    info1 -- Base de la <br> logique --> id22
    id22 -- Base du traitement <br> d'un réseau <br> de neurones <br> artficielles --> id26
    id21 -- Interprétation des <br> résultats du réseau <br> de neurones --> id25
    id26 -- Classification des <br> potentiels évoqués --> id25
    id15 -- Variables aléatoires --> id23
    id23 -- Processus stochastiques --> id26
    id20 -- Transformations <br> des données --> id26
    id25 -- Méthodes numériques <br> d'analyse des <br> potentiels évoqués --> id27
    id21 -- Traitement du signal EGG --> id26
```
### Exemple
On cherche à concevoir de nouvelles technologiques qui pourraient aider les enfants ayant des Troubles de l'Attention avec ou sans Hyperactivité (TDA/H)[^8].<br>
Pour cela, on fait une analyse des technologies déjà développées pour ce type de pratique et on interroge un panel d'enfants pour vérifier leurs besoins.
On test nos différentes versions auprès des enfants. <br> <br>
On aboutit au final à une application mobile où l'enfant pourra soit choisir un jeu parmi ceux proposés, soit créer son propre jeu. 
La création de son propre jeu, reposera sur des thématiques de jeu déjà existantes, qui seront personnalisées selon les demandes de l'enfant. 
Ces demandes pourront se faire à l'écrit ou à l'oral. 
Un modèle d'IA générative conçu par nos soins, se chargera de rendre réalisable les requêtes des enfants. <br><br>

Voici le schéma expérimental que nous avons mis en place :
![](https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/40a4b78eacc362212fe6ca78f41f8dadc661ab9e/images/Exemple%20d'ICO/Sch%C3%A9ma%20exp%C3%A9rimental%20d'une%20interface%20cerveau%20ordinateur.png)
Détails des étapes : <br> <br>
 <img src="https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/441de921469e738f53728654a5dff620e0484be5/images/Exemple%20d'ICO/Etape%201.svg" width=6%/> <br>
Cette première étape consiste à récupérer l'ensemble des informations qui serviront à analyser le comportement (c'est à dire, ce qui est transmis par la tablette, représenté par la flèche <strong> Etat du jeu </strong> sur notre schéma ; exemples : temps pour réaliser une action, choix des équipements, réussite de la mission,  ...) et le cerveau (c'est à dire, ce qui est transmis par la casque, représenté par la flèche <strong> Activité électrique du cerveau </strong> sur notre schéma ; exemple : signaux électriques de différentes régions du cerveau). <br> <br>
<img src="https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/441de921469e738f53728654a5dff620e0484be5/images/Exemple%20d'ICO/Etape%202.svg" width=6%/> <br>
Les informations ainsi recueillies par la box internet vont être envoyées en temps réel sur un serveur qui va traiter les données. <br> 
Ce sont principalement les informations liées à l'activité électrique du cerveau qui vont suivre ce traitement : 
<details>
	<summary><strong>Amplifier</strong></summary>
Les signaux électriques provenant de l'activité du cerveau vont être amplifiés de façon à les rendre exploitable (ils arrivent avec une faible intensité électrique).
</details>
<details>
	<summary><strong>Filtrer</strong></summary>
Les signaux électriques vont être épurés de manière à ne conserver que le signal qui est utile à exploiter (exemples : suppression des bruits parasites comme les petits mouvements de la tête, isoler une partie de la fréquence que l'on souhaite étudier, ...).
</details>
<details>
	<summary><strong>Classifier</strong></summary>
Les signaux alors obtenus vont être comparés à de précédents signaux afin de déduire le niveau de vigilance du joueur.
</details>
<details>
	<summary><strong>Contrôler</strong></summary>
Le niveau de vigilance déduit après ces traitements et l'analyse des actions du joueur, vont amener à l'application de règles.
</details>
<img src="https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/441de921469e738f53728654a5dff620e0484be5/images/Exemple%20d'ICO/Etape%203.svg" width=6%/> 
Une fois celles-ci établies, elles vont être transférées via internet. La boxe internet à son tour, va relayer les instructions. Elles vont avoir pour conséquence de modifier ou non le jeu. <br>
<details>
	<summary><strong>Exemples</strong></summary>
<ul>
	<li>Si le joueur est moins attentif, des actions du personnage ne pourront pas être faites</li>
	<li>Si le joueur est trop impusif, des actions du personnage seront ralenties</li>
</ul> 
</details>
<img src="https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/441de921469e738f53728654a5dff620e0484be5/images/Exemple%20d'ICO/Etape%204.svg" width=6%/>
Les retours pourront se faire sous forme de messages et de modifications du comportement du personnage.<br>
<details>
	<summary><strong>Exemples</strong></summary>
<ul>
	<li>Pour un joueur moins attentif, un message motivant et un affichage de chaque effort de concentration qui améliore l'action du personnage</li>
	<li>Pour un joueur trop impulsif, un message d'apaisement et un affichage de chaque effort pour se ramener à une concentration qui améliore l'efficacité du personnage</li>
</ul>
</details>

[^7]: Elles permettent de contrôler et de réguler (exemples : les mouvements, le langage, la vision, les sensations, ...).
[^8]: Ils se caractérisent par le développement inégaux de niveaux d'inattention, d'hyperactivité et d'impulsivité.

## Gestion de projet
> [!NOTE]
> Sa mise en partique nécessite des outils mathématiques, informatique, statistique et probabiliste ainsi que des connaissances spécifiques en économie-gestion.<br>
> Elle permet de définir un processus pour coordonner, gérer et planifier le développement d'un projet.

### Digramme des compétences à maitriser
```mermaid
flowchart LR
		subgraph le1 [L1]
			subgraph se1 [S1]
				subgraph ecog1 [Eco-gestion]
					id1(Introduction à la gestion des organisations et aux sciences cognitives)
	            end
				subgraph statproba1[Probabilités & Statistique]
					id2(Bases en probabilités et statistique)
				end
				subgraph math1 [Mathématiques]
         			id3(Outils mathématiques)
					id4((Ou))
					id5(Mathématiques générales)
				end
				subgraph info1 [Informatique]
					id6(Informatique 1: programmation, bases de l'algorithmique et logique )
				    id7((Ou))
					id8( Informatique 2: algorithmique, structures de données élémentaires et introduction à la complexité )
			    end
			end
			subgraph se2 [S2]
				subgraph ecog2 [Eco-gestion]
					id9(Introduction aux sciences économiques)
				end
				subgraph info2 [Informatique]
				  	id10(Programmation et Applications interactives)
				end
				subgraph math2 [Mathématiques]
					id11(Analyse appliquée)
				end
			end
		end
		subgraph le2 [L2]
			subgraph se3 [S3]
				subgraph statproba2 [Probabilités & Statistique]
					id12(Probabilités #0040;A#0041; et Statistique Inférentielle #0040;B#0041;)
				end
				subgraph math3 [Mathématiques]
				  id13(Séries et intégrales multiples)
				end
				subgraph info3 [Informatique]
					id14(Techniques d'enquêtes) 
				end
				subgraph ecog3 [Eco-gestion]
					id15(Techniques Comptables)
				end
			end
			subgraph se4 [S4]
				subgraph info4 [Informatique]
					id16(Systèmes de gestion de bases de données, conception de sites web dynamiques)
				end
				subgraph stat1 [Statistique]
					id17(Tests d'Hypothèses et Régression)
				end
				subgraph egcog4 [Eco-gestion]
					id18(Initiation au Droit de l'entreprise)
				end
			end
		end
		subgraph le3 [L3]
			subgraph se5 [S5]
				subgraph ecog5 [Eco-gestion]
					id19(Santé publique)
				end
			end
			subgraph se6 [S6]
				subgraph ecog6 [Eco-gestion]
					id20(Gestion responsable des Ressources Humaines)
				end
				subgraph math4 [Mathématiques]
					id21(Processus Aléatoires et Séries Chronologiques)
				end
			end
		end
		subgraph mr1 [Master]
			subgraph ecog7 [Eco-gestion]
				id22(Conception et développement)
				id23(Analyse fonctionnelle et cahier des charges)
			end
		end
		id24@{shape: dbl-circ, label: Mener un projet}
		%% clickable links
			%% S1
			click id1 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27787"
			click id2 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27784"
			click id3 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38891"
	    	click id5 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
			click id6 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38892"
	    	click id8 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=38897"
			%% S2
			click id9 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27924"
			click id10 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27565"
			%% S3
			click id11 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27957"
			click id12 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=27578"
			click id13 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28115"
			click id14 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28124"
			click id15 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=73949"
			%% S4
			click id16 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=52819"
			click id17 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=73987"
			click id18 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=28032"
			%% S5
			click id19 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77929"
			%% S6
			click id20 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77947"
			click id21 "https://formations.u-bordeaux.fr/details-formation?type=enseignement&id=77951"
		%% knowledge tranfer
		id1 -- Cadre d'une organisation --> id18
		id2 -- Lois usuelles et statistiques descriptives --> id12
		math1 -- Base de l'analyse de fonctions --> id11
		info1 -- Bases algorithmiques --> id10
		id9 -- Courants économiques --> id23
		id10 -- Fonctions courantes --> id16
		id11 -- Base de l'intégration --> id13
		id12 -- Théorie des tests statistiques --> id17
		id13 -- Analyse avancée d'intégrales et de séries --> id21
		id14 -- Méthodes d'analyses quantitatives et qualitatives --> id22
		id14 -- Méthodes d'investigations --> id19
		id15 -- Calcul d'un budget --> id23
		id16 -- Langage web et gestion de bases de données --> id22
		id17 -- Modélisations statistiques --> id22
		id18 -- Base de la réglementation des entreprises --> id20
		id19 -- Politiques publiques et interventions adpatées --> id22
		id20 -- Techniques de gestion du personnel --> id22
		id21 -- Analyse avancée des évolutions au <br> cours du temps --> id23
		id22 -- Processus du projet --> id24
		id23 -- Préparation du projet --> id24
```
### Exemple
Une entreprise fait appel à nos services pour lui développer un site web sur la vente de patisseries haut de gamme en ligne. <br>
Voici une manière d'organiser ce projet : <br> <br>
![](https://github.com/anthobeach/applications-concretes-des-apprentissages/blob/4124b2d288989f1fc52279d67fca2605585d1e2d/images/Organisation%20d'un%20projet%20autour%20d'un%20site%20web.png)

On commence tout d'abord par une présentation de l'équipe :
<details>
<summary><strong>Développeur front-end</strong></summary>
	
Il est spécialisé dans la partie visible par l'utilisteur,  ce qui s'affiche à l'écran et les interactions (interfaces, graphismes, navigation, animations, ...).
</details>

<details>
<summary><strong>Développeur back-end</strong></summary>
	
Il est spécialisé sur la partie invisible, la gestion des serveurs, des bases de données, la logique métier, la sécurité et les performances de l'application.
</details>

<details>
<summary><strong>Développeur full stack</strong></summary>
	
Il est capable à la fois de faire du développement front-end et back-end. Ce qui veut dire, qu'il maitrise toute le processus de développement technique, de la conception de l'interface utilisteur à la gestion des données et des serveurs.
</details>

<details>
<summary><strong>Analyste de marché</strong></summary>
	
Il est chargé de collecter, analyser et interpréter des données relatives à un marché, à la concurrence et aux consomateurs. Cela pour founir des recommandations stratégiques à une entreprise ou une organisation.
</details>

<details>
<summary><strong>Chef de projet</strong></summary>
Il est chargée de coordonner, piloter et gérer la réalisation de projets pour une entreprise ou une organisation, de la conception jusqu'au déploiement final.
</details>

<details>
<summary><strong>UX designer</strong></summary>
	
De son nom développé User eXperience designer, il conçoit et optimise l'expérience utilisateur[^3] d'un produit ou d'un service numérique, en s'appuyant sur les besoins, les attentes et les comportements des utilisateurs.
</details>

<details>
<summary><strong>UI designer</strong></summary>
	
De son nom développé User Interface designer, il conçoit l'interface visuelle d'un produit numérique telle que, une application, un site web ou un logiciel.
</details>

> [!IMPORTANT]
> Pour mieux comprendre cette planification, il faut savoir que chaque membre de l'équipe est affecté à plusieurs projets en même temps ayant des niveaux d'avancements hétérogènes.
> L'entreprise employant des profils très spécifiques (souvent avec des rémunérations élevées), doit utiliser leurs compétences et leurs efficacités afin de rentabiliser ses investissements.
> Cela lui permet également de proposer des offres sur mesure à ses clients, dans des délais résonnables.

On va décortiquer les différentes étapes du projet : 
<details>
<summary><strong>1. Recherche et construction d'une première ébauche du site web</strong></summary>	
	
- Elle s'étalle sur 1 semaine (du **15 au 19 janvier**)
- Elle consite à étudier les différentes opportunités du marché (`Etude de marché`) et concevoir une première version du système de vente (`Conception UML`)
</details>

<details>
<summary><strong>2. Elaboration de la base du site web</strong></summary>	
	
- Elle s'étalle sur 1 semaine (du **22 au 26 janvier**)
- Elle consiste à se baser sur la première ébauche en l'améliorant. Pour cela, un examen plus spécifique du marché (`Etude de marché`) mais également, une délimitation précise des besoins des clients et des utilisateurs du site web (`Analyse des besoins`). Une deuxième version du système de vente est alors établi (`Conception UML`)
</details>

<details>
<summary><strong>3. Conception d'une maquette du site web</strong></summary>	

- Elle s'étalle sur 1 semaine (du **29 janvier au 2 février**)
- Elle consite à créer un modèle structurel (`Création d'une base de données`) et visuel (`Conception de l'interface`) du site, en se référent à la deuxième version du système de vente. Dans le même temps, des patenariats et des sous-traitances sont cherchés (`Affilation avec les partenaires & sous-traitant`) afin pour l'un, de développer les opportunités de collborations et pour l'autre, externaliser certains services comme la commande à emporter
</details>

<details>
<summary><strong>4. Développement du site web</strong></summary>
	
- Elle s'étalle sur 3 semaines (du **5 au 23 février**)
- Elle consiste à coder l'ensemble du site en se basant sur la maquette.<br>
  Plus particulièrement :
	- Toute la structure numérique du site (`Création de l'architecture du site`) comme la sécurité, la cohérence entre les pages, le format des pages
	- L'interface graphique (exemples : boutons, menu, mise en page, ...) et les fonctionnalités (exemples : mettre une patisserie dans le panier d'achat, choisir la quantité, personnaliser un gateau, ...) du site (`Programmation front et back-end`)
	- Plusieurs versions du site vont être réalisées selon l'évolution des besoins du client, la faisabilité dans le temps imparti, les partenariats et sous-traitances concluent (`Affilation avec les partenaires & sous-traitant`)
</details>

<details>
<summary><strong>5. Finalisation du site web</strong></summary>

- Elle s'étalle sur 3 semaines et demi (du **26 février au 21 mars**)
- Elle consiste à faire les derniers réglagles avec l'assemblage de toutes les parties développées (`Lien avec la base de donnèes`) et la vérification du site (`Test du site web`) selon les attentes des clients, des utilisateurs, des sous-traitants et des partenaires. En toute fin, le chef de projet s'assure de la bonne conformité entre les attentes et la réalisation (`Validation du site`)
</details>
