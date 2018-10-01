# Séance 5 : Initiation à l’édition scientifique

---

## Les enjeux et les métiers de l’édition

---

Les éditions ont pour but de rendre accessible et compréhensible un texte pour un lectorat donné.

Il existe différentes formes d'édition (liste non exhaustive) :

* Les éditions génétiques
	* [Madame Bovary  : l'histoire du texte à travers ses brouillons](http://www.bovary.fr/folio_visu.php?folio=458&mode=sequence&mot)
* Les éditions "paléographiques"
	* [Le Didascalicon d’Hugues de Saint-Victor](http://theleme.enc.sorbonne.fr/dossiers/vue100.php)
* Les éditions critiques
	* [La Queste del saint Graal](http://txm.ish-lyon.cnrs.fr/bfm)

---

### Les enjeux d'une édition "paléographique"

#### Donner une représentation matérielle du texte :

- Mise en page;
- Mise en valeur typographique;
- Graphie originale du texte.

NB : Dans une édition numérique, il est conseillé d'utiliser les caractères UTF-8. 
Il existe des [fontes spécialisées](https://folk.uib.no/hnooh/mufi/fonts/) dans la représentation des manuscrits : 

* Palemonas MUFI
* Junicode 

---

#### Éditer le texte :

- Résolutions des abréviations;
- Régularisations des graphies;
- Corrections (si nécessaires).

---

#### Définitions des enjeux 

 - Identifier et délimiter les phénomènes à signaler;
 - Définir les futurs usages de l'édition;
 - Choisir son protocole d'encodage;
---

#### Les solutions TEI 

* Le set pour la [structuration des textes](http://www.tei-c.org/release/doc/tei-p5-doc/fr/html/DS.html)
* Le set pour la [description des sources primaires](http://www.tei-c.org/release/doc/tei-p5-doc/fr/html/PH.html)

---

*Quelques balises courantes*

* `<lg>` contient un groupe de vers fonctionnant comme une unité formelle, par exemple une strophe, un refrain, un paragraphe en vers;
* `<l>` contient un seul vers;
* `<lb>`marque le début d'une nouvelle ligne;
* `<pc>`contient un caractère ou une chaîne de caractères considérés comme un signe de ponctuation:
* Pour les développements d’abréviations : `<choice><abbr></abbr><expan></expan></choice>`;
* Pour les régularisations  : `<choice><orig></orig><reg></reg></choice>`.

---

## Mise en pratique

*Encoder la séquence de sainte Eulalie*

* Lecture interactive : <https://bibliotheque.ville-valenciennes.fr/iguana/www.main.cls?v=6bb63866-fa45-4563-a75e-626d3cccb43c>
* Voir le manuscrit sur Gallica : https://gallica.bnf.fr/ark:/12148/btv1b84526286
* Obtenir le texte sur wikisource :
<https://fr.wikisource.org/wiki/Séquence_de_sainte_Eulalie>

---

# Décrire ses sources

---

## EAD (Encoded Archival Description)

EAD est une DTD (un schéma d’utilisation) de XML.

* 2000, encodage en XML EAD du catalogue général des manuscrits des bibliothèques publiques de France.
* 2010, la DeMarch recommandation est publiée.
	* Attention : : DeMArch est une règle de description indépendante du format informatique.
* 2012, deux tiers des manuscrits et documents d’archives conservés par les bibliothèques françaises sont décrits en EAD (« BnF archives et manuscrits », Calames, le sous-domaine « Manuscrits » du Catalogue collectif de France CCFr).	

---
### Quelques exemples 

* [Inventaire du fonds du Théâtre de Poche-Montparnasse (1942-2011)](https://ccfr.bnf.fr/portailccfr/jsp/index_view_direct_anonymous.jsp?record=eadcgm:EADC:BHPCT0200001)
	* [Voir le fichier XML](./InvThMontparnasse.xml)

* [Catalogue du fonds général, Ms 1 à Ms 721](https://ccfr.bnf.fr/portailccfr/jsp/public/index.jsp?action=public_direct_view&record=eadcgm:EADI:FRCGMBPF-751045102-01a.xml)
	* [Voir le fichier XML](./catMS.xml)

---
### Pour résumer

Extrait de Florent Palluault, « Informatiser des descriptions complexes : l’utilisation de l’EAD et de la TEI pour les manuscrits et les livres anciens en France », *IFLA 2012 (Helsinki)*, [en ligne : http://conference.ifla.org/past/2012/212-palluault-fr.pdf.

"La nécessité d’une arborescence est moindre pour ces documents que pour des ensembles d’archives, et la sémantique EAD n’est pas aussi développée que celle de la TEI-P5, utilisée pour les manuscrits médiévaux dans plusieurs pays d’Europe."

---
"Au-delà des manuscrits et archives, **l’EAD est pertinente pour tout ensemble de documents hiérarchisés, quelle que soit leur nature. Elle permet de visualiser aisément la structure de fonds ou de collections composites** comme celles du Département des Arts du Spectacle de la BnF, qui comprennent fréquemment scénarios manuscrits, programmes imprimés, costumes, objets de décor, etc."

---

## TEI

* 1999-2001 : projet européen MASTER (Manuscript Access through Standards for Electronic Records);
* 2001, la DTD Master, personnalisation de la TEI qui complète par l'ajout d'un élément msDesccription, et d'autres éléments spécialisés qui représentent un enrichissement des possibilités pour la description des manuscrits.
* 2007-2009 : lancement du projet ENRICH (European Networking Resources and Information concerning Cultural Heritage)

---
 
### Les éléments TEI de description des sources : `<msDesc>`

[Voir le fichier TEI](exSourceDesc.xml)

Pour aller plus loin : [**10 Manuscript Description**](http://www.tei-c.org/release/doc/tei-p5-doc/fr/html/MS.html)

---

### Mise en pratique

À l'aide des informations que vous trouverez sur la notice de Gallica, compléter les informations sur le manuscrit qui contient la séquence de sainte Eulalie dans le fichier TEI en utilisant le `<msDesc>`. 



