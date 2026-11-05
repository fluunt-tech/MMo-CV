# Finanzplan in zwei verknüpften Dateien

Geplanter Tätigkeitsbeginn: **10.12.2026**.

1. `Finanzplan_2026_Start_10-12-2026.xlsx`: nur das kurze Gründungsjahr 2026; Januar bis Dezember sind sichtbar, nur Dezember ist befüllt. Keine Folgejahresprognose in dieser Datei.
2. `Finanzplan_2027ff_verknuepft.xlsx`: monatliche Planung 2027, Jahresvorschau 2028/2029 und die verknüpfte Übersicht für 2026.

## So funktioniert die Verknüpfung

Beide Dateien herunterladen und im **selben lokalen Ordner** speichern. Die Dateinamen unverändert lassen. Alternativ das ZIP vollständig in einen Ordner entpacken; nicht einzelne Dateien direkt aus dem ZIP öffnen.

Zuerst die 2026-Datei in Excel bearbeiten, berechnen und speichern. Anschließend die 2027ff-Datei öffnen und die Aktualisierung der eigenen Arbeitsmappenverknüpfung erlauben. Falls Excel die Aktualisierung blockiert, unter **Daten → Arbeitsmappenverknüpfungen** (je nach Excel-Version „Verknüpfungen bearbeiten“) die Quelle prüfen bzw. auswählen. Sicherheitsrichtlinien von Excel können eine Freigabe erfordern. GitHub aktualisiert die Verknüpfung nicht im Browser.

Die 2027ff-Datei enthält genau eine relative externe Arbeitsmappenverknüpfung:

- `Liquiditätsplan!D37`: monatlicher Januarsaldo plus Dezember-Endbestand aus der 2026-Datei (`Liquiditätsplan!O37`) plus gegebenenfalls zusätzliche Anfangsmittel aus `Parameter!B6`.
- `Liquiditätsplan!D35`: Vorsteuer minus erhaltene Umsatzsteuer des Dezembers (`O33 − O7` der Quelle).
- `Tabelle1!B2` und `B4`: Dezemberumsatz und Gewinn vor Steuern aus der 2026-Rentabilitätsvorschau.

Es gibt **keine Rückverknüpfung** aus 2026 nach 2027. Damit entsteht keine zirkuläre Dateiverknüpfung. Wird eine Datei umbenannt oder allein verschoben, muss die Quelle in Excel neu ausgewählt werden. Ohne erreichbare Quelle kann Excel gespeicherte, veraltete Werte anzeigen. Nach Änderungen deshalb den Jahresübertrag kontrollieren.

## Prüfstand und offene Angaben

Beide Dateien wurden mit LibreOffice Calc neu berechnet; alle sichtbaren und ausgeblendeten Blätter wurden auf gespeicherte Excel-Fehlerwerte geprüft. Keine Fehlerwerte gefunden. Der ausgelieferte externe Dateipfad wurde auf den reinen Quelldateinamen gesetzt und geprüft; er enthält keinen Workspace- oder anderen lokalen Verzeichnispfad. Die interaktive Aktualisierung durch Microsoft Excel wurde hier nicht ausgeführt und hängt von den dortigen Verknüpfungs- und Sicherheitseinstellungen ab.

Aktualisierte Dezemberplanung nach Nutzerangabe: **0 € betrieblicher Umsatz, 0 € betriebliche Ausgaben, 0 € Gewinn**, keine geplanten Startinvestitionen oder Kreditbewegungen. Januar bis Dezember bleiben sichtbar. Januar–November enthalten keine Eingaben; rechnerische Nullergebnisse sind dort optisch ausgeblendet, während die Formeln erhalten bleiben. Nur Dezember ist befüllt. Die Hochrechnung für 2026 wurde entfernt. Folgejahre stehen ausschließlich in der zweiten Datei.

Im neuen Blatt `Gründungszuschuss` wird der volle Monatsbetrag von **3.300 €** als Nutzerangabe hinterlegt. Vorläufige Planannahme: **3.300 € / 30 × 22 Kalendertage = 2.420 €** für 10.–31.12.2026. Anspruch, Förderkomponenten, anteiliger Betrag und tatsächlicher Auszahlungstermin sind anhand des Bescheids zu bestätigen. Es wird angenommen, dass der Betrag im Dezember zufließt und vollständig dem Unternehmen als Einlage zugeführt wird. Bei späterem Zufluss muss die Liquiditätsplanung angepasst werden.

Der Zuschuss ist **kein betrieblicher Umsatz und kein betrieblicher Gewinn**. Die geplante Zuführung ist separat in `Liquiditätsplan!O40` erfasst und erhöht den fortgeschriebenen Bestand in `O37`. Damit betragen Dezember-Endbestand und Januar-Anfangsbestand aktuell **2.420 €**. Die verknüpfte Jahresübersicht übernimmt für 2026 Umsatz und Gewinn von jeweils null. Privater Lebensunterhalt wird aus dieser Planung nicht finanziert und benötigt eine separate Deckung. Keine doppelte Erfassung als Anfangsbestand oder Einlage im Jahr 2027.

Beide Dateien wurden nach dieser Änderung neu berechnet: keine gespeicherten Excel-Fehlerwerte; alle zwölf Monatsspalten sichtbar; nur Dezember befüllt; Hochrechnung entfernt; betriebliche Nullplanung und verknüpfter Übertrag von 2.420 € geprüft. Die interaktive Aktualisierung in Microsoft Excel hängt weiterhin von den lokalen Sicherheitseinstellungen ab. 2027-Honorare, Mengen, Kosten und Privatentnahmen bleiben unbestätigte Musterwerte.

Die früheren integrierten Arbeitsmappen bleiben als ältere Alternativen erhalten und synchronisieren sich nicht mit diesen Dateien. Für die weitere Bearbeitung dieses Dateipaar verwenden. Die Businessplan-Dokumente nennen weiterhin den früheren Beginn 09.12.2026 und müssen vor gemeinsamer Einreichung ebenfalls auf 10.12.2026 geändert werden.
