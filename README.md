# NK-Import

Ab der DATAflor Business Version 2022 unterstützt der Digitale Posteingang den Import von Nachkalkulationsdaten in das DATAflor BUSINESS.

Der Import erfolgt über die Verzeichnisüberwachung (ein Import über die Programmoberfläche wird nicht unterstützt) und verwendet als Dateiformat XML.

Der Aufbau der XML-Datei muss dem Schema DFNKImport.xsd entsprechen. Für einen erfolgreichen Import müssen die entsprechenden Nummer-Felder (LV-Nr, Positions-Nr und Stammdatensatz-Nummern) einem Datensatz im DATAflor BUSINESS entsprechen. 

Wenn ein Datensatz nicht zugeordnet werden kann oder sonstige Fehler enthält, wird die komplette Datei nicht importiert! Die importierte Datei wird dann (zusammen mit einer Fehlerbeschreibungsdatei, die den gefundenen Fehler beschreibt) in das Verzeichnis BusinessData\Inbox Files\failed (in der BUSINESS-Freigabe auf dem Server) verschoben.

