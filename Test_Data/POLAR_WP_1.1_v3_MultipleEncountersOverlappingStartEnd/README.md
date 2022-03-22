# Allgemein

Es sind 70 neue Patienten mit den gleichen Patientendaten, aus denen der Datensatz `POLAR_WP_1.1_v2` generiert wurde. Jeder Patient hat entweder 2 oder 4 Encounter, wobei einer immer ein Einrichtungskontakt ist und ein weiterer Encounter als Part-Of ein Abteilungskontakt. Die beiden zusammengehörigen Encounter haben immer dieselben Start- und Endzeiten.
Die zusätzlichen Encounter sind alle mit einer jeweils einer Diagnose verbunden, die im Polar Workpackage 1.1 nicht relevant sind.

Es gibt jeweils 20 Patienten mit 2 Encounter (
* Encounter Startzeit = Encounter Endzeit
Es gibt jeweils 10 Patienten mit 4 Encountern (je 2 Einrichtungskontakte und 2 Abteilungskontakte) mit:
* Encounter überlappen sich teilweise
* Encounter haben dieselbe Startzeit, aber unterschiedliche Endzeit
* Encounter haben dieselbe Endzeit, aber unterschiedliche Startzeit
* Encounter überlappen sich vollständig (dieselbe Start- und Endzeit)
* ein Encounter enthält den anderen gleichartigen Encounter vollständig 

# POLAR_WP_1.1_v3_MultipleEncountersOverlappingStartEnd

=

    Condition                         : 190
    Encounter                         : 240
    Medication                        :  10
    MedicationAdministration          :  70
    Patient                           :  70
    ---------------------------------------
    total                             : 580
    