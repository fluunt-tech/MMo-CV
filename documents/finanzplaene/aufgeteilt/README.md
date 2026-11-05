# Finanzplan in zwei verknüpften Dateien

Geplanter Tätigkeitsbeginn: **10.12.2026**.

1. `Finanzplan_2026_Start_10-12-2026.xlsx`: nur das kurze Gründungsjahr 2026; operative Werte Januar bis November sind null und ausgeblendet. Keine Folgejahresprognose in dieser Datei.
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

Die gespeicherten Werte stimmen überein: 2026-Umsatz 4.375 €, Gewinn vor Steuern 3.650 €, Dezember-Endbestand und Januar-Anfangsbestand −420 €. Die ursprünglichen Dezember-Musterwerte wurden nicht zeitanteilig gekürzt. Es handelt sich weiterhin um unbestätigte Beispielwerte für Preise, Mengen, Kosten, Privatentnahmen, Rücklagen und Finanzierung. Das Startblatt und die Parameterblätter erläutern die nötigen Eingaben. Ein potenzieller Kredit wird nicht als tatsächlich eingegangene Zahlung behandelt.

Die früheren integrierten Arbeitsmappen bleiben als ältere Alternativen erhalten und synchronisieren sich nicht mit diesen Dateien. Für die weitere Bearbeitung dieses Dateipaar verwenden. Die Businessplan-Dokumente nennen weiterhin den früheren Beginn 09.12.2026 und müssen vor gemeinsamer Einreichung ebenfalls auf 10.12.2026 geändert werden.
