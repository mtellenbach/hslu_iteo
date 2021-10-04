# ITEO (IT-Systemengineering & -Operations)
Dieses Repository dient als Zusammenfassung zum Modul ITEO an der Hochschule Luzern 
gemäss den zur Verfügung gestellten Unterlagen und Folien des Moduls.

Als Versionisierung dient die Commit-History des [GitHub-Repositories](https://github.com/mtellenbach/hslu_iteo).

## Das ITEO-Haus
### 1. Fundament
- CNA
- Knowhow
- Normen (IEEE)
- Gesetze
### 2. Rechenzentrum
Das Rechenzentrum setzt sich aus verschiedenen Komponenten zusammen (siehe Das Datacenter -> Building Blocks).
### 3. Virtualisierung
### 4. Störungen & Ausbau
### 5. Monitoring
### 6. ITIL
### 7. Betrieb der IT-Infrastruktur
### 8. Cloud
### 9. Management

## Das Datacenter
### Building Blocks
Die Building Blocks beschreiben die physikalen Bestandteile eines Rechenzentrums (Datacenter). Folgende wichtigen Blocks werden hierbei besonders berücksichtigt:
- Gebäude
- Zutrittskontrolle
- Klimatisierung (Kühlung)
- Brand- und Hochwasserschutz
- Serverracks mit Rechnern
- Stromversorgung (Motor & unterbrechungsfreie Stromversorgung USV)
- Datenleitungen / Netzwerk
- Administration und Überwachung

### Klimatisierung
Die Klimatisierung sorgt für optimale klimatische Bedingungen im Rechenzentrum mittels Abfuhr von Luft.
Als optimale Bedingungen werden ca. 26 Grad Celsius empfohlen. Zudem sorgt die Klimatisierung anhand von Partikelfiltern für reine Luft, um Verschmutzungen von Aussen vorzubeugen. Ablagerungen auf den Platinen können zu verstopften Lüfter, Störungen oder im schlimmsten Fall zu Kurzschlüsse und Ausfälle führen.

Folgende Probleme müssen im Allgemeinen von der Klimatisierung bewältigt werden:
- Kondenswasser
- Filterkontrolle (Druck vorher - nachher)
- Brauch zusätzlich Energie
- Luftverteilung (siehe Kühlluftverteilung)
- Überwachung

Die Kühlleistung wird in BTU pro Stunde angegeben, wobei 1000 BTU/h ungefähr 293 W entspricht. (BTU = British Thermal Unit)

#### Wieso wird ein Rechner warm?
Verantwortlich für (Ab-)Wärme eines Rechners ist der Stromwiderstand.

#### Kühlluftverteilung
Free-Flow-Systeme (Freie Luftzirkulation):
Vorteile:
- Einfacher Aufbau
- Keine zusätzlichen Hindernisse

Nachteile:
- Kalt-/Warmuftvermischung
- Unterschiedliche Temperaturen

Kalt- oder Warmgang-Einhausung:

Vorteile:

- Energieoptimiert durch Trennung von Kalt- und Warmluft
- Geringere Energiekoster
- Keine vertikale Temperaturdifferenzen

Nachteile:

- Zusätzliche Kosten im Aufbau (Trennung durch Wände und Türen)
- Erhöhter Abschottungsbedarf (siehe Trennung)

#### Novec Immersion Cooling
Siehe https://www.youtube.com/watch?v=a6ErbZtpL88

### EDV-Einbau
Standardisierte/Genormte Masse für den EDV-Einbau in Datacenter.

#### Serverracks
- Höhe 21-49U / Tiefe 0.8-1.2m / Breite 0.6-1m
- Integrierte Kühlung möglich
- Zuleitungen oben / unten / seitlich
- 19" als Standard (48.26 cm)
- 1HE = 1U = 1.75" = 44.45mm

#### Netzwerk
Mit Kupfer- oder Glasfaserkabel

#### Stromverteilung (Trasse oben/unten)
Kabelführung via Hohlboden (Doppelboden) oder Deckentrasse

#### Klimageräte, USV, Batterieschränke

### Kritische Punkte
#### Bauliche Massnahmen
- Einbruch
- Diebstahl
- Vandalismus
- Sturmschäden
- Trümmer

#### Fremdzugriff
- Zutrittskontrolle
- Abhörsicherheit
- Firewall
- usw...

#### Brandschutz
- Brandfrüherkennung
- Löschung (CO2-Gas)
- Abschottung

Problem: Brandgasverteilung durch Klimaanlage (Salzsäure)

#### Netzausfälle und -störungen
- Netzfilter
- USV mit Batterien
- Generatoren
- EMP-Abschirmung

#### Staub / Schmutz / Wasser
- Filteranlagen
- Schleusen
- Standortwahl
- Abschottung
- Pumpanlagen
- usw...

### Überwachungsgebiete
#### Gebäude
- Türen offen - zu
- Türen verschlossen
- Kameras
- Bewegungsmelder
- Zutritte

#### Räume
- Temperatur
- Luftfeuchtigkeit
- Bewegung
- Rauch
- Brand
- Leckage
- Wasser

#### Energieversorgung
- Netzausfall
- Strom
- Spannung
- Leistung (kW)
- Leistungsfaktor (cos phi)

#### Einzelne Geräte
- Niederspannungsverteilungen
- Schalterstellungen 0/1
- Stromverbrauch einzelner Bereiche
- Sicherungsausfall
- Kurzschluss
- Überlast
- usw...

#### Generator
- Kraftstoff
- Funktionsbereitschaft
- Temperatur
- Überlast

#### Klimageräte
- Temperaturen
- Luftfeuchtgkeit
- Übertemperatur
- Filterwiderstand
- Störungen

#### USV-Anlagen
- Normalbetrieb
- Batteriebetrieb
- Bypass-Betrieb
- Ladezustand
- Batterietemperatur

#### Brandmelde- und Löschanlage
- Zustandsanzeigen wie z.B. Löschanlage
- Übertragungseinrichtung ausgeschaltet
- Störung
- Service

### RZ Effizienz (PUE Faktor)
PUE-Wert = Power Usage Effectiveness

PUE = (Gesamte im RZ verbrauchte Energie) / (Verbrauch der IT-Geräte)

Der PUE-Wert ist der Massstab für die Effizienz eines Rechenzentrums und wird im Umfeld von "Green IT"
immer wieder benutzt.

Optimaler Energieaufwand bei PUE = 1

Guter Energieaufwand bei PUE = 1.2

Optimierungsbedarf bei PUE > 1.4


### Verfügbarkeitsverbesserungen
Die Verfügbarkeit wird immer in Prozent angegeben. Relevant ist die Verfügbarkeit in Verbindung mit einem Zeitfenster.
`7 * 24 hat einen höheren Wert als 5 * 9 bei einer Verfügbarkeit von 99%.`

Folgende (Kosten-)Faktoren betreffen einen Ausfall eines Services:
- Umsatzverlust
- Wiederherstellungszeit/-kosten
- Produktivitätsverlust
- Immaterielle Verluste (Ansehen, Kundenzufriedenheit)

#### Failover Cluster
Ausgangslage: Aktiver Server und passiver Server

Der passive (slave) Server dient als Fallback für den aktiven (master). Falls von einem Client aus über eine virtuelle IP-Adresse
nicht mehr auf die IP des aktiven Servers zugreifen kann, schaltet der virtuelle Host auf den passiven um.

Die Kommunikation findet dabei nur zwischen den Server zu dem virtuellen Host statt, sodass der Client
nichts mitbekommt.

#### Failover Datacenter
Für ein aktives Rechenzentrum (production) wird ein identisches, passives Rechenzentrum (Development, Failover Production)
bereitgestellt. Das passive Rechenzentrum repliziert sich dabei laufend mit dem aktiven Rechenzentrum.

Die Synchronisierung findet in einzelnen Teilen kombiniert synchron oder asynchron statt. 
Dies je nach relevanz der Daten.

Synchron:
- Fibre-Channel
- 10G Ethernet

Asynchron:
- Internet (TCP/IP)

#### Availability Environment Classification
Die Harvard Research Group (HRG) teile Hochverfügbarkeit in ihrer Availability Environment Classification
in sechs Klassen ein:
- **AEC-0** *Conventional*: Funktion kann unterbrochen werden, Datenintegrität nicht essentiell
- **AEC-1** *Highly Reliable*: Funktion kann unterbrochen werden, Datenintegrität muss gewährleistet werden
- **AEC-2** *High Availability*: Funktion darf nur innerhalb festgelegten Zeiten oder zur Hauptbetriebszeit minimal unterbrochen werden
- **AEC-3** *Fault Resilient*: Funktion muss innerhalb festgelegter Zeiten oder während der Hauptbetriebszeit ununterbrochen aufrechterhalten werden
- **AEC-4** *Fault Tolerant*: Funktion muss ununterbrocken aufrechterhalten werden, 24/7-Betrieb muss gewährleistet sein
- **AEC-5** *Disaster Tolerant*: Funktion muss unter allen Umständen verfügbar sein

#### Repetitionsfragen
- **Welche Verfügbarkeit muss im SLA festgehalten werden, wenn ich
  1h Ausfallzeit während den Bürozeiten nicht überschreiten will?**
99.9574% = (1 - (1/(5 * 9 * 261))) * 100
- **Was versteht man unter Failover-Cluster-Services?**
Ein System übernimmt als Fallback unterbruchfrei die Funktionen eines anderen Systems, falls dieses ausfällt.
- **Wenn z.B. das SAN gespiegelt werden soll, wie erhöhen sich die
  Kosten?
  50% / 100% / mehr als 100% und warum?**
Mehr als 100% => Da zusätzlicher Server, Disks, Kabel, Failover, komplizierter Netzaufbau, Wartung, Lizenzen usw...

### Tier Levels im Datcenter
N = Anzahl Server
N + 1 = Für N Server stehen N + 1 Server zur Verfügung

1. Redundanz: N, \
jährl. Ausfallzeit: 28.8h \
99.67% Verfügbarkeit

2. Redundanz: N+1, \
jährl. Ausfallzeit: 22h, \
99.75% Verfügbarkeit

3. Redundanz: N+1,
jährl. Ausfallzeit: 1.6h, \
99.98% Verfügbarkeit -> gegenüber Tier 2 zusätzliche Systeme (Failover-Cluster usw.)

4. Redundanz: 2 * (N+1), (2 * Tier 3 parallel geschaltet) \
jährl. Ausfallzeit: 0.8h, \
99.99% Verfügbarkeit

### Information Lifecycle Management (ILM)
Beschreibt die Speicherstrategie eines Rechenzentrums.

#### Anforderungen
- Storage Management
- Document Lifecycle Management
- Content Life Cycle Management
- Records Management \
Einträge von Datenbanken/Excel - was speichere ich wo ab? Anordnung GL und Rechtsabteilung, Durchsetzung Abteilungsleiter

#### Regeln
Kriterien, nach welchen die Daten gespeichert werden:
- Änderungshäufigkeit
- Zugriffsgeschwindigkeit
- Zugriffshäufigkeit
- Kosten
- Ökonomischer Wert
- Relevante gesetzliche Bestimmungen

Danach werden die Daten auf die angemessenen Speichermedien verschoben und am Ende des Lifecycles gelöscht.

#### Active vs. Inactive Data
Ungefähr 40% des Speicherplatzes werden mit Daten befüllt, welche nicht aktiv benötigt werden. Diese Daten
werden trotzdem wie aktive Daten behandelt.

### Tiered Storage
Klassifiziert nach Zugriffsgeschwindigkeit von schnell (fast) bis archiviert (archived).
«Verschiedene Datenklassen gespeichert auf verschiedenen Speicherklassen»

1. Mission Critical Data (Beispiel: Datenbank einer Bank)
2. Business Critical Data (Beispiel: Tägliche Benutzung)
3. Nearline or Historical Data (Beispiel: Archiv)
4. Offline Data (Beispiel: Ausgelagerte Festplatten ohne Strom)

#### Tier-1
- Höchster Speed
- Sehr zuverlässig
- Hohe Skalierbarkeit
- Sehr teuer

#### Tier-2
- Mittlerer Speed
- Zuverlässigkeit OK
- Skalierung limitiert
- Weniger teuer

#### Tier-n
- Hohe Kapazität
- Niedrigerer Speed
- Sehr kleine Kosten pro TB

#### spezialisiert
- Offsite Tape Archivierung
- Einmal beschreibbar (WORM -> Write once read many times)
- Dist-to-Disk backup

## Netzwerke im Rechenzentrum
### Topologie
#### Provider
Vielfalt der Provider ist nicht gut zu überblicken. Liste unter [https://www.providerliste.ch/](https://www.providerliste.ch/).
Je nach Anforderungen werden folgende Kriterien berücksichtigt:
- Global, regional, lokal
- Gemischte und Bundle-Angebot
- Vertrauen
- Geschichte
- Reputation
- Verträge
- Support
- Verfügbarkeiten
- NW-Management
- usw...

##### Technologien
- Kupferkabel: 
  - ADSL mit 2 - ca. 16 Mbit/s
  - VDSL mit 20 - ca. 300 Mbit/s
  - SDSL mit 2 - 200 Mbit/s
- Antennenkabel:
  - Paralles zum TV-Signal, 2 - 500 Mbit/s
- Glasfaser:
  - Mit 10 Mbit/s - 10 Gbit/s
- Richtfunk:
  - Abgelegene, unerschlossene Gebiete
  - 1 - 200 Mbit/s (je nach Distanz)
  
Der Knotenpunkt mit der tiefsten Durchlaufsrate bestimmt die gesamte Übertragungsrate.
Der Provider kann mir keine minimale Übertragungsrate garantieren.

#### Grenze

##### Router
Der Router wird oft in Firewall oder in Layer3-Switches integriert.

Arbeitet mit IP-Paketen und umsetzt diese vom öffentlichen in private Adressen und verbindet deshalb verschiedene Netze aneinander.

Sorgt für optimale Weiterleitungen bei redundanten Leitungen oder Fallback-Szenarien.

Erhält QOS durch spezifische Weiterleitungen auf, kann auch VPN-Endpoint sein (Kerberos, Radius).

Passt sich an unterschiedliche Netzwerktechniken an (Ethernet, xDSL, PPPoE, ISDN, ATM, FDDI).

##### Firewall
Dient als Sicherheitsbaustein im Netzwerk und übernimmt meist auch Routing-Funktionen.
Konfigurierbar durch Regeln, welche die Weiterleitungen von unerwünschten Netzwerkpaketen sperrt.
VPN-Endpunkt mit Authentifizierung (lokal, Radius, AD).

Die Firewall kann auf allen OSI-Schichten arbeiten, also auch als Software auf einem einzelnen Client oder auch als physisches Gerät am Physical Layer.

##### IDP (Intrusion Detection Prevention)
Fasst sich zusammen aus Intrusion Detection Systeme (IDS => Erkennung) und Intrusion Prevention Systeme (IPS => Vorbeugung) \
IDS + IPS = IDP

Detection: Eindringungsversuche erkennen (Mustererkennung, DOS, Fakes, Portscan, IP-Spoofing, usw.) \
Rechenintensive Funktion, oft separates Device

#### DMZ (Demilitarized Zone)
Die DMZ ist ein geschützter Bereich innerhalb eines Netzwerkes, worin bestimmte Zugriffe erlaubt werden
(WWW, Mail, FTP, usw.).

Die DMZ hängt typischerweise an der Firewall an einem separaten Port und ist nur durch eine Authentifizierung
an der Firewall erreichbar.

Zur erhöhten Sicherheit konfiguriert man im DMZ Model 2 entsprechend die DMZ zwischen zwei separaten (ungleichen)
Firewalls. Aus dem WWW kommen Pakete durch die erste Firewall in die DMZ und dann über die zweite Firewall
ins innere Netzwerk. Dies ergibt eine doppelte Authentifizierung.

#### Netzwerk / Redundanz
- 1 Provider / 2 Zugängen oder ...
- ... 2 Provider / je 1 Zugang
- Ausfallüberwachung nötig (Router verbunden)
- Getrennte Wege/Trasse (2 Hauseinführungen)
- Ev. Verschiedene Medien (Glasfaser, Kabelanschluss, Laserlink, Satellit)
- Loadbalancing (Beide Verbindungen gleichzeitig benutzbar)

#### Lokales Netzwerk (LAN)
##### LAN-Strukturen
- TOR (Top Of Rack): Jedes Rack hat eigene Switches
- EOR (End Of Row): Racks nur über Patchpanels verbunden -> Switches in separaten Racks

##### Einfaches Layout
- Peering / Peripherie:
  - Anschluss nach aussen
  - Zentrale Knoten
  - Firewalls
  - Router
- Backbone / Spine / Core
  - Rückgrat
  - zentrales Netz
  - Verbindungen innerhalb des Rechenzentrums
- Leaf / Access
  - Anschlüsse für Server
  - Anschlüsse für Peripherie
  - Abgänge auf Gebäude-LAN

##### Grössere Strukturen
- Peering
  - Externe Verbindungen
  - VPN Endpunkte
  - ISP
- Core
  - Zentrale Verbindungen
  - Auch Rechenzentrum zu Rechenzentrum
- Aggregation Layer/s
  - Direkte Verbindungen von Serverfarmen
  - Verbindungen innerhalb der Rackreihen
- Access- / Leaf-Switches
  - Zugangspunkt für physikalische Server und Komponenten

##### Services
**MPLS** (Multiprotocol Label Switching)
VPN-ähnliche Strukturen zur Verbindung von zusammengehörigen Netzen ohne Rücksicht
auf IP-Segmente. Ein Paket bekommt dabei vom Provider ein eindeutiges Label.

##### Produkte
- Core Switches von CISCO
- Huawei Core Switches mit bis zu 100 GE

##### Technikbegriffe
**VLAN**:
- Virtual LAN
- Getrennte Netze auf gemeinsamer Hardware
- Tagged oder Untagged
- Trunks:
  - Verbindet Switches untereinander
  - Mehrere VLANs dürfen **durch den Trunk** mit dem gleichen VLAN auf anderer Switch kommunizieren
- Access Port

**DNS** (Domain Name System/Service):
Zuordnung von IP-Adressen zu DNS-Name (Fully-Qualified Domain Name)

Domainname wird rekursiv aufgelöst (DNS-Server zu DNS-Server).
Z.B. Anfrage auf "de.wikipedia.org": \
.org -> .wikipedia -> .de

**IPAM** (IP Address Management):
MS Service oder separate Verwaltungstools

**DHCP** (Dynamic Host Configuration Protocol):
Dynamische oder reservierte Zuweisung von IP-Adressen und weitere Eigenschaften an
einen TCP/IP-Client

**NAP** (Network Access Protection) oder
**NAC** (Network Access Control):
Qualifiziert den Client anhand von verschiedenen Parametern (User, OS, Version, Antivirus, usw...)

Zuordnung zu den erlaubten Netzwerken oder nur zur Quarantäne Zone.

### Management
#### Netzwerkmanagement
- Verwaltung, Betriebstechnik und Überwachung von IT-Netzwerken und Telekommunikationsnetzen
- OAM(&P): Operation, Administration, Maintenance (& Provisioning)
- ISO: FCAPS Fault/Config/Accounting/Performance/Security Management

#### Systemmanagement
Monitoring aller Betriebsparameter und der Konfiguration nach ITIL

#### Management Netzwerk
Getrenntes LAN, welches nur für das Management benutzt wird und beschränkt zugreifbar
ist. Kann deshalb oft nur via Jump-Host mit Logging erreicht werden.

### Kosten
Annahme 1000 Server

- **51%** Servers
- **11%** Networking Equipment (z.B: Patchkabel)
- **19%** Power Distribution & Cooling (z.B. Klimageräte und Lüftung)
- **15%** Power (Strom/Energie)
- **4%** Other Infrastructure (z.B. Überwachung)

