# Séance 2 : Introduction à XML

Observer un document XML : *L’année 1437 dans la pratique de Pierre Christofle, notaire du Châtelet d’Orléans*, <http://elec.enc.sorbonne.fr/christofle/index.html>

---

## Définition

XML est un format de données pur, très simple et documenté, conçu pour la *description* des documents textuels. XML ne possède pas de jeu de balises prédéfini.

---

## Un standard international

Depuis 1998, XML est un langage libre et documenté. XML est également un **langage standard** respectant les recommandations du **W3C** (World Wide Web Consortium), il facilite :

- la lisibilité, par les machines ou par l’œil humain;
- l’échange de données;
- la migration vers d’autres plates-formes, d’autres logiciels, d’autres formats.

---

## Structure générale du XML

Les données sont incluses dans le document XML sous forme de chaînes de caractères délimitées par un balisage les décrivant. L’unité de base qui comprend données et balisage est appelée élément.

`<nomElement>chaineCaracteres</nomElement>`

Les éléments XML suivent un principe d’arborescence par imbrication.

`<elementParent>`
	`<elementEnfant>chaineCaracteres</elementEnfant>`
`</elementParent>`

Les éléments *enfants* héritent des propriétés des éléments *parents*

On peut ajouter une propriété à un élément grâce à un attribut.
`<nomElement nomAttribut=’chaineCaracteres’>`
`chaineCaractere`
`</nomElement>`

---

## Un peu d'Histoire...

- SGML (1970), Standard Generalized Markup Language;
	- HTML, HyperText Markup Language: affiche des données notamment sur le Web ;
	- XML, eXtensible Markup Language: contient et structure des données textuelles.

---

## Les éléments XML


### Les éléments
`<element>texte</element>` ou `<elementVide/>`

Les éléments doivent tous strictement respecter le principe d'imbrication

### Les attributs
`<MiseEnValeur rendu=" rouge italique" position=" centrePage">texte</MiseEnValeur>`

---

**Quelques règles importantes :**
	
	- À chaque balise de début doit correspondre une fin de balise ;
	- Les éléments sont imbriqués;
	- Les éléments ne doivent pas se recouvrir ;
	- Il ne doit y avoir qu’un seul élément racine ;
	- Un élément ne doit pas avoir deux attributs avec le même nom.

Un encodage qui respecte ces grands principes du XML est dit __bien formé__.

---
### Les commentaires
`<!-- texteCommentaire -->`

### Les entités
`&entité;`

Les entités sont des appels pour insérer dans le XML des caractères interdits ou bien des séquences de code définies au préalable dans une DTD.

---

### Instructions de traitement et déclaration XML

`<?xml version="1.0" encoding="UTF-8"?>`

Les instructions de traitement sont un autre moyen de fournir des informations aux applications auxquelles est destiné le document. Une instruction de traitement commence par `< ?` et se termine par `?>`.

Ces dernières sont des balises et pas des éléments. Elles doivent donc être en dehors d'une balise.

Les instructions de traitement les plus courantes sont l'appel d'une feuille de style, d'un schéma et l'appel d'une version de XML. Ces appels doivent être placés avant l'élément racine.

---

## Mise en pratique

**Encoder en XML la séquence de sainte Eulalie :** 

https://fr.wikisource.org/wiki/Séquence_de_sainte_Eulalie 

https://patrimoine-numerique.ville-valenciennes.fr/ark:/29755/B_596066101_MS_150/F_141_V?highlight=Mot_cle%3A 
