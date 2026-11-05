# Korrigierte Finanzplan-Vorlagen

Stand: 05.11.2026. Technisch korrigierte Kopien der bereitgestellten Max-Muster-Dateien. Keine Anpassung an Dr. Mahsa Motlaghs Geschäftsmodell oder den Gründungsbeginn 09.12.2026. Die Quelldateien bleiben unverändert.

## Aktuell: zwei verknüpfte Dateien

Im Unterordner `aufgeteilt/` liegen die separate 2026-Datei und die extern verknüpfte 2027ff-Datei. Das ZIP enthält beide Dateien und eine Anleitung. Dieses Paar ist für die weitere Bearbeitung vorgesehen. Ältere Ein-Datei-Versionen bleiben erhalten, synchronisieren sich aber nicht.

## Frühere zentrale Arbeitsdatei mit Start 10.12.2026

`Finanzplan_Mahsa_Motlagh_Start_10-12-2026.xlsx` ist die aktualisierte zentrale Fassung. Sie enthält ein Startblatt mit dem tatsächlichen geplanten Tätigkeitsbeginn **10.12.2026**, den kurzen Startmonat Dezember 2026, die monatliche Planung 2027 und die Jahresvorschau 2028/2029.

Januar bis November 2026 wurden bei Umsatzmengen, laufenden Betriebskosten und Privatentnahmen auf null gesetzt und die betreffenden Monatsspalten ausgeblendet. Die Kalenderjahresgrenzen bleiben erhalten, sodass Dezember nicht doppelt erfasst wird. Die Monatsüberschrift 01.12.2026 bezeichnet den Monat, nicht den Tätigkeitsbeginn. Eventuelle tatsächliche Vorgründungskosten sind zusätzlich gesondert zu erfassen.

Die ursprünglichen Dezember-Musterwerte wurden beibehalten und kommentiert, nicht automatisch auf 22/31 gekürzt. Aufträge, Fälligkeiten, Privatbedarf und Startfinanzierung sind weiterhin zu bestätigen. Das unbestätigte Rücklagenziel von 6.500 € in der 2026-Ergebnisübersicht ist keine erfasste Bankbewegung. Die Datei ist daher ein Planentwurf, keine fertig individualisierte Tragfähigkeitsrechnung.

Bei unverändertem Dezember-Musterumsatz von 4.375 €, Gewinn vor persönlichen Steuern von 3.650 € und Anfangsliquidität null ergibt sich ein Endbestand zum 31.12.2026 von **−420 €**. Dieser wird nach Januar 2027 übertragen. Der niedrigste Monatsendbestand 2027 ist **−1.989,25 €**. Bestätigte Finanzierung und reale Startauszahlungen müssen ergänzt werden; potenzielle Kredite werden nicht als bereits eingegangen behandelt.

Neu berechnet und geprüft: keine Excel-Fehlerwerte oder externen Arbeitsmappenverknüpfungen, kein operativer Umsatz oder laufender Zahlungsabfluss vor Dezember 2026, richtige Datumswerte, identischer Jahresübertrag und unveränderter 2027-Musterumsatz. Vorherige Dateien bleiben als ältere Fassungen erhalten. Die Businessplan-Dokumente nennen noch den früheren Start 09.12.2026 und müssen vor gemeinsamer Einreichung ebenfalls angepasst werden.

## Verwendung der älteren korrigierten Vorlagen

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
