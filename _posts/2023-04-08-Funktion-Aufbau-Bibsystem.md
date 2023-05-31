---
title: "Funktion und Aufbau von Bibliothekssystemen 2/2"
date: 2023-04-08
---

An dem Termin, bei dem es um die Funktion und den Aufbau von Bibliothekssystemen gehen sollte, wurde erst einmal über die bereits vorhandenen Lerntagebucheinträge gesprochen.
Danach ging es dann um ChatGPT und wie dieser vielleicht einige Aufgaben beim Datenimport und beim Katalogisieren übernehmen könnte. Da ich mich mit ChatGPT
so absolut noch nicht auseinandergesetzt habe, werde ich in diesem Artikel mal etwas genauer darauf eingehen. Ich werde mich aber mehrheitlich damit auseinandersetzen,
was ChatGPT überhaupt ist.
Was ich hier auch anschauen werde ist die Schnittstelle zu Z39.50. Das Z39.50 ist mir in meienr beruflichen Laufbahn immer wieder vor die Nase geflogen, ich hab
aber nie wirklich genauer hingeschaut, worum es sich dabei handelt. Das möchte ich in diesem Blogbeitrag ändern. Da ich aber nur eine begrenzet Zahl an Zeichen zur Verfügung habe,
heisst das auch, dass ich auf den Unterricht und dessen Inhalt nur wenig bis gar nicht eingehen werde.
<br>

# ChatGPT
---
<br>
Immer wieder habe ich von ChatGPT gehört und in den Nachrichten davon gelesen. Aber wirklich damit auseinander gesetzt habe ich mich noch nicht, da ich dafür irgendwie
auch nie die Zeit fand. Heute soll sich das ändern. Beginnen wir von vorne. 

**Was ist ChatGPT und wie funktioniert es?**
<br>
ChatGPT wurde von OpenAI entwickelt und ist ein sogenannter Chatbot. Dieser soll Fragen beantworten, Aufsätze schreiben aber auch programmieren. Das besondere ist,
dass ChatGPT frei zugänglich ist.
Damit der Chatbot Antworten liefern kann, muss er trainiert werden. Dazu hat OpenAI menschliche KI-Trainer Gespräche geliefert, bei denen sie sowohl den Benutzer aber
auch den KI-Assistenten spielten. Diese erfassten Daten wurden mit den Daten gemischt, welche beim Geschwistermodell InstructGPT erfasst wurden. 
In einem weiteren Schritt wurden Vergleichsdaten gesammelt, indem Gespräche aufgenommen wurden, die zwischen dem KI-Trainer und einem Chatbot stattfanden. Diese Schritte
wurden immer wieder wiederholt und so der Chatbot verfeinert (Quelle: https://openai.com/blog/chatgpt).

![ChatGPT](https://raw.githubusercontent.com/tanyaZoller/Lerntagebuch-BAIN/a5f9c19418d12879dbb479d16858abea5ea8823e/_img/ChatGPT_Diagram.svg)

**Diskussion zu ChatGPT**
<br>
Doch der Chatbot ist nicht bei allen beliebt. Eine Überschrift von der NZZ am 31.3.23 lautet: "Italiens Datenschutzbehörde verbietet Chat-GPT". In dem Artikel heisst
es nicht nur, dass ChatGPT verboten sei, es seien sogar schon Ermittlungen eingeleitet worden (Quelle: https://www.nzz.ch/technologie/italiens-datenschutzbehoerde-sperrt-chat-gpt-ld.1732782).
Ein weiteres Diskussionsthema stellen die Schulen dar. Werden dort die Hausarbeiten zukünftig von künstlicher Intelligenz geschrieben? Wie gehen die Schulen, auch 
die FHGR damit um? Ich würde sagen: es bleibt spannend. Und ich werde mich sicher noch vertiefter damit auseinandersetzen.

<br>
# Netzwerkprotokoll Z39.50
---
<br>
Die Informationen zu Z30.50 habe ich aus Wikipedia. Das ist vielleicht nicht die beste Quelle, aber ich habe so irgendwie gar nicht viel anderes gefunden, das ich 
hier nennen könnte.
Also: Z39.50 kommt im Bibliothekswesen zum Einsatz und ist ein Netzwerkprotokoll, welches Sitzungen zwischen Z39.50 Clients und -Servern generiert. Dadurch können Abfragen
stattfinden. Z39.50 kommt aber auch bei Literaturverwaltungsprogrammen wie EndNote und so wie ich gelesen habe auch Citavi zum Einsatz. 
Die Library of Congress hat das Z39.50 verwaltet das Protokoll. Entwickelt wurde es 1984 in den USA durch die National Information Standards Organization. 1990 hat
dann quasi die Library of Congress die Aufgabe der Weiterentwicklung übernommen (Quelle: https://de.wikipedia.org/wiki/Z39.50).
So wie ich das auch im Unterricht verstanden habe, wird das Z39.50-Protokoll langsam durch die SRU-Server abgelöst.
SRU bedeutet Search/Retrieve via URL. 2004 wurde die Version 1.1 released. Heute ist die Version 2.0 vorhanden (Quelle: https://www.loc.gov/standards/sru/).
