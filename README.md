# Kerndatensatzkonforme FHIR Testdaten

Autor: [Alexander.Struebing@imise.uni-leipzig.de](mailto:alexander.struebing@imise.uni-leipzig.de)

Dieses Projekt stellt kerndatensatzkonforme FHIR json-Testdaten zur Verfügung.

Ohne Authentifizierung:
- https://mii-agiop-3p.life.uni-leipzig.de/fhir
- https://mii-agiop-3p.life.uni-leipzig.de/blaze

Mit Authentifizierung:
- https://mii-agiop-polar.life.uni-leipzig.de/fhir/
- https://mii-agiop-polar.life.uni-leipzig.de/blaze/

Alle einzelnen Datensätze im Verzeichnis `Test_Data` sind aufgeteilt in jeweils (maximal) 1000 Patienten, die jeweils als `json.zip` und `ndjson` verfügbar sind.  
Die `json.zip` und `ndjson` beinhalten jeweils bis zu 1000 Transaktion-Bundles mit 1 Patienten.
Die gleichnamige Excel-Datei ist jeweils die Vorlage zum Generieren JSON-Bundles.

Im Moment sind alle vorhandenen Daten mit folgenden Datenobjekten und Beziehungen untereinander generiert:
![Schema der Daten](https://github.com/medizininformatik-initiative/kerndatensatz-testdaten/blob/master/FHIR_Data_Resource_Scheme.png)

