# Séance 3 : TEI

## Introduction
 
 **Quels sont les avantages de TEI ?**
 
 * Le XML TEI s’intéresse au sens du texte plutôt qu’à son apparence; 
 * Le XML TEI est indépendant de tout environnement logiciel particulier;
 * Le XML TEI a été conçu par la communauté scientifique qui est aussi en charge de son développement continu.

Lou Burnard et Marjorie Burghart, *Qu’est-ce que la Text Encoding Initiative ?*, 2015.

 ---
 
## Naissance de la TEI
 
  Lou Burnard et Marjorie Burghart, *Qu’est-ce que la Text Encoding Initiative ?*, 2015 :
	
"La TEI a été d’abord développée, il y a plus de trente ans, comme un projet de recherche dans le champ alors émergent du « Humanities computing ». L’idée originelle était de proposer un ensemble de recommandations sur la façon dont les chercheurs devraient créer des ressources textuelles « lisibles par ordinateur », qui soient adaptées aux besoins de la recherche – dans la mesure où un consensus existait sur le sujet –, mais qui soient également extensibles, puisque ces besoins changent et évoluent."

---

 
**Quelques dates**

* 1987 : établissement de la *Text Encoding Initiative*;
* 1990 : [TEI P1 (proposal 1)](http://www.tei-c.org/Vault/Vault-GL.html), dir. Michael Sperberg-McQueen et Lou Burnard;
* 1992-1993 : TEI P2, expansion;
* 1994 : [TEI P3](http://www.tei-c.org/Vault/GL/P3/index.htm), première version complète;
* 2000 : naissance du TEI Consortium;
* 2001-2004 : TEI P4, introduction du XML;
* 2007-... : [TEI P5](http://www.tei-c.org/Guidelines/P5/), abandon de SGML.

---

## La communauté TEI

La communauté TEI est animée par le *TEI consortium*, fondation interdisciplinaire à but non lucratif.

Il se compose des unités suivantes:

* [TEI Board of Directors](http://www.tei-c.org/Board/);
* [TEI Technical Council](http://www.tei-c.org/Activities/Council/index.xml);
* [Membres institutionnels et individuels](http://members.tei-c.org/);
* [TEI Workgroups](http://www.tei-c.org/Activities/Workgroups/), par ex. :
  * [TEI Manuscripts Special Interest Group](http://www.tei-c.org/Activities/SIG/Manuscript/);
  * [Correspondence SIG](http://www.tei-c.org/Activities/SIG/Correspondence/);
* [Special Interest Groups](http://www.tei-c.org/Activities/SIG/).

---

La communauté peut échanger et se rencontrer grâce à :

* Une liste de diffusion : [TEI-L mailing list](https://listserv.brown.edu/?A0=TEI-L);
* Une liste francophone :  [TEI-FR](https://groupes.renater.fr/sympa/info/tei-fr) et un wiki;
* Des members meetings (congrès) annuels* Des congrès annuels : [TEI Conference](http://www.tei-c.org/Membership/Meetings/);
* Une revue : [*Journal of the Text Encoding Initiative*](http://jtei.revues.org/);
* Des **[Guidelines](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html)** ("recommandations") qui documentent notamment chaque élément.
---

## TEI, mode d'emploi

TEI est un set de balises prédéfini et documenté dans les [TEIguidelines](http://www.tei-c.org/guidelines/) qui permet de procéder à une description « scientifique » et « sémantique » d’un texte. 

Pour utiliser un set de balises TEI, il faut déclarer le nom de domaine TEI (name space) dans l'élément racine du document XML grâce à ce qu’on appelle une adresse URI qui pointe vers une description du set de données.

Exemple : `<TEI xmlns="http://www.tei-c.org/ns/1.0">`

---

TEI (All) ne propose pas un schéma de données à proprement parler, mais plutôt un éventail de possibilités, utile à la conception de son propre schéma. Il est fortement déconseillé d’utiliser un schéma englobant l’intégralité de la TEI. 

**La conception d’un modèle adapté à ses données et son projet, ainsi qu'à l’exploitation des documents, est une étape extrêmement importante dans la conception d'une édition numérique.**