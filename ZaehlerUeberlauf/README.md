# Zählerüberlauf
Das Modul stellt überlaufende Zähler als kontinuierliche Zähler dar.

### Inhaltsverzeichnis

1. [Funktionsumfang](#1-funktionsumfang)
2. [Voraussetzungen](#2-voraussetzungen)
3. [Software-Installation](#3-software-installation)
4. [Einrichten der Instanzen in IP-Symcon](#4-einrichten-der-instanzen-in-ip-symcon)
5. [Statusvariablen und Profile](#5-statusvariablen-und-profile)
6. [WebFront](#6-webfront)
7. [PHP-Befehlsreferenz](#7-php-befehlsreferenz)

### 1. Funktionsumfang

* Berechnet den Gesamtwert einer Variable und zählt diese hoch, obwohl das Gerät einen Überlauf hat.

### 2. Voraussetzungen

- IP-Symcon ab Version 4.2

### 3. Software-Installation

* Über den Module Store das Modul Zähler-Überlauf installieren.
* Alternativ über das Module Control folgende URL hinzufügen:
`https://github.com/symcon/ZaehlerUeberlauf`

### 4. Einrichten der Instanzen in IP-Symcon

- Unter "Instanz hinzufügen" kann das 'Zählerüberlauf'-Modul mithilfe des Schnellfilters gefunden werden.
    - Weitere Informationen zum Hinzufügen von Instanzen in der [Dokumentation der Instanzen](https://www.symcon.de/service/dokumentation/konzepte/instanzen/#Instanz_hinzufügen)

__Konfigurationsseite__:

Name        | Beschreibung
----------- | ---------------------------------
Quelle      | Quellvariable, welche für die Berechnung genutzt werden soll.
Maximalwert | Ab welchem Wert ein Überlauf stattfindet. Der maximale Wert, welcher das Gerät zählt.

### 5. Statusvariablen und Profile

Die Statusvariablen/Kategorien werden automatisch angelegt. Das Löschen einzelner kann zu Fehlfunktionen führen.

##### Statusvariablen

Name    | Typ   | Beschreibung
------- | ----- | ----------------
Zähler  | Float | Fortlaufend hochzählender Wert.

##### Profile:

Es werden keine zusätzlichen Profile hinzugefügt.

### 6. WebFront

Über das WebFront wird die Variable angezeigt. Es ist keine weitere Steuerung oder gesonderte Darstellung integriert.

### 7. PHP-Befehlsreferenz

Es sind keine besonderen Funktionen vorhanden.