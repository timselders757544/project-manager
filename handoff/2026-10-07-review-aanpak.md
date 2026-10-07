# Handoff 2026-10-07: review van de aanpak

Status: verwerkt

Verwerkt op 2026-10-07: de adviezen bij O04, O09 en O12 en het nieuwe advies bij O15 staan in `decisions.md`, gemarkeerd als "(chat, 07-10)". O06 was al besloten als B29 (eerst een voorstel, trede 1, zo snel mogelijk naar trede 3), in lijn met het advies hier. O16 tot en met O20 zijn toegevoegd als open vragen; de eerdere O16 van Claude Code (hoe hij in een dossier schrijft) heet nu O21. In de README heet "De stand" nu "Lijsten van het project", omdat het kopje Besluiten al bestaat en naar `decisions.md` wijst. "Stand" bij de snelle lijsten werd "besluiten", "draden" verwijst naar O11, en `notes.md` staat in de projectmap voor "Voor de AI zelf". Er is geen besluit genomen. `goal.md`, `foundation/` en `steering.md` zijn niet aangeraakt.

Gelezen: de versie van 07-10 07:16 (README, decisions.md, tekening.svg, tot en met ae3fab4). Daarna kwamen B24 tot en met B28 binnen; O03 is met B26 besloten en valt hier weg.
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
7. **Niet elke open vraag heeft een advies**, terwijl B03 dat vraagt. Hieronder staan ze, voor O04, O06, O09 en O12.

## Adviezen bij de bestaande open vragen
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
1. Zet de adviezen bij O04, O06, O09 en O12 in `decisions.md`, gemarkeerd als advies van de assistent.
2. Voeg O16 tot en met O20 toe aan de open vragen en vervang het advies bij O15. Neem zelf geen besluit: dat doet Tim.
3. Werk de README bij volgens punt 5: het kopje Besluiten, "draden" alleen laten staan zolang O11 open is (met een verwijzing), en een plek in de projectmap voor "Voor de AI zelf".
4. Raak `goal.md`, `foundation/` en `steering.md` niet aan.
5. Zet bovenaan deze handoff: Verwerkt op JJJJ-MM-DD, met wat er gedaan is.
