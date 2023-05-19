---
title: "Metadaten modellieren"
date: 2023-05-09
---
Diese Lerneinheit beschäftigte sich mit der Modellierung von Metadaten sowie dem Nutzen von Schnittstellen.
<br>
Ein paar Dinge von dieser Lerneinheit hatten wir bereits in vorhergegangenen Einheiten. So zum Beispiel die Schnittstellen Z.39.50 und SRU. Ich bin gerade unsicher, ob wir OAI-PMH auch bereits genauer angeschaut
hatten. Aber das würde ich in diesem Blogbeitrag gerne noch tun.
<br>
# OAI-PMH 
---
<br>
OAI-PMH bedeutet Open Archives Initative Protocol for Metadata Harvesting. 
Das Protokoll legt fest, wie Metadaten strukturier und dann für die Aufnahme durch externe Dienste, wie das Internet, dargestellt werden sollen. Kodiert sind die Metadaten im XML-Format, die Datensätze werden über 
HTTP-Anfragen abgerufen. Die Gliederung eines solchen Datensatzes sieht wie folgt aus:
* Header:
  * eindeutige Bezeichner
  * Datum
  * set membership
* Metadaten:
  * Satz von Metadaten
  * oft in Dublin Core
* About:
  * Optionale Angaben zu Rechten, Herkunft und andere Verwendugnszwecke

Für bibliografische Daten von Bibliotheken wird eine besondere Form des OAI-PMH verwendet: das OAI-DC (Dublin Core)-Metadatenschema. Bibliotheken verwenden diesen Typ, um zu Erschliessen aber auch für das Harvesting.
Das Harvesting findet über GET oder POST-Anfragen statt. Jede dieser Anfragen enthält:
* die Basis-URL
* optional die Pfadangabe
* eine Verb-Anweisung
* mehrere optionale Argumente
(Quelle: https://libtechlaunchpad.com/2017/02/13/oai-pmh-basics-and-resources/)

# ETL-Prozesse
---
<br>
In dieser Einheit wurden viele Dinge wie XSLT-Crosswalks, MarcEdit, ETL-Prozesse oder auch die Nutzung von JSON-APIs besprochen. Da die Zeichenzahl in diesen Artikeln jeweils begrenzt ist, konzentriere ich mich jeweils auf
1-2 Punkte, die mich interessieren. Hier möchte ich noch auf die ETL-Prozesse eingehen.
ETL-Prozesse dienen grundlegend der Übertragung von Daten in ein anderes System. Der Prozess besteht aus drei zentralen Schritten:
* Extract
* Transform
* Load

Im folgenden Bild wird der Prozess graphisch dargestellt:
![ETL-Prozesse](https://github.com/tanyaZoller/Lerntagebuch-BAIN/blob/master/_img/etl-prozess.png?raw=true)

Doch was bedeuten diese drei Schritte Extraktion, Transformation und Laden? Hier möchte ich ganz kurz darauf eingehen.

## Extraktion
Das Ziel dieses Schrittes ist die Auswahl und der Abzug von relevanten Daten aus verschiedenen Quellen. Das ist das Harvesting, welches weiter oben schon einmal erwähnt wurde. Der Prozess des Harvesting kann entweder
manuell oder aber automatisiert ausgelöst werden.
Als Datenquellen können Dateien, Datenbanken, Schnittstellen oder Webseiten dienen. 
<br>
## Transformation
Bei diesem Schritt sollen alle Daten in ein einheitliches Format übertragen werden. Beim ETL-Prozess wird das Zielformat als Schema bezeichnet. Die Vereinheitlichung des Schemas wird als Mapping bezeichnet und ist einer
der wesentlichen Schritte jeder Datenkonvertierung. Um den Transformationsaufwand zu reduzieren einigte man sich auf Standards wie MARC21.
Es werden bei der Transformation noch weitere Schritte notwendig, welche hier nicht aufgeführt werden.
<br>
## Laden
Bei diesem Schritt werden die vereinheitlichten Daten in das Zielsystem überführt. Daten, welche den vorherigen Transformationsschritt nicht erfolgreich abgeschlossen haben, dürfen nicht in ein produktives System 
überführt werden. Beim Schritt des Ladens muss jedoch darauf geachtet werden, dass das laufende System nicht ausfällt, während die neuen Daten eingespeist werden. Das würde ja sonst bedeuten, dass Swisscovery jedes mal 
bei der Einspeisung neuer Daten nicht genutzt werden könnte.
(Quelle Abschnitt ETL-Prozesse: https://it-in-bibliotheken.de/metadaten.html#datenverarbeitung)

In vorherigen Modulen war bereits Harvesting, etc. ein Thema. Jedoch war es für mich immer schwer zu verstehen. Dank des ETL-Prozesses und des Handbuches für IT in Bibliotheken habe ich jetzt aber deutlich besser
verstanden, wie diese Schritt ablaufen.


