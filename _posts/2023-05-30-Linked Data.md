---
title: "Linked Data"
date: 2023-05-30
---

Die heutige Lerneinheit handelte von Linked Data. Doch zuerst ging es im Wesentlichen um eine Übung mit ChatGPT. Wir sollten in Gruppen Fragen zusammentragen und diese dann an ChatGPT stellen. Danach wurden die
wichtigsten Erkenntnisse, welche daraus gewonnen wurden, im gemeinsamen Dokument zusammengetragen.
Danach ging es um Bibframe, Records in Context und schliesslich um das Anreichern von Metadaten mit OpenRefine und Wikidata. In diesem Beitrag möchte ich gerne genauer auf Bibframe und OpenRefine/Wikidata eingehen.


# Bibframe
---

Laut der Deutschen Nationalbibliothek ist Bibframe die "Bibliographic Framework Initiative". Das Ziel war, die bis anhin gängigen Datenaustauschformate wie MARC21 abzulösen. Dabei war wichtig, dass das neue
Format auf die Veränderungen durch das Semantic-Web und Linked-Data reagieren kann. Bibframe wurde 2011 von der Library of Congress ins Leben gerufen. 
Die DNB (Deutsche Nationalbibliothek) ist Mitglied der "Early Implementers Group". Ihr Ziel war in erster Linie die Mitwirkung an den Bibframe Point Papers.

**Bibframe-Modell**

Katalogisiert eine Bibliothekarin oder ein Bibliothekar ein Medium, in unserem Fall nun ein Buch, dann entsteht ein Datensatz mit einigen Informationen darin. Dazu gehören der/die AutorIn, der Titel des Werks, die Signatur, 
etc. Bibframe spaltet dieses Informationen in drei Teile auf, welche auf dem untenstehenden Modell zu finden sind:


![Bibframe-Modell](https://github.com/tanyaZoller/Lerntagebuch-BAIN/blob/master/_img/Bibframe_Modell.jpg?raw=true)


Um die drei Stufen etwas besser erklären zu können nehmen wir als Beispiel das Werk Harry Potter.

**Work**
Work bezeichnet die oberste Ebene. Auf Deutsch wird diese Stufe auch "Werk" genannt. Diese Ebene bildet den Kern der zu katalogisierenden Ressource ab. Dazu gehören zum Beispiel der Autor, die Sprache oder das Thema.
Das heisst, hier würde die Autorin von Harry Potter ihren Platz finden (J.K. Rowling) und die Sprache, in der das Werk erschienen ist.

**Instance**
Die nächste Stufe ist die Instanz des Werkes. Ein Werk kann in verschiedenen Formen erschienen sein. Harry Potter gibt es zum Beispiel als Buch, als Film, als Hörbuch und wenn man Hogwarts Legacy dazuzählt auch als Game.
Auf dieser Stufe werden Informationen wie Verlag, Ort, Erscheinungsjahr und eben auch das Format aufgenommen.

**Item**
Nun wird es konkret. Auf der Stufe "Exemplar" wird das tatsächliche Werk erfasst. Hier kommen Informationen einer Bibliothek rein. Zum Beispiel den Standort (Kinder- oder Jugendabteilung - Belletristik), die Signatur
(PZB III* ROWL(b)) und den Strichcode, der das Buch von den Bibliotheksmitarbeitenden erhält. 

(Quelle Abschnitt Bibframe: https://www.loc.gov/bibframe/docs/bibframe2-model.html)

# Wikidata
---
<br>
OpenRefine wurde bereits in einem eigenen Artikel behandelt. Aus diesem Grund gehe ich hier eigentlich nur noch auf Wikidata und, wenn der Platz reicht, auf Alma ein.
Wikidata ist eine freie Wissensdatenbank. Diese Datenbank kann laut der Startseite von Wikidata sowohl von Menschen als auch von Maschinen gelesen werden. Dabei dient Wikidata als Speicher für die strukturierten Daten von
Wikipedia, Wiktionary, etc. 
Die Sammlung bei Wikidata besteht mehrheitlich aus Datenobjekten. Dabei erhält jedes Datenobjekt eine eindeutige Identifizierung, eingeleitet durch den Buchstaben Q und eine fortlaufende Nummer. Jedes Datenobjekt erhält
eine Bezeichnung und eine Beschreibung.


![Datenobjekt in Wikidata](https://github.com/tanyaZoller/Lerntagebuch-BAIN/blob/master/_img/Datamodel_in_Wikidata_de.svg.png?raw=true)


Im Unterricht ging es dann darum, wie Daten importiert und bei Wikidata angeschaut werden können. Ich muss aber ehrlicherweise gestehen, dass ich da den Faden verloren habe und diesen Prozess hier nicht wiedergeben kann.
Aufgrund der Bachelor-Thesis und anderen Projekten, die noch abgeschlossen werden müssen, bleibt leider keine Zeit, um dies noch einmal durchzuspielen. 

(Quelle Abschnitt Wikidata: https://www.wikidata.org/wiki/Wikidata:Main_Page)

