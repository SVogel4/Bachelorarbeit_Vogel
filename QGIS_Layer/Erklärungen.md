# QGIS-Layer

Dieser Ordner enthält die verschiedenen QGIS-Layer, die sich aus der Erreichbarkeitsanalyse der verschiedenen POIs ergeben.

## Unterordner zu den POIs
In der Unterordner der einzelnen POIs sind jeweils die POIs als Punktlayer dargestellt sowie die Erreichbarkeiten mit den verschiedenen Verkehrsmitteln. 
Hierzu zählen
`KiTas_Grundschulen`
`weiterfuehrendeSchule`
`Gesundheitsversorgung`
`Einkaufsmoeglichkeiten`
`Freizeitmoeglichkeiten`

Die POIs selbst ergeben sich aus der Befragung der Bewohnerinnen und Bewäóhner der beiden Dörfer Schaidt und vollmersweiler.
Die Erreichbarkeiten wurden mithilfe von openrouteservice oder der eigenen Erreichbarkeitsanalyse ermittelt.

## Erreichbarkeit der Zentroide
In dem Ordner zur Erreichbarkeit der Zentroide sind die jeweiligen ausgewählten zwei Zentroide der vier Bereiche des Untersuchungsgebietes gemeinsam mit ihrer Erreichbarkeit gespeichert. 
Hierbei wurden sowohl die vier Bereiche als auch im westlichen Bereich in einem Raster zwei Zentroide in ihrer Erreichbarkeit zu Fuß dargestellt.

## Beispiel Analyse
Der Inhalt des Ornders zeigt bezugnehmnd auf den ORdner mit den Erreichbarkeitsanalysen die Erreichbarkeit von zwei Haltestellen aus einmal im Bus- und im Regionalbahnverkehr an. Zudem sind die Bus- und Bahnhaltepunkte der beiden Dörfer kartiert.

## Auswertung
Dieser Ordner enthält bereits Ergebnisse aus der Analyse der Daten. 
Hierbei handelt es sich um den vergleich der subjektiv wahrgenommenen Erreichbarkeiteen, die in der Umfrage ermittelt wurden und der objektiven Erreichbarkeit, die mit Hilfe der Erreichbarkeitsanalysen ermittelt werden. 
Unter dem Dateinamen `Teilnehmer_je_Raster.gpkg` ist die Anzahl der Teilnehmer je Befragungsraster kartiert. 
Die Raster selbst sind nochmals unter `Raster_Schaidt_Vollmersweiler` dargestellt. 

Einen konkreten Vergleich stellt der Layer `Abweichung_Erreichbarkeit_Prozent`dar. 
Die Abweichungen der Erreichbarkeit folgern aus den Analysen mit ORS im Vergleich mit den Angaben der Befragten und dem Anteil falscher Antworten.


# weiterführende Hinweise
Die Codes zur Durchführung der beiden Erreichbarkeitsanalysen im Bus- und Bahnverkehr wurden mit Python 3.10.20 in Visual Studio Code entwickelt.
Die Erreichbarkeitsanalysen in openrouteservice wurden mit den Verkehrsmitteln "foot-walking", "cycling-regular" und "driving-car" durchgeführt.
