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

Die USV kann 

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

3. Redundanz: N+1, \
jährl. Ausfallzeit: 1.6h, \
99.98% Verfügbarkeit

4. Redundanz: 2 * (N+1), \
jährl. Ausfallzeit: 0.8h, \
99.99% Verfügbarkeit

### Information Lifecycle Management

### Tiered Storage