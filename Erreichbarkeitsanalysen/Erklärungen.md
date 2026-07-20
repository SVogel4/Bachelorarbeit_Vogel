# Erreichbarkeitsanalysen

Dieser Ordner enthält die Python-Skripte zur Durchführung der Erreichbarkeitsanalysen im Bus- und Bahnverkehr sowie die hierfür benötigten Datengrundlagen.

## Bevölkerungsraster
Beide Erreichbarkeitsanalysen basieren auf dem Bevölkerungsraster im Umfeld von Schaidt. Die Rasterdaten beruhen auf den Bevölkerungsdaten des Zensus-Atlas und 
liegen als deutsches INSPIRE-Geogitter mit einer räumlichen Auflösung von 100 × 100 m in Lambert-Projektion vor. Die Daten wurden vom Bundesamt für Kartographie und Geodäsie (BKG) bereitgestellt.
Die Rasterdaten werden als GeoJSON-Datei in das Projekt eingebunden und befinden sich unter dem Dateinamen:
`Raster_BZA_Woerth`.geojson

## OpenStreetMap-Daten
Als Grundlage für das Wegenetz werden für beide Analysen Daten aus OpenStreetMap (OSM) von der offiziellen Webseite verwendet. 
Diese sind im Repository unter folgendem Dateinamen gespeichert:
`OSM_Daten`.pbf 

## GTFS-Daten des Busverkehrs
Die GTFS-Daten des Busverkehrs konnten aufgrund ihrer Dateigröße nicht in das GitHub-Repository integriert werden. Sie können über das Open-Data-Portal des Verkehrsverbundes Rhein-Neckar (VRN) unter folgendem Link heruntergeladen werden:
https://opendata.vrn.de/datasets/vrn-und-rnn-gtfs-sollfahrplandaten-aktuell (letzter Zugriff am 20.07.2026)
Für die Reproduzierbarkeit der Analysen ist der Datensatz mit Stand vom 23.06.2026 zu verwenden. Nach dem Download der ZIP-Datei ist diese entsprechend der im Python-Skript verwendeten Dateibezeichnung umzubenennen.

## GTFS-Daten des Bahnverkehrs
Die für die Erreichbarkeitsanalyse mit der Regionalbahn benötigten GTFS-Daten werden unter dem Dateinamen
`Schienenverkehr`.zip
bereitgestellt und können direkt in die Analyse eingebunden werden.
Die Daten stammen von der Plattform gtfs.de und umfassen den regionalen Schienenverkehr innerhalb der Untersuchungsregion.

## weiterführende Hinweise
Die Erreichbarkeitsanalyse wurde nach einer Vorlage von Prof. Dr.-Ing. Yu Feng programmiert, die unter 
`Vorlage_Analyse_Feng.html` 
gespeichert ist.

Detaillierte Erläuterungen zum Aufbau und Ablauf der Analysen sind in den Dateien
`Erreichbarkeitsanalyse_Bus`
`Erreichbarkeitsanalyse_Bahn`
enthalten. Dort werden die einzelnen Verarbeitungsschritte sowie die benötigten Eingabedaten näher beschrieben. 
