# Heli Setup 1.4

Im Einrichtungsabschnitt sind die Original-Punkte 1.3 (Blatthalter zieht/schiebt), 1.4 (Taumelscheibe steigt/sinkt bei mehr positivem Kollektiv-Pitch) und 1.6 (Nickservo vorne/hinten) enthalten.

Die Bewegung aus 1.4 wird gespeichert und bei den Kollektiv-Pitch-Sollwerten berücksichtigt. Bei unbekannter Richtung fordert die App eine Auswahl an. Der zyklische Pitch bleibt von dieser Auswahl unabhängig.

Außerdem ist die Zuordnung der Eingabemasken zu den Schritten im Einrichtungsabschnitt berichtigt; die Pitchwerte stehen nun bei Schritt 1.6 und die Nickservo-Auswahl bei 1.6. Bestehende Messdaten bleiben erhalten.

## Version 1.6 (Teststand)
Die drei Libellen-Auswahlfelder zeigen jetzt unmittelbar die eindeutigen Soko-Symbole O-- (Außen), -O- (Mitte) und --O (Innen). Die internen Vorzeichen sind unverändert (Außen positiv, Innen negativ). Bei Nachstellrunden bleiben die letzten drei vollständigen Kontrollmessungen als Berechnungsbasis erhalten, bis neue Kontrollwerte vollständig erfasst sind. Nach diesem Update bitte einen neuen Einstellvorgang beginnen, da ältere Messwerte wegen der vorher missverständlichen Anzeige nicht zuverlässig zugeordnet werden können.


## Gezielte Nachstellung in Testversion 1.6

Bei der Neigungskontrolle wird die größte der drei um den gemeinsamen Versatz bereinigten Abweichungen bestimmt. Pro Nachstellrunde wird **nur dieses eine Servo** korrigiert, und zwar zunächst um **60 %** der berechneten Winkelabweichung. Die beiden anderen Servomitten bleiben unverändert. Anschließend werden **alle drei Positionen erneut gemessen**. Das ist ein vorsichtiges iteratives Verfahren; es ersetzt keine individuelle Messung der mechanischen Kopplung und garantiert keine Konvergenz. Der gemeinsame Versatz wird erst später am oberen Gestänge korrigiert. Die bisherige Messreihe kann importiert werden.
