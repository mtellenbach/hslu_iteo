# ITEO (IT-Systemengineering & -Operations)
Dieses Repository dient als Zusammenfassung zum Modul ITEO an der Hochschule Luzern.

## Das ITEO-Haus
### 1. Fundament
- CNA
- Knowhow
- Normen (IEEE)
- Gesetze
### 2. Rechenzentrum
Das Rechenzentrum setzt sich aus verschiedenen Komponenten zusammen (siehe Building Blocks).
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

### Staub / Schmutz / Wasser
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
