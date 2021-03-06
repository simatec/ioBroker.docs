﻿---
local:       true
---
![logo](media/tradfri.png)
# Ikea tradfri Adapter

## Tradfri
Tradfri ist ein SmartHome System der Firma Ikea. Zum jetzigen Zeitpunkt umfasst
dieses System verschiedenste Komponenten aus:

- Leuchtmittel(Lampen)
- LED-Panele/Leisten für Wände und Schränke/Schranktüren
- Bewegungsmelder
- Rolläden für Fenster
- Fernbedienung
- zentraler Gateway

Das Tradfri System ist somit eines der umfangreichesten SmartHome Komponentensystem
was es momentan auf dem Markt gibt.

## Voraussetzungen zur Verwendung von Tradfri mit ioBroker

- RaspberryPi 3 Model B+
- Tradfri Gateway
- Tradfri Komponenten (z.b. Leuchtmittel oder Bewegungsmelder etc.)
- Tradfri Fernbedienung


## Verwaltung und Steuerung von Tradfri mit ioBroker
Um Tradfri mit ioBroker optimal zu verwalten und zu steuern
wird folgender Adapter benötigt:

1.  Ikea Tradfri

Dieser Adapter stellt eine Verbindung zum zentralen Tradfri Gateway her
Er synchronisiert Komponenten(Lampen, Bewegungsmelder etc.), Szenen, Systemvariablen 
Tradfri Gateway und ioBroker. Abb. 01 zeigt eine vereinfachte Darstellung der Kommunikation
zwischen ioBroker, Gateway und Komponenten.

![Kommunikationsablauf](media/TradfriOverview_002.PNG)


### Installation des Adapters und Konfiguration der Instanz
<b>Schritt 1.</b>

- Installieren des Adapters durch klicken auf ![Adapter](media/Adapter.PNG) in der linken Navigationsleiste des Webinterface
- in der nun erscheinenden Seite, in der Suche nach "Ikea Tradfri" suchen/filtern (siehe Abb. 01)
- den Adapter über das Icon ![Plus](media/plus.PNG) (letzte Spalte, ganz rechts) installieren. (hierbei wird auto. eine neue Instanz 
  des Adapters unter ![Instanzen](media/instanzen.PNG) angelegt)


![Ikea Tradfri Adapter hinzufügen](media/TradfriAdapterInstanz_002.PNG)

<b>Schritt 2.</b>

- Durch wechseln der Ansicht in der linken Navigationsleiste ![Instanzen](media/instanzen.PNG) werden die aktuell vorhandenen
  Instanzen angezeigt. Nach setzen des Filters auf "Tradfri" werden alle laufenden "Tradfri" Instanzen angezeigt. 
  Dies sollte der unteren Abbildung entsprechen.

![Ikea Tradfri Instanzansicht](media/TradfriAdapterInstanz_003optimiert.PNG)

- In der Spalte der jeweiligen Instanz bestehen folgende Anzeigen/ Aktionsmöglichkeiten Beschrieben von links nach rechts.
  - <b>Anzeige Aktivitätsstatus</b> (einfaches Ampelsystem)
    - ![Status Grün](media/status_green.PNG) ->Instanz läuft innerhalb der zu erwartenden Parameter, alles ok
    - ![Status Gelb](media/status_yellow.PNG) -> Instanz läuft, allerdings gibt es ggf. Probleme mit der Konfiguration des Tradfri Gateway
    - ![Status Rot](media/status_red.PNG) -> Instanz ist zwar gestartet, hat aber Probleme sich mit dem Host zu verbinden. 
  - <b>Aktionen</b>
    - ![Start Instanz](media/starting.PNG)Start und ![Stop Instanz](media/stop.PNG) Stop der Instanz ermöglichen diese Buttons
    - ![Start Instanz](media/konfiguration.PNG) Zugriff auf den Konfigurationsbereich der Instanz
    - ![Start Instanz](media/reload.PNG) Instanz wird neu gestartet 
    - ![Start Instanz](media/delete.PNG) Instanz wird unwiederruflich gelöscht





