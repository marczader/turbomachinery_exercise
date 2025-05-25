# Hausarbeit Strömungsmaschinen (Ziffer: 29121)

## Projektbeschreibung
Im Rahmen der Vorlesung ***Strömungsmaschinen*** an der DHBW Karlsruhe wurde das Betriebsverhalten einer Wasserpumpe analysiert. Hierzu wurden reale Messdaten und das Datenblatt mit unterschiedlichen Kennlinien der verwendeten Pumpe eingesetzt. Ziel war es, die Energieeffizienz der Pumpe zu bewerten und mögliche Energieverluste zu identifizieren.

Die Ergebnisse sollten abschließend in einem Jupyter Notebook dokumentiert und dem Dozent bereitgestellt werden. Zusätzlich soll ein kurzes README verfasst werden, um eine Übersicht zu erhalten

## Vorbereitung

Der Python-Code wurde in englischer Sprache geschrieben und für besseres Verständnis mit deutschen Kommentaren versehen.

Im ersten Abschnitt wird zunächst die CSV-Datei mit den Messdaten des Volumenstroms eingelesen und in einem DataFrame (df_1) gespeichert. Gleichzeitig werden zwei weitere DataFrames (df_2 und df_3) erstellt, die Kennliniendaten für die Pumpenhöhe bzw. Eingangsleistung als Funktion des Volumenstroms enthalten, um diese später für Interpolationen und Berechnungen zu nutzen.

Im zweiten Abschnitt werden physikalischen Konstanten definiert und verschiedene Einheiten angepasst, um diese zu einem späteren Zeitpunkt einzusetzen.

## Aufgabe 1: Berechnung der Input-Energie

Die Eingangsleistung wird mithilfe einer linearen Interpolation aus den zuvor erzeugten Dataframes bestimmt. Anschließend wird die Energie für jedes Messintervall berechnet, indem die Leistung mit der Zeit multipliziert wird. Schließlich werden alle Einzelwerte summiert, um die gesamte Input-Energie zu bestimmen.

## Aufgabe 2: Berechnung des Pumpenwirkungsgrades

Die hydraulische Leistung wird anhand einer Interpolation des Pumpenkopfes berechnet und in Kilowatt umgerechnet. Hierzu wird die hydraulische Energie für jedes Messintervall ermittelt und anschließend summiert. Anschließend wird der Pumpenwirkungsgrad berechnet, indem die hydraulische Gesamtenergie mit der Eingangsenergie verglichen wird.

## Aufgabe 3: Berechnung der ungenutzten Energie

Die ungenutzte Energie wird als Differenz zwischen der Eingangsenergie und der hydraulischen Energie berechnet. Dieser Ergebnis gibt die Energieverluste im System an.

## Ergebnisse

- **Gesamte Input-Energie**

- **Durchschnittlicher Pumpenwirkungsgrad**

- **Verlustleistung**

- **hydraulische Energie**

## Python-Pakete

- ***pandas*** – für Verarbeitung von Daten
- **matplotlib*** – für Erstellung von Diagramme und statistische Visualisierungen
- ***scipy.interpolate*** – für die Interpolation der Pumpenkennlinien

## Dateistruktur

- ***README*** - Erläuterung und Inhalt des Repository
- ***csv-Datei*** - mit Messdaten der Pumpe
- ***Jupyter-Notebook*** - mit Python-Code