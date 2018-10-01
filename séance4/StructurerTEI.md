# Séance 4 : Structurer un fichier TEI


Tout document TEI a au moins deux parties : 

* Un en-tête, représenté au moyen d’un élément **`<teiHeader>`** contenant des métadonnées décrivant le document ;

* le texte lui-même, représenté par un élément **`<text>`**.

---

`<TEI xmlns=’http://www.tei-c.org/​ns/​1.0’>`
     `<teiHeader>`
         `<!-- métadonnées décrivant un texte -->`
    `</teiHeader>`
     `<text>`
         `<!-- une représentation du texte lui-même -->`
     `</text>`
`</TEI>`<br/>

---

Le **teiHeader** minimal comporte les trois sections suivantes :

   * `<titleStmt>` : informations identifiant le document lui-même;
   * `<publicationStmt>` : informations sur la façon dont il est distribué ou publié;
   * `<sourceDesc>` : indications sur ses origines.

---

L’**élément <text>** contient les trois parties suivantes :

   * `<front>` : pour les préfaces et tous les éléments liminaires du texte ; 
   * `<body>` : pour le corps du texte proprement dit;
   * `<back>` : pour tous les appendices, épilogues, postfaces, etc.
---

## Le teiHeader

L’en-tête TEI possède quatre composants principaux :

* `<fileDesc>` : description bibliographique du document, **Attention : il est obligatoire**;
* `<encodingDesc>` : description de l’encodage;
* `<profileDesc>` : description détaillée des aspects non bibliographiques d’un texte, plus précisément les langues et sous-types de langues qu’il utilise, le contexte dans lequel il a été produit, les participants et leur cadre (soit à peu près tout ce qui n’est pas déjà couvert par les autres composants principaux de l’en-tête).
* `<revisionDesc>` : résume l’historique des révisions pour un fichier.

---

## Le fileDesc

Il se compose de trois parties obligatoires :

* `<titleStmt>` : Déclaration du titre;
* `<publicationStmt>` :  Déclaration de la publication;
* `<sourceDesc>` : Description de la source.

---
Exemple :

`<teiHeader>`
     `<fileDesc>`
         `<titleStmt>`
             `<title>Titre de l’œuvre</title>`
         `</titleStmt>`
         `<publicationStmt>`
             `<p>Informations sur la publication de l’œuvre.</p>`
         `</publicationStmt>`
         `<sourceDesc>`
             `<p>`
             `Informations sur la source dont est tirée l’œuvre.`
             `</p>`
         `</sourceDesc>`
     `</fileDesc>`
`</teiHeader>`

---

## Encoder en XML-TEI la préface et l'acte I du Cid de Corneille.

* Récupérer le texte :[le Cid](./leCid.txt).
* Balises à utiliser : `<text>`, `<body>`, `<front>`, `<performance>`(conditions de représentation), `<p>`, `<div>`, `<head>`, `<stage>`(indications de mise en scène), `<roleName>`, `<sp>`(réplique), `<l>`(vers).
* Vous pouvez également vous aider de la documentation suivante : <http://www.tei-c.org/release/doc/tei-p5-doc/fr/html/DR.html>
* Compléter les métadonnées du texte dans le `<TEIheader>`.
---

# Séance 4 : TEIguidelines

L’objectif des **guidelines** est de guider les pratiques d’encodage.

## Les “principes de Poughkeepsie” (1987)

Les recommandations visent à :

  * Fournir un format standard;  
  * Favoriser l’échange de textes dans les humanités;
  * Suggérer des principes abstraits pour l’encodage des textes;
  * Proposer des ensembles de conventions d’encodage adaptés à plusieurs applications différentes;
  * Inclure un ensemble minimal de conventions pour l’encodage de nouveaux textes;
  * Proposer des ensembles de conventions d’encodage adaptés à plusieurs applications différentes.
   
---

## Comment lire les **guidelines** ?

### La page d'accueil : <http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html>

![](./img/guidelines_accueil.png)

---

### [Lire les spécifications](./img/guidelines_msIdentifier.png)

![](./img/guidelines_msIdentifier.png)