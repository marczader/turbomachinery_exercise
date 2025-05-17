# Hausarbeit Strömungsmaschinen

## Projektbeschreibung
Im Rahmen der Vorlesung ***Strömungsmaschinen*** an der DHBW Karlsruhe wurde das Betriebsverhalten einer Wasserpumpe analysiert. Hierzu wurden reale Messdaten und das Datenblatt mit unterschiedlichen Kennlininen der verwendeten Pumpe eingesetzt. Ziel war es, die Energieeffizienz der Pumpe zu bewerten und mögliche Energieverluste zu identifizieren.

Die Ergebnisse sollten abschließend in einem Jupyter Notebook dokumentiert und dem Dozent bereitgestellt werden. Zusätzlich soll ein kurzes README verfasst werden, um eine Übersicht zu erhalten

## Vorbereitung

In ersten Abschnitt wird zunächst die CSV-Datei mit den Messdaten des Volumenstroms eingelesen und in einem DataFrame (df_1) gespeichert. Gleichzeitig werden zwei weitere DataFrames (df_2 und df_3) erstellt, die Kennliniendaten für die Pumpenhöhe bzw. Eingangsleistung als Funktion des Volumenstroms enthalten, um diese später für Interpolationen und Berechnungen zu nutzen.

Im zweiten Abschnitt werden physikalischen Konstanten definiert und verschiedene Einheiten angepasst, um diese zu einem späteren Zeitpunkt einzusetzen.

## Aufgabe 1: Berechnung der Input-Energie

Die Eingangsleistung wird mithilfe einer linearen Interpolation aus den vorliegenden Messdaten bestimmt. Anschließend wird die Energie für jedes Messintervall berechnet, indem die Leistung mit der Zeit multipliziert wird. Schließlich werden alle Einzelwerte summiert, um die gesamte Eingangsenergie zu bestimmen.

## Aufgabe 2: Berechnung des Pumpenwirkungsgrades

Die hydraulische Leistung wird anhand einer Interpolation des Pumpenkopfes berechnet und in Kilowatt umgerechnet. Die hydraulische Energie wird für jedes Messintervall ermittelt und anschließend summiert. Der Pumpenwirkungsgrad wird dann berechnet, indem die hydraulische Gesamtenergie mit der Eingangsenergie verglichen wird.

## Aufgabe 3: Berechnung der ungenutzten Energie

Die ungenutzte Energie wird als Differenz zwischen der Eingangsenergie und der hydraulischen Energie berechnet. Dieser Wert gibt die Energieverluste im System an. Abschließend werden die Ergebnisse ausgegeben, um die Effizienzbewertung der Pumpe zu unterstützen.

