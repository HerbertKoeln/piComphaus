# piComphaus
Die iPhone-App dient dazu, Steueraufgaben die in einem Haus automatisiert erledigt werden sollen zu überwachen und ggf. durch gezielte Aktionen zu beeinflussen. Die eigentliche Steuerung erfolgt auf einem Raspberry Pi, der über eine Hardwareschnittstell zum 1-Wire Bus verfügt, über den die Sensoren und Schaltern angebunden sind. Dies Steuerung ist Bestandteil dieses Github-Projekts und wird dort sukzessive veröffentlicht.<p>
Basisaufgabe des Gesamtsystems ist das Steuern von Rollladen und/oder Jalousien, die nach einem in einer Datenbank hinterlegten Zeitplan gesteuert werden. Dieser Zeitplan berücksichtigt Sonn- und Feiertage sowie die aktuelle Helligkeit zum gewünschten Schaltzeitpunkt. Dadurch kann z.B. im Winter der Öffnungszeitpunkt innerhalb eines Zeitfensters verzögert werden. Unabhängig davon kann jederzeit eine Schaltaktion über die App ausgelöst bzw. unterbunden werden.<p> 
Da die App ohne Verbindung zum Server nicht funktionsfähig ist, verfügt sie über einen Simulationsmodus, der nach Installation automatisch aktiv ist. Dadurch kann ein Eindruck von der Funktionalität vermittelt werden, allerdings ohne wirklich Schalten und Steuern zu können. Alle angezeigten Inhalte sind in die App integriert und es erfolgen keine Netzwerkzugriffe.
<h4>Hauptfenster</h4>
Hier kann der Schaltzustand (Position der Rollladen) des ausgewählten Schalters angezeigt. Wählt man im oberen Fensterbereich die gewünschte neue Position aus und betätigt den Ausführen Button, dann wird die Schaltaktion ausgelöst.
<h4>Zimmer</h4>
Hier werden Temperaturen der Heizungsanlag sowie der einzelnen Zimmer angezeigt. Eine Temperatur Steuerung ist dabei zeitabhängig für jedes einzelne Zimmer möglich.  
<h4>WindInfo</h4>
Aktuelle Windvorhersagen für den jeweiligen Standort werden in einer Tabelle für mehrere Tage dargestellt. Bei Überschreitung einer Maximalgeschwindigkeit wird eine Warnung per Appel Push Notifikation an den App Nutzer übermittelt. Dieser kann dann entsprechend reagieren und die Jalousien öffnen, um ggf. Schäden zu vermeiden.
<h4>Spezial</h4>
Jeder Schalter verfügt über eine Basiskonfiguration, die über diese Seite modifiziert werden kann. Die ist notwendig, da z.B. die Zeiten zum öffnen und schließen der Rollladen sehr individuell angepasst werden müssen. Darüber hinaus können weitere Parameter eingestellt und deren Auswirkung gleich getestet werden. Ebenso unterstützen die dort verfügbaren Funktionen Reparaturarbeiten an den Rollladen und Jalousien, die von Zeit zu Zeit notwendig werden.
<h4>Benachrichtigung</h4>
Der App-Nutzer kann hier auswählen, worüber er per Push Notifikation benachrichtigt werden möchte.  
<h4>Einstellungen</h4>
Diese Seite dient der Konfiguration der Verbindung zum Server. Durch ausschalten der Simulation erscheint ein Menü, in dem bis zu drei verschiedene Verbindungen konfiguriert werden können, die dann im Hauptfenster über das Buch Icon oben rechts aktiviert werden können.
