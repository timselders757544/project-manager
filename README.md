# Project Manager

Experiment: een AI-projectassistent die zelf werk aflevert in plaats van op Tim te wachten.
Eerst Melk en Meer; daarna Visie op Noordeloos, JUMP en La Grange.

## Waarom de huidige niets oplevert
- Hij mag alleen lijsten bijhouden; voor al het andere vraagt hij toestemming.
- Zijn doelen kan alleen Tim halen.
- Hij wordt wakker met "is er nieuwe mail?". Meestal is het antwoord nee, en dan stopt hij.
- De bal ligt overal bij Tim.

## Wat hem proactief maakt
Een trigger, een product dat bij die trigger hoort, en ruimte om het zonder Tim af te maken.
Elke ronde begint bij een trigger: een nieuw data-item, of elke dag terug vanaf de mijlpaal.
- Maken mag altijd; versturen nooit zonder Tim.
- Mist er een besluit, dan schrijft hij op zijn eigen advies door en markeert hij dat. Tim streept.
- Eén keer per dag één bericht: dit ligt klaar.

## Opbouw
![Tims tekening van de projectassistent](tekening.svg)

1. **Verzamelen en routeren**: de data-collector haalt alle bronnen op en legt elk stuk in de postbus van het project. Eerst vaste regels, daarna Jev, de rest naar een twijfelbak. Dit bouwt pilot-experiment-2.
2. **Analyse**: bij elk stuk de vraag "wat verandert hierdoor?". Daarnaast elke dag een ronde: wat blijft uit, wat loopt achter op het plan?
3. **Uitkomst**:
   - de to-do's: afspraken dat anderen iets doen, wie doet wat en wanneer (een herinnering staat eerst als concept klaar); Tims eigen to-do's staan in Todoist, daar leest hij ze en daar past hij ze aan;
   - het plan met mijlpalen;
   - een nieuwe versie van het programmavoorstel;
   - een dashboard dat eerst laat zien wat er klaarligt.

## De stand
- **Lijsten van het project**:
  - de draden;
  - het doel en het plan;
  - de besluiten, open en genomen, met de reden (dit blokje heette eerst Stand; beloftes van anderen zijn to-do's);
  - het programmavoorstel;
  - de mensen en partijen, met wat ze willen en hoe hun naam ook geschreven of verstaan wordt.
- **Bij elke regel**: bron en datum, feit of aanname, en bij wie de bal ligt.
- **Voor de AI zelf**: zijn eigen logboek, wat we niet weten, de spelregels en de correcties van Tim.

## Het logboek
Eén logboek voor alles, één regel per ronde, in vijf vaste vakjes: 1 trigger (waardoor), 2 gelezen (welke data-items), 3 gezien (de vier vragen: wat verandert, verschil met plan, wat blijft uit, wat maak ik zelf af), 4 bijgewerkt (welke regel waar), 5 klaargelegd (wat, voor Tim).
Er komt alleen bij; "niets gevonden" is ook een regel. Het verwijst naar de lijsten en kopieert niet. De volgende ronde begint bij de laatste regel.

## Op GitHub
- Eén map met projecten; elk project is één repo. Geen repo per onderdeel.
- Elk blokje van de tekening is een map of bestand in die repo.
- Eén ronde is één commit; de diff is wat de analyse veranderde.
- Geen pull requests. De snelle lijsten (stand, to-do's, mensen, logboek) wijzigt hij direct. Voor het plan en het programmavoorstel legt hij een voorstel klaar; de wijziging komt pas na Tims ja. Goal en foundation zijn alleen van Tim.
- Het dashboard is een viewer op alle onderdelen, een HTML-pagina die de repo leest; Tim hoeft GitHub niet in.
- Buiten de repo: de postbus (data-items liggen bij de data-collector), de dossiers (blijven op Desk; hij leest ze en werkt ze bij) en Tims to-do's (in Todoist; een wijziging daar komt als data-item via de post binnen).

## Spelregels
Overgenomen uit Tims tekst "Inrichting op GitHub" van 06-10-2026.
1. **Eén schrijver per bestand.** Per bestand staat vast wie erin schrijft (de assistent, Tim). Een controle na elke ronde weigert als de assistent een bestand raakt dat niet van hem is, zoals goal en foundation.
2. **Inhoud en machinerie gescheiden.** De project-repo bevat alleen inhoud: plan, besluiten, logboek. Protocol, viewer-bouwer en controles staan één keer apart (de engine); elk project noemt welke versie hij gebruikt.
3. **Een voorstel is een bestand met een status.** Wat klaarligt voor Tim is één bestand per voorstel, met de precieze wijziging en een status: open, ja, pas aan, nee, doorgevoerd. Tims antwoord wordt erin geschreven; een nee blijft staan met de reden, zodat het niet terugkomt. Bij ja verandert de volgende ronde het echte bestand en noemt de commit het voorstel en wie besloot.
4. **Het protocol staat in de repo.** De trigger zegt alleen: volg het protocol. Alles wat een ronde moet doen staat in dat ene bestand; de werkwijze veranderen is een bestand veranderen, met geschiedenis.
5. **Out there heeft een weekritme.** Eén keer per week naar buiten kijken, begrensd, met hooguit één voorstel.
6. **Twee mensen bij de knoppen.** Alles hangt nu aan Tim; er is altijd een reserve die erbij kan. Dit is een afspraak, geen bouwpunt.

## Open
- Mag Jev in de data-collector meekijken?
- Bevat de postbus de inhoud of alleen een verwijzing?
- Wie leegt de twijfelbak?
- Krijgt geld een eigen lijst, of is het een draad?
- Waar Tims eigen handelingen (strepen, versturen, corrigeren) in het logboek komen.
- Mag hij in de dossiers op Desk schrijven, of legt hij een bijwerking klaar?
- De namen van de mappen in de repo.
- Leest hij Foundation altijd of als nodig?
- Volgende stap: de stand van Melk en Meer in deze vorm uitschrijven.
