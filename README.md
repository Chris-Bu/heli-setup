# Heli Setup – Digitale Rotorkopfvermessung · Version 1.2

Offlinefähige PWA für Android und Windows.

## Neues Verfahren für Null-Pitch und Taumelscheibe
1. VMS: sechs Winkel erfassen.
2. Drei Blatthalterwinkel an den Servopositionen erfassen.
3. Drei Servomitten nach berechneten Sollwinkeln einstellen. Die Berechnung bewahrt den gemeinsamen Winkelversatz der oberen Anlenkung.
4. Alle drei Winkel erneut messen und ggf. nachstellen.
5. Oberes Gestänge an Servo 3 auf den VMS-basierten Null-Pitch-Sollwinkel einstellen.
6. Drei Endmessungen und getrennte Prüfung von gemeinsamem Versatz und Restneigung.
7. Tatsächliche Neutralanzeige für Kollektiv/Zyklisch erfassen.

Rechenmodell: q_i = -servoMidTarget(i) in der Außen-positiv-Konvention; x = Mittelwert(m_i-q_i); Servo-Sollwinkel q_i+x; Gestänge-Sollwinkel q_3. Für drei 120°-Positionen ist die mittlere Restneigung null. Gilt unter der bisherigen linearen Winkelmodell-Annahme und unveränderter Messgeräteorientierung.

Die Messdaten bleiben über den bisherigen lokalen Speicher-Schlüssel erhalten. Beim Update kann der alte Navigationsschritt in den neuen Ablauf fallen; über die Kapitelübersicht den passenden Schritt auswählen.

Wichtig: Motor elektrisch trennen; vor Flug Wirkrichtungen, Freigängigkeit und Pitch am lotrecht ausgerichteten Heli unabhängig kontrollieren.
