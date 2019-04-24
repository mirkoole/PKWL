Public-Key-Web-Login (PKWL)
====

A Method for Password-free Authentication

Ein Verfahren zur passwortlosen Authentifizierung


Introduction
----

This repository contains the bachelor's thesis "A Method for Password-free Authentication" by Mirko Oleszuk (2013).
The source-code for the clients and server is placed in its respective submodule-folder.
The presentation slides are available in english and german.


Zusammenfassung
----

Die vorliegende Arbeit stellt ein Verfahren zur passwortlosen Authentifizierung von Benutzern einer Webanwendung vor.

Die Grundlage für die Authentifizierung bildet das asymmetrische RSA-Kryptosystem. Aufgrund der Eigenschaft der Asymmetrie besteht eine eindeutige Zuordnung zwischen verschlüsselten Daten und dem Schlüsselpaar, mit dem die Daten verschlüsselt wurden. Passwörter lassen sich bei der Authentifizierung in Webanwendungen vermeiden, da eine Webanwendung einen Benutzer anhand seines öffentlichen Schlüssel durch signierte Noncen oder verschlüsselte Cookies authentifizieren kann.

Diese Arbeit zeigt zudem Schwächen der passwortbezogenen Authentifizierung auf und analysiert bereits vorhandene Alternativen auf Ihre Sicherheit und Einsatzfähigkeit.

Die Beschreibung der Entwicklung des Verfahrens wird von Erläuterungen zu einigen Angriffstechniken begleitet und die jeweiligen Designentscheidungen und Weiterentwicklungen dadurch begründet.

Die Implementierung des Verfahrens wird anhand eines Clientplugins für den Browser Chromium und anhand eines Serverplugins für die Blogsoftware Wordpress beschrieben. Es werden die einzelnen Kommunikationsschritte ausführlich dargestellt. Die Plugins wurden generisch geschrieben, sodass eine Portierung auf andere Systeme keinen großen Aufwand bedeutet.

In der Evaluation der Arbeit wird gezeigt, dass die Laufzeit des Verfahrens, mit einem 2048 Bit langen Schlüssel, ca. 13 Sekunden beträgt. Damit ist das Verfahren sicher und zugleich performant.

Somit ist das im Rahmen dieser Arbeit entwickelte Verfahren zur passwortlosen Authentifizierung eine sichere Alternative zur klassischen Authentifizierung via Passwort. Es funktioniert sicher über eine unverschlüsselte Verbindung, sodass es in eingeschränkten Umgebungen eingesetzt werden kann. Der Benutzer benötigt zur Installation keine besonderen Rechte und auch keine andere Software als den Browser und die Webanwendung selbst.
