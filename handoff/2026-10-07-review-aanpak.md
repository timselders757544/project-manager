# Handoff 2026-10-07: review van de aanpak

Status: open

Gelezen: de versie van 07-10 07:16 (README, decisions.md, tekening.svg, tot en met ae3fab4).
Alles hieronder is advies van chat, een aanname tot Tim streept (B03).

## Wat beter is geworden
- Hij stopt niet meer bij "geen nieuwe mail": de dagronde terug vanaf de mijlpaal en de vierde vraag ("wat maak ik zelf af?") maken hem proactief (B07, B09).
- Alles is na te gaan: één ronde is één commit en één logboekregel, ook als er niets is (B11, B16).
- Een nee blijft staan met de reden, dus hetzelfde voorstel komt niet terug (B20, regel 3).
- Het schaalt: de engine staat er één keer, met template en skills (B21, B22).
- De rollen zijn helder: één schrijver per bestand met `check.sh`; Todoist voor Tims to-do's, het project voor die van anderen.

## Wat beter kan
1. **De belangrijkste belofte heeft geen mechanisme.** Het dagbericht (B04) en het versturen na Tims ja (B03) staan nergens in de engine: geen kanaal, geen script, geen regel in `steering.md`. Zie O16 en O17.
2. **23 besluiten, nog geen ronde.** Het advies bij O13 (eerst één ronde met de hand) geldt ook voor Melk en Meer, vóór de engine gebouwd wordt. Zie O15.
3. **Eén schrijver botst met de buitenbronnen.** De assistent werkt de dossiers op Desk bij (B12) en past Tims to-do's in Todoist aan (B14). Dat zijn Tims bestanden en `check.sh` ziet ze niet. Zie O06 en O18.
4. **De bal kan terug bij Tim komen.** Plan en programmavoorstel wachten op Tims ja. Liggen er elke dag vijf voorstellen klaar, dan zijn we terug bij af. Zie O19.
5. **De README loopt achter op de besluiten.** Het kopje heet nog "De stand" (B15 noemt het Besluiten), er staat nog "draden" (O11), en "Voor de AI zelf" (correcties van Tim, wat we niet weten) heeft geen bestand in de projectmap. "Bron, feit of aanname, bal bij elke regel" is alleen uitgewerkt voor besluiten, niet voor to-do's en mensen.
6. **Er is geen meetlat.** De meter (B10) laat zien wat er gebeurt, niet wanneer het experiment geslaagd is. Zie O20.
7. **Niet elke open vraag heeft een advies**, terwijl B03 dat vraagt. Hieronder staan ze.

## Adviezen bij de bestaande open vragen
- **O03 · Wie leegt de twijfelbak?** *Advies:* niemand apart. Elk item uit de twijfelbak komt als één regel in het dagbericht: "hoort dit bij Melk en Meer, La Grange, of nergens?". Tims antwoord wordt een vaste regel in de data-collector, zodat de twijfelbak vanzelf kleiner wordt.
- **O04 · Krijgt geld een eigen lijst?** *Advies:* nu niet. Geld is een kenmerk op besluiten en to-do's, waarop de viewer kan filteren. Een eigen lijst pas als het programmavoorstel een begroting krijgt.
- **O06 · Schrijft hij in de dossiers op Desk?** *Advies:* nee, hij legt een bijwerking klaar als voorstel in `proposals/`. Dan blijft "één schrijver per bestand" ook buiten GitHub waar.
- **O09 · De wekker op de Mini of als routine in claude.ai?** *Advies:* op de Mini. Aanname, te controleren: daar zijn de data-collector en Desk bereikbaar, en een routine in de cloud kan niet vanzelf bij lokale bestanden.
- **O12 · Wie is de reserve bij de knoppen?** *Advies:* iemand die Melk en Meer al kent. Minimaal nodig: leesrecht op de repo en de viewer, en één regel uitleg hoe je de wekker uitzet.

## Nieuwe open vragen
- **O16 · Langs welk kanaal komt het dagbericht?** *Bal bij:* Tim. *Advies:* de laatste ronde van de dag bouwt de viewer en stuurt één korte melding met een link (mail of pushbericht). Het kanaal staat in `steering.md`, het script in `engine/bin/`.
- **O17 · Wie verstuurt na Tims ja?** *Bal bij:* Tim. *Advies:* de volgende ronde, als status ja en het voorstel een mail is, met Tim als afzender en in het logboek onder Klaargelegd. Tot dat gebouwd is: Tim verstuurt zelf vanuit het concept.
- **O18 · Herziening van B14: past hij Tims to-do's in Todoist zelf aan?** *Bal bij:* Tim. *Advies:* nee, hij legt de wijziging klaar als voorstel, net als bij O06. B14 blijft staan; bij een ja komt er een nieuw besluit dat ernaar verwijst.
- **O19 · Een plafond voor open voorstellen?** *Bal bij:* Tim. *Advies:* hooguit drie open voorstellen tegelijk die Tims ja nodig hebben. Wordt het plafond vaak geraakt, dan pakt hij te weinig zelf op; de meter houdt dat bij.
- **O20 · Wanneer is het experiment geslaagd?** *Bal bij:* Tim. *Advies:* na drie weken Melk en Meer gaat meer dan de helft van de voorstellen ongewijzigd door, en Tim besteedt minder tijd aan het project dan nu.

## Aanpassing van O15
- **O15 · Volgende stap.** *Advies:* eerst één ronde voor Melk en Meer met de hand: één trigger, de vier vragen, één logboekregel, één voorstel. Pas daarna de engine bouwen, met wat die ronde liet zien.

## Voor Claude Code
1. Zet de adviezen bij O03, O04, O06, O09 en O12 in `decisions.md`, gemarkeerd als advies van de assistent.
2. Voeg O16 tot en met O20 toe aan de open vragen en vervang het advies bij O15. Neem zelf geen besluit: dat doet Tim.
3. Werk de README bij volgens punt 5: het kopje Besluiten, "draden" alleen laten staan zolang O11 open is (met een verwijzing), en een plek in de projectmap voor "Voor de AI zelf".
4. Raak `goal.md`, `foundation/` en `steering.md` niet aan.
5. Zet bovenaan deze handoff: Verwerkt op JJJJ-MM-DD, met wat er gedaan is.
