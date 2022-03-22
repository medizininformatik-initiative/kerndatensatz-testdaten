# Achtung

DIESE DATEN SIND NICHT KDS-KONFORM. DER VALIDATOR WÜRDE SIE ABLEHNEN.

Sie werden aber zum Testen gebraucht, da einige DIZ-FHIR-Server anscheinend mit solchen unvalidierten Daten bespielt wurden.

# Allgemein

Es sind 165 neue Patienten mit den gleichen Patientendaten, aus denen der Datensatz `POLAR_WP_1.1_v2` generiert wurde, nur dass hier jede Condition eine Referenz zum Encounter hat, aber der Encounter keine Referenz auf die Condition. Die letzte der beiden Referenzen müsste aber auf jeden Fall vorhanden sein, um KDS-konform zu sein.

# POLAR_WP_1.1_v4b_ReferencesOnlyConditionsToEncounter

=

	Condition                         :  330
	Consent                           :  100
	Encounter                         :  330
	Medication                        :   10
	MedicationAdministration          :  165
	Patient                           :  165
	----------------------------------------
	total                             : 1100
	