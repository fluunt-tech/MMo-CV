# Korrigierte Finanzplan-Vorlagen

Stand: 05.11.2026. Technisch korrigierte Kopien der bereitgestellten Max-Muster-Dateien. Keine Anpassung an Dr. Mahsa Motlaghs Geschäftsmodell oder den Gründungsbeginn 09.12.2026. Die Quelldateien bleiben unverändert.

## Verwendung

- `Finanzplan_2026_korrigiert.xlsx`: Hauptansicht 2026, integrierte 2027-Detailplanung auf den Blättern mit Präfix `2027`.
- `Finanzplan_2027ff_korrigiert.xlsx`: Hauptansicht 2027 mit Vorschau 2028/2029, integrierte 2026-Planung mit Präfix `2026`.
- Jede Datei enthält beide Jahre und funktioniert ohne externe Excel-Dateien. Die beiden Dateien sind alternative, eigenständige Arbeitskopien; Änderungen werden **nicht** zwischen ihnen synchronisiert. Für die laufende Bearbeitung eine Datei als führende Version wählen.
- Frühere ausgeblendete Monatsvorschauen und der Soll-Ist-Vergleich bleiben ausgeblendet und können in Excel eingeblendet werden. Die Monatsvorschauen verteilen Jahreswerte gleichmäßig und sind keine eigenständig erhobene Monatsplanung.
- `Parameter` und `Prüfung` erläutern offene Eingaben. Zeitaufwand je Einheit in `Parameter!E19:E29` eintragen und verfügbare Monatsstunden in `Umsatzberechnung!C32:N32` prüfen. Ohne erforderliche Zeitangaben bleibt die Auslastung leer. Leere Ist-Felder bedeuten „noch nicht erfasst“, nicht tatsächliche Nullwerte.

## Reparaturen

1. Monatsdaten durch DATE-Formeln ersetzt; historische Datumssuchtabellen entfernt. Jahresgrenzen werden dynamisch ermittelt.
2. Defekte Vorsteuerbezüge ersetzt. Vorsteuersätze sind je Kostenposition in `Parameter!B13:B30` prüfbar. Für die Ausgabe-Vorsteuer ist der tatsächlich abziehbare Satz maßgeblich; Miete und Versicherungen werden nicht automatisch mit Umsatzsteuer belastet. Die erhaltene Umsatzsteuer wird weiterhin über `Liquiditätsplan!B7` gesteuert. Bei gemischten Steuersätzen sind Kosten aufzuteilen.
3. Falschen externen Verweis auf „Peter-Krisch“ durch interne Übernahme des Vorjahresbestands ersetzt. Umsatzsteuerverrechnung des Januars berücksichtigt den Dezember des Vorjahres.
4. 2027-Detailplanung als maßgebliche Quelle für die 2027/2028-Werte in der 2026-Vorschau verknüpft. Alte Wachstumsfelder der 2026-Planung sind mit Hinweisen als nicht mehr maßgeblich markiert. Jahresübersicht 2026 nun mit Formelbezügen statt festgeschriebenen Summen.
5. Doppelte Leistungszeile in der Umsatzberechnung repariert; alle vorgesehenen Leistungszeilen werden berücksichtigt. Stunden, Tage und Stückzahlen werden nicht mehr ungeprüft für eine Prozent-Auslastung addiert. Umrechnung erfolgt erst nach Eingabe von Stunden je Einheit.
6. Nicht mehr vorhandene Materialposition in den ausgeblendeten Monatsvorschauen ausdrücklich mit null angesetzt; übrige Kosten bleiben enthalten. Jahressummen summieren die Monatswerte. Blattnamen und Datumswerte den tatsächlich prognostizierten Jahren angepasst.
7. Soll-Ist-Vergleich vollständig neu mit allen vorgesehenen Kostenpositionen aufgebaut. Noch leere Ist-Eingaben erzeugen keine scheinbaren Ist-Salden oder Abweichungen.
8. Null-Finanzierung verursacht keinen Divisionsfehler bei der Eigenkapitalquote. Bewirtung und die freie Kostenzeile werden in der Ergebnisrechnung berücksichtigt.

## Fachlich offen

- Max-Muster-Honorare, Mengen, Kapazitäten, private Entnahmen und Steuersätze sind Beispielwerte. Vorhandene Kapazitätswerte von 120 bzw. 3 Stunden sind nicht validiert.
- Die Steuerrückstellung ist eine monatliche positive-Überschuss-Pauschale, keine individuelle Einkommensteuerberechnung. Verlustverrechnung über Monate wird darin nicht modelliert.
- Kapitaldienst in Liquiditätsplan Zeile 28 muss für die Ergebnisrechnung auf Zinsen/Gebühren beschränkt bleiben. Kredittilgungen sind keine Betriebsausgaben und müssten bei tatsächlichem Bedarf separat modelliert werden.
- Investitions- und Finanzierungsplan sind gesonderte Budgetpläne. Potenzielle Familienkredite sind keine bestätigten Zahlungseingänge. Daher werden sie nicht automatisch als Bankbewegung angesetzt. Tatsächliche Anfangsbestände können in `Parameter!B6` eingetragen werden; reale Startinvestitionen und Kreditbewegungen müssen vor Einreichung zusätzlich terminiert werden.
- Leistungen werden im selben Monat als Zahlungseingang angesetzt. Zahlungsziele und eine individuelle Förderzusage sind gesondert zu planen. Der Hinweis zum Gründungszuschuss stammt aus der Mustervorlage; er ist kein Anspruchsnachweis.
- Die Formelprüfung bestätigt technische Berechenbarkeit und die geprüften Rechenzusammenhänge, nicht die wirtschaftliche Tragfähigkeit oder eine vollständige steuerliche Prüfung.

## Validierung

Beide Dateien wurden mit LibreOffice Calc vollständig neu berechnet und als XLSX gespeichert. In jeder Datei: 20 Tabellenblätter, 4.019 Formelzellen, keine gespeicherten Excel-Fehlerwerte und keine externen Arbeitsmappenverknüpfungen. Zusätzlich geprüft: Monatsanfänge 2026/2027, fortgeschriebene Liquidität, Jahresübertrag und Übereinstimmung der Jahresvorschauen.

Ein gesonderter Test mit 19 % Umsatzsteuer, Beispiel-Zeitumrechnungen und 120 verfügbaren Stunden pro Monat wurde ebenfalls neu berechnet. Alle Formelzellen blieben ohne Fehlerwert; die Vorsteuer, der Umsatzsteuerübertrag und exemplarische Stunden-/Auslastungsergebnisse wurden geprüft. Diese Testannahmen sind nicht in den ausgelieferten Dateien aktiviert.

Unveränderte Muster-Ergebnisse: 2026 Umsatz 24.745 €, Gewinn vor Steuern 16.945 €; 2027 Umsatz 67.200 €, Gewinn vor Steuern 56.400 €.
