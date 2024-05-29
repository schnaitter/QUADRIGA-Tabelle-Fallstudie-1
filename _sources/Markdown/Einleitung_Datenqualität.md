# Einleitung: Datenqualität

**Hier:**\
Einführung Erläuterung: strukturierte Daten, Fokus Datentyp, Struktur ist nicht gleich Struktur


## Grobziel (#- zu bearbeiten)
Nach Absolvierung der QER-Gruppe sind die Lernenden in der Lage, die Datenquellen und die Qualität der Datensätze zu bewerten sowie die Reproduzierbarkeit der Fallstudie zu evaluieren.

## Feinziel (#- zu bearbeiten)
Die Lernenden können die Qualität von Datensätzen bewerten.

*Der Forschende lädt sich den zugehörigen Datensatz zum Bildungsberichts 2022 als xlsx Datei herunter (Link) zu den Datensätzen des Bildungsberichts). Als der Forschende sich die Daten genauer anschaut, stellt er fest, dass es sich um aggregierte Daten handelt. Als Quelle für die Rohdaten wird auf das Statistische Bundesamt (Destatis) verwiesen. Hier findet er die Rohdaten im CVS-Format (Link zu Destatis). Wie offen und technisch verwendbar sind diese Datensätze für seine nachfolgenden Analysen?*

## Tidy Data Struktur

Die Datenqualität spiegelt sich zudem in einer guten Ausgangsstruktur wider. Diese ermöglicht eine einfach und effektiv bearbeiten der Daten. Ein weitverbreiteter Standard für diese Struktur setzt das sogenannte „Tidy Dataset“ (Wickham, 2014). Ein Datensatz wird als „Tidy“ bezeichnet, wenn es folgende Struktur erfüllt:

(1)  Jede Variable ist eine Spalte

(2)  Jede Beobachtung ist eine Zeile

(3)  Jeder einzelne Wert (Datenpunkt) wird
einer Variable und einer Beobachtung zugeordnet.

Durch Einhaltung dieser Struktur entsteht eine Tabelle, die eine schnelle, einfache und vor allem konsistente Datenmanipulation und -auswertung ermöglicht (Wickham, 2014).

Beispiel für Tidy Data:

Name | Alter | Testergebnis
---- | ----- | ------------
Tina | 34    | 61
Tom  | 27    | 52


**Typische Fehler**

Nach Wickham (2014) sind die häufigsten Fehler im Aufbau von Datensätzen folgende:

- Spaltenüberschriften sind keine vernünftigen Variablennamen sondern numerische Werte.

- Mehrere Variablen werden in einer Spalte gespeichert.

- Variablen werden sowohl in Spalten als auch in Zeilen gespeichert.

- Verschiedene Beobachtungseinheiten (z.B. Kilo/Pfund/Unze) werden unter derselben Variable gespeichert.

- Eine einzelne Beobachtungseinheit wird wiederholt in mehreren Datensätzen gespeichert.

Für die Computersprache R wurde in diesem Kontext das "Tidyverse" ([https://www.tidyverse.org](https://www.tidyverse.org)) erschaffen, welches eine Ansammlung von Funktionen enthält, die den Aufbau von und das effiziente Arbeiten mit Tidy Data ermöglichen.