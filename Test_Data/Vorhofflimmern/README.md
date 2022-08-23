# Allgemein

Alle einzelnen Datensätze sind aufgeteilt in jeweils (maximal) 1000 Patienten, die jeweils als `json.zip` und `ndjson` verfügbar sind.  
Die `json.zip` und `ndjson` beinhalten jeweils bis zu 1000 Transaktion-Bundles mit jeweils 1 Patienten.
Die gleichnamige Excel-Datei ist die Vorlage zum Generieren JSON-Dateien.

# VHF-Testdaten_01

Ursprüngliche Vorhofflimmern (VHF) Testdaten sind Patienten
* unterschiedlichen Alters (17 bis 83 Jahre, davon 3300
Patienten mit Alter > 65 Jahre)
* mit 1 stationären Versorgunsstellenkontakt vom 01.01.2021 bis zum 02.01.2021
* mit 1 Abteilungskontakte in der Kardiologie ebenfalls vom 01.01.2021 bis zum 02.01.2021
* mit 1 Diagnose 
Vorhofflimmern (I48.0 oder I48.1) (= 104 Patienten) oder
Idiopathische Hypotonie (I95.0) (= 9896 Patienten)
* mit 1 Wert NT-proBNP SerPl-mCnc (LOINC = 33762-6) mit der Einheit pg/mL
* mit willkürlichen Consent-Daten
* aufsteigend nach Alter sortiert (d.h. größere Pat-ID = höheres Alter)

Der Datensatz umfasst folgende Dateien:

VHF-Testdaten_01-VHF00001-VHF01000  
VHF-Testdaten_01-VHF01001-VHF02000  
VHF-Testdaten_01-VHF02001-VHF03000  
VHF-Testdaten_01-VHF03001-VHF04000  
VHF-Testdaten_01-VHF04001-VHF05000  
VHF-Testdaten_01-VHF05001-VHF06000  
VHF-Testdaten_01-VHF06001-VHF07000  
VHF-Testdaten_01-VHF07001-VHF08000  
VHF-Testdaten_01-VHF08001-VHF09000  
VHF-Testdaten_01-VHF09001-VHF10000  

=

    Condition                         : 10000
    Consent                           :  9687
    Encounter                         : 20000
    Observation                       : 10000
    Patient                           : 10000
    -----------------------------------------
    total                             : 59687

# VHF-Testdaten_02-andereDiagnose

1000 neue Patienten wie in VHF-Testdaten_01 aber mit
* einer anderen Diagnose
* ohne Consent.

VHF-Testdaten_02-andereDiagnose-VHF10001-VHF11000

=

    Condition                         : 1000
    Encounter                         : 2000
    Observation                       : 1000
    Patient                           : 1000
    ----------------------------------------
    total                             : 5000

# VHF-Testdaten_03-andererLaborwert

1000 neue Patienten wie in VHF-Testdaten_01 aber mit
* einem anderen Laborwert
* ohne Consent

VHF-Testdaten_03-andererLaborwert-VHF11001-VHF12000

=

    Condition                         : 1000
    Encounter                         : 2000
    Observation                       : 1000
    Patient                           : 1000
    ----------------------------------------
    total                             : 5000

# VHF-Testdaten_04-MixedCases

Testfälle speziell für das Script zum Vorhofflimmern.
Sie sind in a, b, c, und d aufgeteilt, wobei sich die Datensätze
immer nur darin unterscheiden, wie die Encounter die Observations
(Diagnosen) referenzieren und umgekehrt.

* a = Encounter referenziert die Diagnosen, aber die Diagnosen nicht den Encounter
* b = Diagnosen referenzieren den Encounter, aber die Encounter nicht die Diagnosen
* c = Encounter referenziert die Diagnosen und die Diagnosen den Encounter
* d = Weder referenziert der Encounter die Diagnosen noch die Diagnosen den Encounter


* VHF-Testdaten_04-MixedCases_VHF-MIXED-TEST-CASE-0001-a-VHF-MIXED-TEST-CASE-0001-a
* VHF-Testdaten_04-MixedCases_VHF-MIXED-TEST-CASE-0001-a-VHF-MIXED-TEST-CASE-0001-b
* VHF-Testdaten_04-MixedCases_VHF-MIXED-TEST-CASE-0001-a-VHF-MIXED-TEST-CASE-0001-c
* VHF-Testdaten_04-MixedCases_VHF-MIXED-TEST-CASE-0001-a-VHF-MIXED-TEST-CASE-0001-d

=

    Condition                         :  36
    Encounter                         :  56
    Observation                       :  92
    Patient                           :   4
    ---------------------------------------
    total                             : 188

