# Lösungshinweise zu KSM IT-System-Management

## Probeprüfung Nr. 1 (KSM AP2 PB1)

### 1. Aufgabe (24 Punkte)

#### Aufgabenteil a (4 Punkte)

1. Smarte Thermostate

- Automatisierte Temperaturregelung
- Anpassung an Nutzergewohnheiten
- Senkung des Energieverbrauchs um 10-15 %
- Remote-Steuerung möglich

2. Intelligente Beleuchtungssysteme

- Automatisierte Beleuchtung basierend auf Anwesenheitssensoren
- Anpassung an Tageszeit und natürliches Licht
- Stromverbrauch für Beleuchtung um bis zu 50 % reduziert

3. Energiemanagement-Sensoren

- Echtzeitüberwachung des Energieverbrauchs
- Identifikation ineffizienter Geräte
- Energieverbrauch um bis zu 20 % senkbar
- Daten zur Optimierung und Verbrauchsspitzen-Glättung

4. Gebäude-Überwachungssoftware

- Integration und Analyse von Sensordaten
- Visualisierung des Energieverbrauchs
- Echtzeit-Alarme und Optimierungsvorschläge
- Energieeinsparungen von 10-30 % möglich

#### Aufgabenteil b (4 Punkte)

Vorteile von WLAN:

- Flexibilität bei der Installation
- Einfachere und kostengünstigere Nachrüstung
- Keine Einschränkungen durch Kabelwege
- Mobilität der Geräte
- Geringerer baulicher Aufwand

Nachteile von WLAN:

- Anfälliger für Störungen und Interferenzen
- Begrenzte Reichweite im Vergleich zu kabelgebundenen Verbindungen
- Höherer Energieverbrauch der Geräte
- Sicherheitsrisiken bei unzureichender Verschlüsselung
- Potenziell geringere Übertragungsgeschwindigkeit und Stabilität

#### Aufgabenteil c

#### Aufgabenteil ca (3 Punkte)

- Ein Mesh-Netzwerk besteht aus mehreren Zugangspunkten (Nodes), die sich drahtlos miteinander verbinden.
- Diese Nodes leiten Datenpakete untereinander weiter, um eine flächendeckende WLAN-Abdeckung zu gewährleisten.
- Jeder Node agiert als Relaisstation, wodurch eine flexible und erweiterbare Netzwerkinfrastruktur entsteht.

#### Aufgabenteil cb (2 Punkte)

- Der sogenannte "Seamless Roaming"-Mechanismus ermöglicht es Endgeräten, nahtlos von einer Funkzelle zur nächsten zu wechseln.
- Die Verbindung bleibt dabei stabil und ununterbrochen, was für den Benutzer eine kontinuierliche Sitzung ohne Unterbrechung sicherstellt.

#### Aufgabenteil cc (2 Punkte)

- Ein echtes Mesh-Netzwerk benötigt mindestens zwei alternative Pfade zwischen den Nodes.
- Damit dies funktioniert, sind mindestens drei Zugangspunkte erforderlich, um Redundanz zu schaffen und Daten flexibel weiterleiten zu können.

#### Aufgabenteil cd (3 Punkte)

- Ein Tri-Band-System verwendet unterschiedliche Frequenzbänder, um Stabilität und Effizienz zu gewährleisten.
- Die Verbindung zwischen den Nodes erfolgt über einen hohen Kanal im 5 GHz-Bereich, während die Datenübertragung für WLAN-Clients über das 2.4 GHz-Band und einen unteren Kanal im 5 GHz-Bereich erfolgt.

#### Aufgabenteil ce (4 Punkte)

- "Mesh-Steering" bezieht sich auf die gezielte Steuerung der Endgeräte durch das Mesh-Netzwerk.
- Der Ansatz sorgt dafür, dass Clients automatisch mit dem optimalen Zugangspunkt verbunden werden, was die Netzwerkstabilität und Performance verbessert.

#### Aufgabenteil cf (2 Punkte)

- Die Kompatibilität zwischen Komponenten unterschiedlicher Hersteller ist oft eingeschränkt, da diese möglicherweise proprietäre Protokolle oder Standards verwenden.
- Für eine reibungslose Interoperabilität ist es ratsam, Geräte desselben Herstellers oder solcher zu nutzen, die kompatible Standards wie IEEE 802.11s unterstützen.

### 2. Aufgabe (26 Punkte)

#### Aufgabenteil a (5 Punkte)

- Subnetz in CIDR-Schreibweise für den Showroom: 172.18.3.0/24 (oder alles mit 0 und von 3 bis 255 richtig)
- IP-Adresse und Subnetzmaske für ...
  - WLAN Access-Point: 172.18.3.1
  - Raspberry Pi: 172.18.3.2
  - ZigBee IP-Bridge: 172.18.3.3
  - KNX IP-Interface: 172.18.3.4

Keine Dopplungen der IP-Adressen, IP-Adressen müssen aus dem korrekten Subnetz stammen.

#### Aufgabenteil b (2 Punkte)

Um die drahtlosen ZigBee-Geräte in das Netzwerk zu integrieren, wird das OSI-7-Schichten-Modell als Grundlage verwendet. ZigBee baut wie Bluetooth auf dem IEEE-Standard 802.15.4 auf, der die unteren beiden OSI-Schichten abdeckt.

Ergänzen Sie in der folgenden Tabelle die Namen der fehlenden OSI-Schichten, um das OSI-Modell vollständig darzustellen.

| Schicht | Name |
| :---: | :--- |
| 7 | Anwendungsschicht |
| 6 | Darstellungsschicht |
| 5 | Sitzungsschicht |
| 4 | Transportschicht |
| 3 | Netzwerkschicht / Vermittlungsschicht |
| 2 | Sicherungsschicht |
| 1 | Bitübertragungsschicht |

#### Aufgabenteil c (6 Punkte)

*Sensoren:*

- Grundlegende Funktion: Sensoren erfassen physikalische oder umgebungsbedingte Veränderungen und wandeln diese in elektrische Signale um. Diese Signale werden dann an ein zentrales Steuersystem oder an Aktoren weitergeleitet, um eine Reaktion auszulösen.
- Beispiel: Ein Bewegungsmelder erkennt Bewegung in einem Raum und sendet ein Signal an ein Smart-Home-System, um Aktionen wie das Einschalten der Beleuchtung auszulösen.

*Aktoren:*

- Grundlegende Funktion: Aktoren setzen empfangene Signale in physische Aktionen um, indem sie mechanische Bewegungen oder andere Outputs ausführen. Sie sind für die Umsetzung von Steuerungsbefehlen zuständig, die von einem Steuerungssystem oder einem Sensor ausgelöst werden.
- Beispiel: Ein smarter Thermostat ist ein Aktor, der die Heizung basierend auf den Eingaben eines Temperatursensors steuert und die Raumtemperatur anpasst.

#### Aufgabenteil d (4 Punkte)

*Bus-Topologie:*

- Eigenschaften:
  - Alle Geräte sind über eine gemeinsame Leitung (Bus) miteinander verbunden.
  - Daten werden linear entlang dieser Leitung übertragen, und alle Geräte empfangen die gesendeten Signale.
  - Kosteneffizient und einfach zu installieren, besonders bei kleineren Netzwerken.
  - Ein einzelner Ausfall der Busleitung kann das gesamte Netzwerk beeinträchtigen.
- Beispiel neben KNX: CAN-Bus (z. B. in Fahrzeugen zur Steuerung von Elektroniksystemen)

*Stern-Topologie:*

- Eigenschaften:
  - Alle Geräte sind direkt mit einem zentralen Knoten (z. B. einem Router oder Switch) verbunden.
  - Der zentrale Knoten steuert die Kommunikation und leitet Datenpakete zwischen den Geräten weiter.
  - Höhere Ausfallsicherheit, da der Ausfall eines einzelnen Geräts das Netzwerk nicht beeinträchtigt. Ein Ausfall des zentralen Knotens führt jedoch zum Zusammenbruch des gesamten Netzwerks.
  - Gut skalierbar und einfach zu erweitern.
- Beispiel neben ZigBee: WLAN-Heimnetzwerke (mit einem Router als zentralem Punkt)

#### Aufgabenteil e

#### Aufgabenteil ea (6 Punkte)

Als Nachteil der Nutzung von Smart-Home-Komponenten wird in der Regel der zusätzliche Energiebedarf angegeben. Hierbei gilt es also den Trade-Off zwischen Funktion und weiteren Kosten abzuwägen. Um im Showroom entsprechend argumentativ gerüstet zu sein, bereiten Sie eine Beispielrechnung vor.

Berechnen Sie bei einem Strompreis von 28 Cent je Kilowattstunde und bei einem Preis von 0,55 EUR je AAA-Batterie die Energiekosten für den KNX-Einsatz auf der einen und den ZigBee-Einsatz auf der anderen Seite.

| Gerät | Anzahl | Leistung | Betriebsdauer |
| :--- | :---: | ---: | :--- |
| KNX-BUS Netzteil | 1 | 1,4 Watt | 24h / 365 Tage |
| KNX-BUS IP-Interface | 1 | 0,9 Watt | 24h / 365 Tage |
| KNX-BUS Binäreingang (8-fach) | 1 | 0,3 Watt | 24h / 365 Tage |
| ZigBee Bridge | 1 | 4 Watt | 24h / 365 Tage |
| ZigBee Tür-/Fenster-Kontakt | 8 | 1x AAA-Batterie/pa | 365 Tage |

Berechnen Sie den jährlich anfallenden Strombedarf in Kilowattstunden und die jährlichen Kosten je System.

\(KNX Leistung = 1,4\,\text{W} + 0,9\,\text{W} + 0,3\,\text{W} = 2,6\,\text{W}\)  
\(KNX Energie = 2,6\,\text{W} * 24\,\text{h} * 365\,\text{Tage} = 22776\,\text{Wh} ≙ 22,78\,\text{kWh}\)  
\(KNX Kosten pro Jahr = 22,78\,\text{kWh} * 0,28\,\text{EUR/kWh} = 6,38\,\text{EUR}\)

\(ZigBee Leistung = 4\,\text{W}\)  
\(ZigBee Energie = 4\,\text{W} * 24\,\text{h} * 365\,\text{Tage} = 35040\,\text{Wh} ≙ 35,04\,\text{kWh}\)  
\(ZigBee Kosten pro Jahr = \,\text{kWh} * 0,28\,\text{EUR/kWh} + 8\,\text{AAA-Batterien} * 0,55\,\text{EUR} = 39,44\,\text{EUR}\)

#### Aufgabenteil eb (3 Punkte)

Bei entsprechender Begründung kann beides korrekt sein:

*Vorschlag für ein KNX-basiertes Smart-Home-System:*

- **Empfohlene Kombination von Geräten:** Smarte Thermostate, Beleuchtungssysteme, Rollladensteuerungen, Sicherheitskameras und Bewegungsmelder.
- **Begründung:**
  - Stabilität und Zuverlässigkeit: KNX ist kabelgebunden und bietet daher eine extrem stabile und zuverlässige Verbindung, die besonders für größere Gebäude oder komplexe Installationen von Vorteil ist.
  - Skalierbarkeit und Flexibilität: Das System ist flexibel erweiterbar und eignet sich hervorragend für die Integration einer Vielzahl von Geräten und Funktionen in einem komplexen Gebäudeautomatisierungssystem.
  - Interoperabilität: KNX ist ein offener Standard, der die Integration von Geräten unterschiedlicher Hersteller ermöglicht, was eine größere Auswahl und Anpassungsmöglichkeiten bietet.
  - Datensicherheit: Aufgrund der kabelgebundenen Kommunikation bietet KNX eine höhere Datensicherheit und ist weniger anfällig für drahtlose Störungen oder Angriffe.

*Vorschlag für ein ZigBee-basiertes Smart-Home-System:*

- **Empfohlene Kombination von Geräten:** Intelligente Beleuchtung, smarte Steckdosen, Tür- und Fenstersensoren, Bewegungsmelder und smarte Lautsprecher.
- **Begründung:**
  - Einfache Installation und Flexibilität: ZigBee ist ein drahtloses System und eignet sich besonders gut für Nachrüstungen oder Mieter, da keine aufwendigen Kabelinstallationen erforderlich sind.
  - Kosteneffizienz: Im Vergleich zu kabelgebundenen Systemen wie KNX sind die Installationskosten und die Gerätepreise oft günstiger, was es ideal für kleinere Smart-Home-Projekte macht.
  - Mesh-Netzwerk-Funktionalität: ZigBee bietet eine Mesh-Netzwerkstruktur, bei der Geräte untereinander Signale weiterleiten, was die Abdeckung verbessert und die Kommunikation stabil hält.
  - Energieeffizienz: ZigBee-Geräte sind in der Regel sehr stromsparend, was die Batterielebensdauer bei kabellosen Sensoren und Aktoren verlängert.

### 3. Aufgabe (Punkte)

#### Aufgabenteil a (3 Punkte)

- Stars (Sterne)
- Cash Cows (Milchkühe)
- Dogs (Arme Hunde)

#### Aufgabenteil b (3 Punkte)

- **Hohes Marktwachstum:** Der Smart-Home-Markt wächst kontinuierlich durch das steigende Interesse an Automatisierung und Energieeffizienz. Neue Technologien und Innovationen treiben dieses Wachstum an.
- **Geringer Marktanteil:** Trotz des wachsenden Marktes haben viele Produkte in dieser Kategorie noch keine signifikante Marktstellung erlangt. Dies liegt an der starken Konkurrenz und der Vielzahl neuer Anbieter und Technologien.
- **Hohe Investitionsanforderungen:** Smart-Home-Produkte erfordern oft umfangreiche Investitionen in Forschung, Entwicklung und Marketing, um wettbewerbsfähig zu sein und die Verbraucher zu überzeugen.
- **Unsicherheit hinsichtlich der Akzeptanz:** Produkte in dieser Kategorie stehen vor der Herausforderung, sich gegen etablierte Technologien durchzusetzen und breite Akzeptanz bei den Verbrauchern zu finden. Es ist unklar, ob sie genügend Marktanteile gewinnen können, um sich zu lohnen.
- **Möglichkeit, zu "Stars" zu werden:** Wenn ein Smart-Home-Produkt durch strategische Investitionen und erfolgreiche Positionierung seine Marktstellung verbessert, kann es zu einem „Star“ aufsteigen, was hohe Umsätze und Gewinne zur Folge hat.
- **Hohe Risiken:** Aufgrund des Wettbewerbs und der schnellen technologischen Entwicklungen besteht die Gefahr, dass ein Produkt nicht die erwartete Akzeptanz erhält und langfristig eher zu einem "Poor Dog" wird.

#### Aufgabenteil c (4 Punkte)

**Investitionsstrategie zur Marktdurchdringung**

- **Beschreibung:** Diese Strategie beinhaltet gezielte Investitionen in Werbung, Produktentwicklung und Marktanalysen, um den Marktanteil der neuen Produktgruppe zu steigern. Dies kann durch intensive Marketingkampagnen, Promotions und Kooperationen mit anderen Smart-Home-Marken erfolgen, um die Bekanntheit zu erhöhen und das Vertrauen der Verbraucher zu gewinnen.
- **Eignung für "Question Marks":** Da "Question Marks" sich in einem wachsenden Markt befinden, jedoch noch keinen großen Marktanteil besitzen, ist es entscheidend, diesen schnell zu vergrößern. Durch umfangreiche Investitionen wird die Position der Produktgruppe gestärkt und es besteht die Chance, sie zu einem "Star" zu entwickeln. Der Fokus auf Markenbildung und Produktbekanntheit hilft, sich von Wettbewerbern abzuheben und eine loyale Kundenbasis aufzubauen.

**2. Differenzierungsstrategie**

- **Beschreibung:** Diese Strategie zielt darauf ab, die Produktgruppe durch einzigartige Merkmale und Vorteile von den Wettbewerbern abzuheben. Dies kann durch innovative Features, eine benutzerfreundliche Bedienoberfläche, verbesserte Sicherheit oder die Integration neuer Technologien erreicht werden. Ein gezieltes Content-Marketing mit Demonstrationen, Tutorials und Erfahrungsberichten ist ebenfalls Teil dieser Strategie, um die Alleinstellungsmerkmale hervorzuheben.
- **Eignung für "Question Marks":** Die Differenzierungsstrategie ist besonders geeignet, da "Question Marks" in einem umkämpften Markt operieren und es entscheidend ist, die Aufmerksamkeit der Verbraucher zu gewinnen. Ein klar erkennbarer Mehrwert kann den Marktanteil steigern und dazu beitragen, das Produkt zu einem „Star“ zu machen. Diese Strategie spricht gezielt technikaffine Kunden an, die nach Innovationen suchen und bereit sind, in Smart-Home-Lösungen zu investieren, die über Basisfunktionen hinausgehen.

#### Aufgabenteil d (3 Punkte)

**1. Zentralisierte Kundeninformation:**

- **Erklärung:** Ein CRM-System sammelt und verwaltet alle Kundendaten zentral, einschließlich Kaufhistorien, Kontaktdaten, Präferenzen und Kommunikationshistorien. Dies ermöglicht ein umfassendes Verständnis der Kundenbedürfnisse.
- **Vorteil im Kundenkontakt:** Vertriebsteams können maßgeschneiderte Empfehlungen geben und auf individuelle Kundenanfragen präzise eingehen, was das Vertrauen und die Zufriedenheit der Kunden stärkt.

**2. Personalisierte Marketingkampagnen:**

- **Erklärung:** CRM-Systeme ermöglichen die Segmentierung der Zielgruppe basierend auf verschiedenen Kriterien wie Interessen, Kaufverhalten und demografischen Merkmalen. Dies erlaubt eine zielgerichtete Ansprache.
- **Vorteil im Kundenkontakt:** Kunden erhalten relevante Informationen und Angebote, die ihren individuellen Interessen entsprechen, was die Wahrscheinlichkeit von Kaufentscheidungen erhöht und die Kundenbindung stärkt.

**3. Automatisierung von Marketing- und Vertriebsprozessen:**

- **Erklärung:** CRM-Systeme können automatisierte Workflows für Follow-up-Mails, Erinnerungen oder Angebote erstellen, wodurch Marketing- und Vertriebsprozesse effizienter werden.
- **Vorteil im Kundenkontakt:** Potenzielle Kunden fühlen sich durch automatisierte, aber personalisierte Nachrichten besser betreut, und das Unternehmen kann schnell auf Anfragen oder Aktionen reagieren.

**4. Unterstützung im Kundenservice:**

- **Erklärung:** Ein CRM-System bietet einen umfassenden Überblick über frühere Interaktionen mit dem Kunden, wodurch der Kundenservice gezielt auf bestehende Probleme oder Fragen eingehen kann.
- **Vorteil im Kundenkontakt:** Kunden erleben einen besseren und schnelleren Service, da Servicemitarbeiter über alle relevanten Informationen verfügen und personalisierte Lösungen anbieten können.

**5. Verbesserte Kundenbindung durch Nachverfolgung:**

- **Erklärung:** CRM-Systeme unterstützen die Nachverfolgung von Kundenfeedback und das Monitoring von Kundeninteraktionen nach dem Verkauf.
- **Vorteil im Kundenkontakt:** Durch aktives Feedbackmanagement kann das Unternehmen Probleme schnell lösen und sicherstellen, dass Kunden zufrieden bleiben, was die Loyalität erhöht und zu Folgekäufen führen kann.

**6. Analyse und Optimierung von Marketing-Strategien:**

- **Erklärung:** CRM-Systeme bieten umfassende Berichts- und Analysefunktionen, um den Erfolg von Marketingmaßnahmen zu messen und Anpassungen vorzunehmen.
- **Vorteil im Kundenkontakt:** Das Unternehmen kann besser auf Marktveränderungen reagieren und Kampagnen kontinuierlich optimieren, was die Chancen auf eine erfolgreiche Markteinführung erhöht.

#### Aufgabenteil e (4 Punkte)

**1. Cross-Selling:**

- **Definition:** Cross-Selling bezeichnet die Strategie, einem Kunden ergänzende Produkte oder Dienstleistungen anzubieten, die zu seinem ursprünglichen Kauf passen oder diesen sinnvoll ergänzen.
- **Einsatz im Kontext der Portfolioerweiterung:** Wenn die TechHome Solutions AG neue Lichtsteuerungssysteme in ihr Angebot aufnimmt, könnten sie diese Strategie nutzen, indem sie bestehenden Kunden, die bereits andere Smart-Home-Geräte (z. B. smarte Thermostate oder Sicherheitssysteme) gekauft haben, die neuen Lichtsteuerungen als sinnvolle Ergänzung anbieten. Beispielsweise könnte Kunden, die ein smartes Sicherheitssystem besitzen, ein Paket mit integrierten Bewegungsmeldern und Lichtsteuerungen angeboten werden, um die Sicherheitsfunktionen zu erweitern und die Beleuchtung automatisiert zu steuern.

**2. Up-Selling:**

- **Definition:** Up-Selling ist die Strategie, den Kunden zu überzeugen, ein teureres oder höherwertiges Produkt oder eine Version eines Produkts zu kaufen, das mehr Funktionen oder bessere Leistung bietet als die ursprüngliche Auswahl.
- **Einsatz im Kontext der Portfolioerweiterung:** Bei der Einführung von Produkten mit erweiterten Funktionen kann die TechHome Solutions AG Up-Selling nutzen, indem sie bestehenden Kunden, die einfache smarte Beleuchtungssysteme verwenden, eine verbesserte Version mit erweiterten Funktionen wie Farbwechsel, Dimmfunktionen oder App-gesteuerten Szenen vorschlägt. Ein Beispiel wäre, einem Kunden, der eine einfache smarte Glühbirne gekauft hat, ein Upgrade auf ein System anzubieten, das mit Sprachsteuerung und anpassbaren Lichtprogrammen ausgestattet ist.

#### Aufgabenteil f (3 Punkte)

**1. Interaktive Produktpräsentationen und -demos:**
- **Beschreibung:** Die Website sollte interaktive Präsentationen und Demos enthalten, die die Funktionen der neuen Smart-Home-Produkte anschaulich darstellen. Dies könnte durch 3D-Modelle, Videos oder virtuelle Rundgänge erfolgen, bei denen die Nutzer sehen können, wie die neuen Lichtsteuerungssysteme und andere Produkte in realen Szenarien funktionieren.
- **Vorteil:** Dies spricht visuell orientierte Kunden an und erhöht das Verständnis für die Anwendungsmöglichkeiten der Produkte, was die Kaufentscheidung positiv beeinflusst.

**2. Personalisierte Produktempfehlungen und Bundles:**
- **Beschreibung:** Die Website könnte eine Funktion bieten, die personalisierte Produktempfehlungen basierend auf dem bisherigen Kaufverhalten oder den Präferenzen der Besucher anzeigt. Ebenso könnten spezielle Bundles erstellt werden, die neue Produkte mit bereits beliebten Artikeln kombinieren, um Cross-Selling-Potenziale zu nutzen.
- **Vorteil:** Dies hilft, Kunden gezielt anzusprechen und fördert den Verkauf komplementärer Produkte, indem es zeigt, wie die neuen Produkte das bestehende Smart-Home-System des Kunden ergänzen.

**3. Kundenbewertungen und Erfahrungsberichte:**
- **Beschreibung:** Die Website sollte eine Sektion enthalten, in der frühzeitige Anwender der neuen Produkte ihre Bewertungen und Erfahrungsberichte teilen können. Diese Inhalte könnten durch ein Bewertungssystem und Video-Testimonials ergänzt werden.
- **Vorteil:** Authentische Kundenmeinungen schaffen Vertrauen und liefern potenziellen Käufern wertvolle Einblicke in die tatsächliche Nutzung der Produkte. Positive Bewertungen steigern die Glaubwürdigkeit und fördern den Kauf.

#### Aufgabenteil g (4 Punkte)

**1. Online-Marktplätze (z. B. Amazon, eBay):**
- **Begründung:** Diese Plattformen haben eine enorme Reichweite und ermöglichen es der TechHome Solutions AG, ein großes Publikum anzusprechen, das gezielt nach Smart-Home-Produkten sucht. Die Präsenz auf etablierten Marktplätzen erhöht die Sichtbarkeit und erleichtert den Zugang zu potenziellen Käufern, die eine vertraute Plattform für ihre Einkäufe bevorzugen.

**2. Partnerschaften mit Elektronikfachhändlern (z. B. MediaMarkt, Saturn):**
- **Begründung:** Durch den Vertrieb über bekannte Elektronikketten kann die TechHome Solutions AG von deren bestehendem Kundenstamm und Vertriebsnetz profitieren. Der physische Zugang zu den Produkten in den Läden ermöglicht es den Kunden, sich direkt ein Bild von der Qualität zu machen und sich vor Ort beraten zu lassen, was den Kaufimpuls fördern kann.

**3. Kooperation mit Smart-Home-Installationsdiensten:**
- **Begründung:** Der Vertrieb über spezialisierte Installationsdienste, die auch die Einrichtung von Smart-Home-Lösungen anbieten, spricht Kunden an, die umfassende Lösungen mit Installationsunterstützung bevorzugen. Diese Kooperationen ermöglichen es, Komplettpakete aus Produkt und Service anzubieten und den Verkauf durch eine Rundum-Dienstleistung zu fördern.

**4. Eigener Online-Shop mit exklusiven Angeboten:**
- **Begründung:** Ein gut gestalteter eigener Online-Shop mit exklusiven Angeboten, Bundles und speziellen Rabatten kann die Kundenbindung stärken und höhere Margen ermöglichen. Durch die direkte Kontrolle über den Online-Shop kann die TechHome Solutions AG die Markenerfahrung personalisieren und spezielle Aktionen, wie Vorbestellungen oder limitierte Produkteinführungen, anbieten.

**5. Vertrieb über Bau- und Möbelhäuser (z. B. Bauhaus, IKEA):**
- **Begründung:** Viele Bau- und Möbelhäuser bieten bereits smarte Lösungen an und ziehen Kunden an, die ihr Zuhause renovieren oder modernisieren wollen. Die Einführung der Smart-Home-Produkte in diesem Umfeld ermöglicht es, den Endkunden direkt bei der Hausgestaltung anzusprechen und Impulskäufe zu fördern.

### 4. Aufgabe (26 Punkte)

#### Aufgabenteil a

#### Aufgabenteil aa (4 Punkte)

**Direkte Beschaffung:**
- **Definition:** Bei der direkten Beschaffung handelt es sich um den Einkauf von Gütern und Dienstleistungen, die unmittelbar in die Herstellung eines Produkts oder in die Bereitstellung einer Dienstleistung einfließen. Diese Güter sind integraler Bestandteil des Produktionsprozesses und werden in der Regel regelmäßig in größeren Mengen beschafft.
- **Beispiele:** Rohstoffe (z. B. Holz für Möbelproduktion), Bauteile (z. B. Mikroprozessoren für Elektronikprodukte), Halbfertigprodukte und andere Materialien, die zur Fertigung benötigt werden.
- **Charakteristik:** Eine gut organisierte und zuverlässige direkte Beschaffung ist entscheidend für die Produktionseffizienz und Qualitätssicherung.

**Indirekte Beschaffung:**
- **Definition:** Indirekte Beschaffung bezieht sich auf den Einkauf von Gütern und Dienstleistungen, die nicht direkt in das Endprodukt eingehen, aber für den Betrieb des Unternehmens notwendig sind. Diese Güter und Dienstleistungen unterstützen den Produktionsprozess und den allgemeinen Geschäftsbetrieb.
- **Beispiele:** Büromaterial, Wartungs- und Reparaturdienstleistungen, IT-Dienstleistungen, Reinigungsmittel, Ausstattung für den Arbeitsplatz.
- **Charakteristik:** Die indirekte Beschaffung hat oft einen unregelmäßigeren Bedarf und ist weniger mengenintensiv, aber für den reibungslosen Ablauf des Unternehmensbetriebs unverzichtbar.

#### Aufgabenteil ab (2 Punkte)

**Vorteile der direkten Beschaffung für die TechHome Solutions AG:**
- **Sicherstellung der Produktionsqualität:**
  - Zugang zu hochwertigen Rohstoffen und Komponenten sichert die Qualität der Smart-Home-Produkte.
- **Kosteneffizienz durch Mengenrabatte:**
  - Große Bestellmengen bei wichtigen Bauteilen ermöglichen Rabatte und geringere Kosten pro Einheit.
- **Zuverlässige Lieferketten:**
  - Langfristige Verträge mit Lieferanten gewährleisten eine stabile und planbare Produktion.
- **Produktionskontinuität:**
  - Reduziert das Risiko von Produktionsunterbrechungen durch fehlende Materialien.

**Vorteile der indirekten Beschaffung für die TechHome Solutions AG:**
- **Effizienzsteigerung im Betrieb:**
  - Beschaffung von IT-Dienstleistungen und Büromaterial unterstützt einen reibungslosen Geschäftsbetrieb.
- **Flexibilität und schnelle Anpassungen:**
  - Einfache Anpassung an veränderte Anforderungen oder kurzfristige Bedarfe.
- **Optimierung der Betriebskosten:**
  - Effiziente Beschaffung von Betriebsmitteln kann zu Kosteneinsparungen im Tagesgeschäft führen.

#### Aufgabenteil ac (4 Punkte)

B2B-Marktplatz: Ein B2B-Marktplatz ist eine digitale Plattform, auf der Unternehmen Produkte und Dienstleistungen direkt miteinander handeln können. Im Gegensatz zu B2C-Marktplätzen, die Endverbraucher ansprechen, richtet sich ein B2B-Marktplatz ausschließlich an Geschäftskunden und bietet eine zentrale Anlaufstelle für den Einkauf von Waren und Dienstleistungen, oft mit speziellen Funktionen wie Preisverhandlungen, Mengenrabatten und langfristigen Verträgen.

- **Breite Produkt- und Dienstleistungsauswahl:**
  - Zugang zu einer Vielzahl von Lieferanten und Produkten aus unterschiedlichen Branchen und Regionen.
- **Kostenersparnis:**
  - Möglichkeit, Angebote zu vergleichen und wettbewerbsfähige Preise zu finden, was die Beschaffungskosten senken kann.
- **Schnelle Beschaffungsprozesse:**
  - Vereinfachte und beschleunigte Einkaufsprozesse durch digitale Transaktionen und automatisierte Bestellabwicklung.
- **Transparenz und Vergleichbarkeit:**
  - Bessere Übersicht über Preise, Produktdetails und Lieferbedingungen zur Unterstützung fundierter Entscheidungen.
- **Flexibilität und Verfügbarkeit:**
  - 24/7-Zugang zur Plattform ermöglicht flexible Beschaffung unabhängig von Geschäftszeiten.
- **Netzwerk und Partnerschaften:**
  - Möglichkeit, neue Geschäftskontakte zu knüpfen und langfristige Partnerschaften mit Lieferanten aufzubauen.
- **Reduzierter Verwaltungsaufwand:**
  - Integration in bestehende ERP-Systeme kann den Verwaltungsaufwand verringern und die Effizienz steigern.

#### Aufgabenteil b

#### Aufgabenteil ba (2 Punkte)

**Vorteile der Digitalisierung für die Beschaffung:**
- **Automatisierte Bestellprozesse:** Schnellere und effizientere Bestellungen durch automatisierte Systeme.
- **Echtzeitdaten und Transparenz:** Übersicht über den aktuellen Status von Bestellungen und Lieferungen in Echtzeit.
- **Optimierte Lieferantenkommunikation:** Schnellerer Austausch von Informationen und Dokumenten mit Lieferanten durch digitale Plattformen.
- **Datenanalyse und Prognosen:** Nutzung von Algorithmen zur Vorhersage von Bedarf und Bestellmengen auf Basis historischer Daten.
- **Kostensenkung:** Reduzierung manueller Prozesse spart Zeit und senkt Verwaltungsaufwand und Kosten.

**Optimierung des Bestandsmanagements durch Digitalisierung:**
- **Echtzeit-Überwachung des Lagerbestands:** Transparente Übersicht über den aktuellen Lagerbestand zur Vermeidung von Über- oder Unterbeständen.
- **Bedarfsgesteuerte Nachbestellung:** Automatisierte Nachbestellungen basierend auf definierten Mindestbeständen und Nachfrageprognosen.
- **Just-in-Time-Beschaffung:** Reduzierung der Lagerkosten durch Lieferung von Materialien und Produkten genau dann, wenn sie benötigt werden.
- **Bessere Planung und Variantenmanagement:** Digitalisierung ermöglicht eine genaue Planung und Verwaltung von verschiedenen Produktvarianten, um die Lagerhaltung minimal zu halten.
- **Optimierte Lagerverwaltung:** Effizientere Einlagerung, Auslagerung und Bestandskontrolle durch digitale Systeme und Barcode/RFID-Technologien.

#### Aufgabenteil bb (6 Punkte)

**Unterschiede zwischen auftragsbezogener und vorratsbezogener Beschaffung:**

- **Auftragsbezogene Beschaffung:**
  - **Definition:** Materialien oder Produkte werden erst dann beschafft, wenn ein konkreter Auftrag vorliegt.
  - **Vorteile:** Reduzierte Lagerkosten, da keine Überbestände entstehen; geringeres Risiko der Kapitalbindung; flexibel auf Kundenwünsche anpassbar.
  - **Nachteile:** Längere Lieferzeiten, da die Beschaffung erst nach Auftragseingang erfolgt; potenzielle Lieferengpässe, die die Erfüllung von Aufträgen verzögern könnten.

- **Vorratsbezogene Beschaffung:**
  - **Definition:** Materialien oder Produkte werden auf Lager beschafft, um eine kontinuierliche Verfügbarkeit zu gewährleisten.
  - **Vorteile:** Kurze Lieferzeiten für Kunden, da die Produkte sofort verfügbar sind; besser planbare Produktionsprozesse.
  - **Nachteile:** Höhere Lagerkosten und Kapitalbindung; Risiko von Überbeständen und veralteten Produkten.

**Empfehlung für das Basispaket der TechHome Solutions AG:** Vorratsbezogene Beschaffung

**Begründung:**
- Das Basispaket stellt wahrscheinlich die am häufigsten nachgefragte Produktvariante dar und muss kurzfristig verfügbar sein, um die Kundenzufriedenheit zu gewährleisten.
- Durch eine vorratsbezogene Beschaffung kann die TechHome Solutions AG sicherstellen, dass gängige Basispakete ohne Verzögerung geliefert werden können, was den Kundenservice verbessert und den Absatz steigert.
- Obwohl höhere Lagerkosten anfallen, können diese durch die kontinuierliche Nachfrage kompensiert werden. Zudem ermöglicht eine vorratsbezogene Beschaffung, Produktionsprozesse zu optimieren und Schwankungen in der Nachfrage besser aufzufangen.

#### Aufgabenteil bc (6 Punkte)

**Single-Sourcing:**
- **Beschreibung:** Beschaffung von Waren oder Dienstleistungen von nur einem Lieferanten.
- **Vorteile:** Starke Lieferantenbeziehung, bessere Verhandlungsbedingungen, vereinfachte Kommunikation.
- **Nachteile:** Abhängigkeit von einem Lieferanten, erhöhtes Risiko bei Lieferproblemen.
- **Beispiel:** Ein Hersteller bezieht exklusive elektronische Bauteile nur von einem spezialisierten Zulieferer.

**Multi-Sourcing:**
- **Beschreibung:** Beschaffung von Waren oder Dienstleistungen von mehreren Lieferanten.
- **Vorteile:** Geringere Abhängigkeit von einem Lieferanten, bessere Verhandlungsposition, erhöhte Versorgungssicherheit.
- **Nachteile:** Erhöhter Verwaltungsaufwand, komplexere Logistik.
- **Beispiel:** Ein Unternehmen bezieht Mikroprozessoren von mehreren Anbietern, um Versorgungssicherheit zu gewährleisten.

**Local-Sourcing:**
- **Beschreibung:** Beschaffung von Waren oder Dienstleistungen von Lieferanten in der geografischen Nähe.
- **Vorteile:** Kürzere Lieferzeiten, geringere Transportkosten, Unterstützung der lokalen Wirtschaft.
- **Nachteile:** Möglicherweise höhere Kosten im Vergleich zu internationalen Lieferanten.
- **Beispiel:** Ein Unternehmen kauft Verpackungsmaterialien bei einem regionalen Hersteller, um die Lieferkette zu verkürzen.

**Preferential-Sourcing:**
- **Beschreibung:** Beschaffung bevorzugt von Lieferanten, die bestimmte Kriterien erfüllen (z. B. Nachhaltigkeit, ethische Standards).
- **Vorteile:** Unterstützung von Unternehmenswerten, positive Imagewirkung, Beitrag zu sozialen und ökologischen Zielen.
- **Nachteile:** Möglicherweise höhere Kosten, begrenzte Anzahl qualifizierter Lieferanten.
- **Beispiel:** Ein Unternehmen bezieht Rohstoffe ausschließlich von Lieferanten, die nachweislich nachhaltige Praktiken anwenden.

#### Aufgabenteil bd (2 Punkte)

**1. E-Procurement-Plattformen:**
- **Nutzen:** Automatisierung des gesamten Beschaffungsprozesses, von der Bestellung bis zur Bezahlung.
- **Vorteil für TechHome Solutions AG:** Reduzierte Bearbeitungszeit und Verwaltungskosten, bessere Übersicht und Kontrolle über alle Bestellungen.

**2. Cloud-basierte ERP-Systeme:**
- **Nutzen:** Integrierte Datenplattform zur Verwaltung von Beschaffungs-, Lager- und Bestandsmanagement.
- **Vorteil für TechHome Solutions AG:** Echtzeit-Überwachung der Lagerbestände, effiziente Planung und Optimierung der Lieferketten.

**3. E-Auctions (elektronische Auktionen):**
- **Nutzen:** Online-Plattformen zur Durchführung von Auktionen zur Ermittlung der besten Preise von Lieferanten.
- **Vorteil für TechHome Solutions AG:** Kosteneinsparungen durch Wettbewerb unter Lieferanten, bessere Verhandlungsposition.

**4. Künstliche Intelligenz (KI) und Machine Learning:**
- **Nutzen:** Analyse von großen Datenmengen zur Vorhersage von Nachfrageschwankungen und Optimierung der Beschaffung.
- **Vorteil für TechHome Solutions AG:** Verbesserte Bedarfsvorhersagen und proaktive Beschaffungsstrategien, Minimierung von Engpässen.

**5. Blockchain-Technologie:**
- **Nutzen:** Sicherstellung der Transparenz und Rückverfolgbarkeit der Lieferkette.
- **Vorteil für TechHome Solutions AG:** Erhöhte Sicherheit und Vermeidung von Betrug, Nachverfolgbarkeit der Herkunft und Qualität der eingekauften Materialien.

**6. IoT (Internet of Things):**
- **Nutzen:** Automatisierte Erfassung von Lagerbeständen und Bestellungen durch smarte Sensoren.
- **Vorteil für TechHome Solutions AG:** Automatisierte Nachbestellung bei niedrigem Lagerbestand, Echtzeit-Daten für effizienteres Bestandsmanagement.

**7. E-Signaturen und digitale Vertragsmanagementsysteme:**
- **Nutzen:** Ermöglicht rechtssichere digitale Signaturen und Verwaltung von Verträgen online.
- **Vorteil für TechHome Solutions AG:** Beschleunigte Vertragsabschlüsse und weniger Papieraufwand, verbesserte Nachverfolgbarkeit von Vertragsänderungen.

**8. Mobile Beschaffungs-Apps:**
- **Nutzen:** Zugriff auf Beschaffungsplattformen und Genehmigungsprozesse von unterwegs.
- **Vorteil für TechHome Solutions AG:** Höhere Flexibilität und schnelle Entscheidungen, verbesserte Effizienz für das Beschaffungsteam.

Die folgenden Begriffe wurden in der bisherigen Antwort noch nicht erklärt:

**9. Vergleichsportale:**
- **Nutzen:** Plattformen zur Analyse und zum Vergleich von Preisen und Leistungen verschiedener Lieferanten.
- **Vorteil für TechHome Solutions AG:** Ermöglicht eine schnelle und effiziente Auswahl des besten Angebots, Optimierung der Einkaufspreise und bessere Transparenz bei der Lieferantenauswahl.

**10. EDI (Electronic Data Interchange):**
- **Nutzen:** Standardisiertes, elektronisches Format für den Austausch von Geschäftsdokumenten zwischen Unternehmen.
- **Vorteil für TechHome Solutions AG:** Automatisierte und fehlerfreie Übermittlung von Bestellungen, Rechnungen und anderen Dokumenten, was den Verwaltungsaufwand und die Bearbeitungszeiten erheblich reduziert.

**11. EBANF (Elektronischer Bestellanforderungsschein):**
- **Nutzen:** Digitale Übermittlung und Genehmigung von Bestellanforderungen innerhalb eines Unternehmens.
- **Vorteil für TechHome Solutions AG:** Erhöht die Effizienz der internen Freigabeprozesse und reduziert den Papierverbrauch durch digitale Genehmigungsworkflows.

**12. E-Kanban:**
- **Nutzen:** Digitales Kanban-System zur Verwaltung und Automatisierung der Nachbestellung und Lagerauffüllung.
- **Vorteil für TechHome Solutions AG:** Echtzeitüberwachung des Materialflusses und automatische Bestellvorgänge bei Bedarf, was eine Just-in-Time-Beschaffung unterstützt und Lagerkosten reduziert.

**13. E-Invoicing (Elektronische Rechnungsstellung):**
- **Nutzen:** Elektronische Erstellung und Übermittlung von Rechnungen an Kunden oder Lieferanten.
- **Vorteil für TechHome Solutions AG:** Schnelle und kostengünstige Rechnungsbearbeitung, Reduzierung von Fehlern und verbesserte Nachverfolgbarkeit der Zahlungen.

{%
   include-markdown "inhalte/lizenzhinweis.md"
   start="<!--include-start-->"
   end="<!--include-end-->"
%}