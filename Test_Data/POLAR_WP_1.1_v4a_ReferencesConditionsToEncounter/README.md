# Allgemein

Es sind 165 neue Patienten mit den gleichen Patientendaten, aus denen der Datensatz `POLAR_WP_1.1_v2` generiert wurde, nur dass zusätzlich jede Condition eine Referenz zum Encounter hat. Da der Encounter selbst auch eine Referenz auf die Condition hat, gibt es hier eine Kreisreferenz, deren Upload einige FHIR-Server ablehnen (z.B. Vonk).

# POLAR_WP_1.1_v4a_ReferencesConditionsToEncounter

=

	Condition                         :  330
	Consent                           :  100
	Encounter                         :  330
	Medication                        :   10
	MedicationAdministration          :  165
	Patient                           :  165
	----------------------------------------
	total                             : 1100