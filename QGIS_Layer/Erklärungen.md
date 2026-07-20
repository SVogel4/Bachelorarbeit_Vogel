# QGIS-Layer

Dieser Ordner enthält die verschiedenen QGIS-Layer, die im Rahmen der Erreichbarkeitsanalysen erstellt wurden.

## Unterordner zu den POIs
Die Unterordner der einzelnen Points of Interest (POIs) enthalten sowohl die jeweiligen POIs als Punktlayer als auch die zugehörigen Erreichbarkeitslayer für die verschiedenen Verkehrsmittel. 
Hierzu zählen die Kategorien:
`KiTas_Grundschulen`
`weiterfuehrendeSchule`
`Gesundheitsversorgung`
`Einkaufsmoeglichkeiten`
`Freizeitmoeglichkeiten`

Die Auswahl der POIs basiert auf den Ergebnissen der Befragung der Bewohnerinnen und Bewohner der Ortsgemeinden Schaidt und Vollmersweiler. Die Erreichbarkeiten wurden mithilfe von OpenRouteService (ORS) sowie der im Rahmen dieser Arbeit entwickelten Erreichbarkeitsanalysen ermittelt.

## Erreichbarkeit der Zentroide
Der Ordner zur Erreichbarkeit der Zentroide enthält die ausgewählten Zentroide der vier Teilbereiche des Untersuchungsgebietes sowie die jeweils ermittelten Erreichbarkeiten.
Darüber hinaus wurden für den westlichen Untersuchungsbereich zusätzlich zwei Zentroide innerhalb eines Rasters ausgewählt und deren fußläufige Erreichbarkeit dargestellt.

## Beispiel Analyse
Der Inhalt dieses Ordners veranschaulicht – ergänzend zu den Skripten im Ordner `Erreichbarkeitsanalysen` – die Ergebnisse der Erreichbarkeitsanalyse für jeweils zwei Beispielhaltestellen im Bus- und Regionalbahnverkehr.
Zusätzlich sind die Bus- und Bahnhaltepunkte der beiden Untersuchungsorte kartiert.

## Auswertung
Dieser Ordner enthält bereits Ergebnisse der Analyse und des Vergleichs zwischen subjektiver und objektiver Erreichbarkeit.
Hierbei werden die in der Befragung ermittelten subjektiv wahrgenommenen Erreichbarkeiten den objektiv bestimmten Erreichbarkeiten aus den GIS-Analysen gegenübergestellt.
Unter dem Dateinamen `Teilnehmer_je_Raster.gpkg` ist die Anzahl der Befragungsteilnehmenden je Untersuchungsraster kartiert. 
Die zugrunde liegenden Raster sind zusätzlich unter `Raster_Schaidt_Vollmersweiler` dargestellt. 

Einen konkreten Vergleich der subjektiven und objektiven Erreichbarkeit stellt der Layer `Abweichung_Erreichbarkeit_Prozent`dar. 
Dieser zeigt die prozentualen Abweichungen zwischen den auf Grundlage der ORS-Analysen ermittelten Erreichbarkeiten und den Angaben der Befragten. 
Die dargestellten Werte basieren auf dem Anteil der von den Befragten falsch eingeschätzten Erreichbarkeiten.


# weiterführende Hinweise
Die Codes zur Durchführung der beiden Erreichbarkeitsanalysen im Bus- und Bahnverkehr wurden mit Python 3.10.20 in Visual Studio Code entwickelt.
Die Erreichbarkeitsanalysen in openrouteservice wurden mit den Verkehrsmitteln "foot-walking", "cycling-regular" und "driving-car" durchgeführt.
