# Besluiten

De besluiten van dit experiment, genomen en open, in de vorm die elk project in `decisions.md` krijgt.

Vorm van een regel:
- **Genomen**: nummer, datum, wie besloot; het besluit; waarom; de bron (gesprek, commit).
- **Open**: nummer, de vraag; bij wie de bal ligt; wat er al bekend is (gemeten feit) en het advies van de assistent (aanname, tot Tim streept).
- Er komt alleen bij. Wordt een besluit herzien, dan krijgt het een nieuwe regel die naar de oude verwijst; de oude blijft staan.

## Genomen

- **B01 · 06-10 · Tim.** Een projectassistent die zelf werk aflevert in plaats van op Tim te wachten. Eerst Melk en Meer, daarna Visie op Noordeloos, JUMP en La Grange. *Waarom:* de huidige projectmanager mag alleen lijsten bijhouden, wordt wakker met "is er nieuwe mail?" en legt de bal overal bij Tim. *Bron:* gesprek 06-10, 6cb7e9e.
- **B02 · 06-10 · Tim.** Het is een projectassistent, geen projectmanager: hij ondersteunt Tim als persoon. *Bron:* gesprek 06-10.
- **B03 · 06-10 · Tim.** Maken mag altijd; versturen nooit zonder Tim. Mist er een besluit, dan schrijft hij door op zijn eigen advies en markeert hij dat; Tim streept. *Waarom:* zonder ruimte om af te maken blijft hij wachten. *Bron:* 6cb7e9e.
- **B04 · 06-10 · Tim.** Eén keer per dag één bericht: dit ligt klaar. *Bron:* 6cb7e9e.
- **B05 · 06-10 · Tim.** Chat en Claude Code werken samen via `handoff/` in deze repo. *Bron:* f17d8b8.
- **B06 · 06-10 · Tim.** Verzamelen en routeren hoort bij de data-collector (pilot-experiment-2). De assistent haalt de data-items met zijn projectlabel uit de postbus. *Waarom:* één verzamelaar voor alle projecten. *Bron:* 7654b4b.
- **B07 · 06-10 · Tim.** Elke ronde begint bij een trigger (heette eerst wekker): een nieuw data-item, of elke dag terug vanaf de mijlpaal. *Waarom:* de dagronde maakt hem proactief, ook als er geen post is. *Bron:* 06fc7b1, 48c4582.
- **B08 · 06-10 · Tim.** Input links, analyse in het midden, output rechts: dezelfde onderdelen in een nieuwe versie, plus Klaar voor Tim. *Bron:* 2193c0e.
- **B09 · 06-10 · Tim.** De analyse stelt vier vragen: wat verandert, verschil met het plan, wat blijft uit, wat maak ik zelf af. *Waarom:* de vierde vraag maakt hem proactief. *Bron:* 06fc7b1.
- **B10 · 06-10 · Tim.** Het dashboard heeft een meter: wat lag klaar, wat deed Tim ermee. *Bron:* 06fc7b1.
- **B11 · 06-10 · Tim.** Eén logboek voor alles, één regel per ronde, vijf vakjes (trigger, gelezen, gezien, bijgewerkt, klaargelegd). Er komt alleen bij; "niets gevonden" is ook een regel; het verwijst en kopieert niet. *Waarom:* de volgende ronde begint bij de laatste regel. *Bron:* 65284af, b73c457.
- **B12 · 06-10 · Tim.** De projectassistent staat op GitHub; de dossiers blijven op Desk, buiten hem. Hij leest ze en werkt ze bij (gestippeld in beide kolommen). *Bron:* 15141bc, a089584.
- **B13 · 06-10 · Tim.** To-do's zijn afspraken dat anderen iets doen: wie doet wat, wanneer. Beloftes zijn de to-do's van anderen. *Bron:* 5a5d37e, 011941a.
- **B14 · 06-10 · Tim.** Tims eigen to-do's staan in Todoist, een buitenbron net boven de dossiers. De assistent leest daar de to-do's van dit project en past ze daar aan; een wijziging in Todoist komt als data-item via de post binnen. *Bron:* 011941a.
- **B15 · 06-10 · Tim.** Het blokje Stand heet Besluiten, genomen en open. *Waarom:* met de beloftes bij de to-do's en de dossiers buiten bleven alleen de besluiten over. *Bron:* bde27c1.
- **B16 · 06-10 · Tim.** Eén map met projecten, elk project één repo; elk blokje een map of bestand; één ronde is één commit, de diff is de wijziging. *Bron:* b73c457.
- **B17 · 06-10 · Tim.** Geen pull requests. De snelle lijsten wijzigt hij direct; plan en programmavoorstel pas na Tims ja; goal en foundation zijn alleen van Tim. *Bron:* b73c457.
- **B18 · 06-10 · Tim.** Het dashboard is een viewer op alle onderdelen, een HTML-pagina die de repo leest; Tim hoeft GitHub niet in. *Waarom:* Tim wil kunnen zien wat er precies gebeurt. *Bron:* 8178ac2.
- **B19 · 06-10 · Tim.** Elke wijziging van de tekening verschijnt ook als artifact. *Bron:* gesprek 06-10.
- **B20 · 07-10 · Tim.** Zes spelregels uit Tims tekst "Inrichting op GitHub": één schrijver per bestand met controle; inhoud en machinerie gescheiden; een voorstel is een bestand met een status; het protocol staat in de repo; Out there wekelijks met hooguit één voorstel; twee mensen bij de knoppen. *Bron:* 5159766.
- **B21 · 07-10 · Tim.** De projectenmap: de engine één keer (protocol, scripts, viewer), per project een repo met alleen inhoud en een `steering.md` met de projectsturing; de trigger is een wekker buiten de repo. *Bron:* 451a32d.
- **B22 · 07-10 · Tim.** In de engine een template om een nieuw project aan te maken, en per onderdeel een skill die zegt hoe het gevuld wordt. *Waarom:* elk project houdt dezelfde vorm, en de controle kan die vorm nakijken. *Bron:* gesprek 07-10, 451a32d.
- **B23 · 06-10 · Tim.** De Vercel-storingsmail hoort bij Melk en Meer: een signaal dat de site eruit ligt, geen ruis. Lege titels zijn Tims eigen mails zonder onderwerp en blijven leeg. *Bron:* gesprek 06-10 (gaat over de postbus van Melk en Meer).

## Open

- **O01 · Mag Jev in de data-collector meekijken?** *Bal bij:* Tim. *Bekend:* in de proef van pilot-experiment-2 kiest Jev al mee (gemeten 07-10).
- **O02 · Bevat de postbus de inhoud of alleen een verwijzing?** *Bal bij:* Tim. *Bekend:* in de proef bevat een data-item beide, `inhoud` en `verwijzing` (collector.ts).
- **O03 · Wie leegt de twijfelbak?** *Bal bij:* Tim.
- **O04 · Krijgt geld een eigen lijst, of is het een draad?** *Bal bij:* Tim.
- **O05 · Waar komen Tims eigen handelingen (strepen, versturen, corrigeren)?** *Bal bij:* Tim. *Advies:* zijn antwoord in het voorstelbestand (B20, regel 3) en een vakje in het logboek.
- **O06 · Schrijft hij in de dossiers op Desk, of legt hij een bijwerking klaar?** *Bal bij:* Tim.
- **O07 · De namen van de mappen in de repo.** *Bal bij:* Tim. *Bekend:* de projectenmap in de README gebruikt werknamen.
- **O08 · Is de engine een eigen repo of een map naast de projecten?** *Bal bij:* Tim. *Advies:* een eigen repo, met een versie per project.
- **O09 · Draait de wekker op de Mini of als routine in claude.ai?** *Bal bij:* Tim.
- **O10 · Leest hij Foundation altijd of als nodig?** *Bal bij:* Tim. *Bekend:* de tekening zegt nu altijd.
- **O11 · Blijft het woord "draden"?** *Bal bij:* Tim. *Bekend:* de README noemt het nog bij de lijsten van het project.
- **O12 · Wie is de reserve bij de knoppen (B20, regel 6)?** *Bal bij:* Tim.
- **O13 · Proef voor La Grange.** *Bal bij:* Tim. *Bekend:* dossier op Desk bijgewerkt tot 28-07; 3 items in de proefpostbus; oude mail in te halen tot ongeveer mei 2026; WhatsApp nog niet (gemeten 07-10). *Advies:* eerst één ronde met de hand op een kopie.
- **O14 · De analyse van "Inrichting op GitHub" afmaken: wat bij hen beter kan, wat wij al beter doen.** *Bal bij:* Tim.
- **O15 · Volgende stap: de stand van Melk en Meer in deze vorm uitschrijven.** *Bal bij:* assistent, na Tims ja.
