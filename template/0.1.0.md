# NeRDS Template v0.1.0

## Introductie

Dit document beschrijft de template voor NeRDS (Nederlandse Richtlijnen Digitale Systemen) richtlijnen. Deze template biedt een gestandaardiseerde structuur voor het documenteren van richtlijnen voor digitale systemen binnen de Nederlandse overheid.

## Specificatie van de Template

```yaml
schema_version: "0.1.0"
titel: "{richtlijn_titel}"                              # Verplicht. Voorbeeld: "Toegankelijkheid van Overheidswebsites"
beschrijving: "{richtlijn_beschrijving}"                # Verplicht. Voorbeeld: "Deze richtlijn beschrijft hoe overheidswebsites toegankelijk moeten zijn volgens WCAG 2.1 niveau AA standaarden."

rationale:
  waarom: "{rationale_waarom}"                          # Optioneel. Voorbeeld: "Toegankelijke websites zorgen ervoor dat alle burgers, ongeacht hun beperkingen, gelijke toegang hebben tot overheidsinformatie en -diensten."
  beoogd_effect: "{rationale_beoogd_effect}"            # Optioneel. Voorbeeld: "Verhoogde inclusiviteit en naleving van wettelijke verplichtingen."
  risicos:                                              # Optioneel.
    - "{risico_1}"                                      # Voorbeeld: "Uitsluiting van burgers met een beperking"
    - "{risico_2}"                                      # Voorbeeld: "Juridische risico's door niet-naleving van wetgeving"

doelgroep:
  - doelgroep: "{doelgroep_naam}"                      # Voorbeeld: "Frontend ontwikkelaars"
    handelingen: "{handelingen_beschrijving}"          # Optioneel. Voorbeeld: "Implementeer ARIA-labels en zorg voor keyboard navigatie"

implementatie:
  methoden_technieken:                                  # Optioneel.
    - naam: "{methode_naam}"                            # Voorbeeld: "Semantische HTML"
      beschrijving: "{methode_beschrijving}"            # Voorbeeld: "Gebruik correcte HTML elementen voor hun bedoelde doel"
      verplicht: {true/false}                           # Voorbeeld: true
  tools:                                                # Optioneel.
    - naam: "{tool_naam}"                               # Voorbeeld: "axe DevTools"
      type: "{tool_type}"                               # Voorbeeld: "Browser extensie voor toegankelijkheidscontrole"
      beschrijving: "{tool_beschrijving}"               # Voorbeeld: "Automatische detectie van toegankelijkheidsproblemen"
      verplicht: {true/false}                           # Voorbeeld: false
      url: "{tool_url}"                                 # Voorbeeld: "https://www.deque.com/axe/"
  subrichtlijnen:                                       # Optioneel.
    - titel: "{subrichtlijn_titel}"                     # Voorbeeld: "Kleurcontrast"
      omschrijving: "{subrichtlijn_omschrijving}"       # Voorbeeld: "Richtlijnen voor voldoende contrast tussen tekst en achtergrond"
      link: "{subrichtlijn_link}"                       # Voorbeeld: "./subrichtlijnen/kleurcontrast.yaml"

succescriteria:                                         # Optioneel.
  - criterium: "{succes_criterium}"                     # Voorbeeld: "Alle afbeeldingen hebben alt-tekst"
    voldaan: {true/false}                               # Voorbeeld: true

toepassingsvoorwaarde:
    - "{toepassingsvoorwaarde_1}"                       # Voorbeeld: "Van toepassing op alle publiek toegankelijke overheidswebsites"
    - "{toepassingsvoorwaarde_2}"                       # Voorbeeld: "Verplicht volgens het Tijdelijk besluit digitale toegankelijkheid overheid"

bronnen:
  wetten:                                               # Optioneel.
    - naam: "{wet_naam}"                                # Voorbeeld: "Tijdelijk besluit digitale toegankelijkheid overheid"
      url: "{wet_url}"                                  # Voorbeeld: "https://wetten.overheid.nl/BWBR0040936"
  beleid:                                               # Optioneel.
    - naam: "{beleid_naam}"                             # Voorbeeld: "Digitale Inclusie Agenda"
      url: "{beleid_url}"                               # Voorbeeld: "https://www.digitaleoverheid.nl"
  standaarden:                                          # Optioneel.
    - naam: "{standaard_naam}"                          # Voorbeeld: "WCAG 2.1"
      url: "{standaard_url}"                            # Voorbeeld: "https://www.w3.org/TR/WCAG21/"
  communities:                                          # Optioneel.
    - naam: "{community_naam}"                          # Voorbeeld: "Toegankelijkheid Community NL"
      url: "{community_url}"                            # Voorbeeld: "https://www.toegankelijkheidsverklaring.nl"
  literatuur:                                           # Optioneel.
    - titel: "{literatuur_titel}"                       # Voorbeeld: "Inclusive Design Patterns"
      auteurs:                                          # Optioneel.
        - "{auteur_1}"                                  # Voorbeeld: "Heydon Pickering"
      url: "{literatuur_url}"                           # Optioneel. Voorbeeld: "https://shop.smashingmagazine.com/products/inclusive-design-patterns"
      doi: "{doi}"                                      # Optioneel. Voorbeeld: "10.1234/example"
  developer_overheid:                                   # Optioneel.
    - titel: "{artikel_titel}"                          # Voorbeeld: "Toegankelijkheid testen met automatische tools"
      type: "{artikel_type}"                            # Voorbeeld: "blog" of "kennisbank"
      url: "{artikel_url}"                              # Voorbeeld: "https://developer.overheid.nl/blog/toegankelijkheid"

gerelateerde_richtlijnen:                               # Optioneel.
  - titel: "{gerelateerde_richtlijn_titel}"             # Voorbeeld: "Gebruiksvriendelijkheid van Overheidswebsites"
    relatie: "{relatie_beschrijving}"                   # Voorbeeld: "Toegankelijkheid en gebruiksvriendelijkheid versterken elkaar"
    link: "{gerelateerde_richtlijn_link}"               # Voorbeeld: "./gebruiksvriendelijkheid.yaml"
```

## Voorbeeld YAML Structuur

```yaml
schema_version: "0.1.0"
titel: "Toegankelijkheid van Overheidswebsites"

beschrijving:
  wat: "Deze richtlijn beschrijft hoe overheidswebsites toegankelijk moeten zijn volgens WCAG 2.1 niveau AA standaarden. Toegankelijkheid betekent dat websites bruikbaar zijn voor alle burgers, inclusief mensen met visuele, auditieve, motorische of cognitieve beperkingen."

rationale:
  waarom: "Toegankelijke websites zorgen ervoor dat alle burgers, ongeacht hun beperkingen, gelijke toegang hebben tot overheidsinformatie en -diensten. Dit is een fundamenteel recht en wettelijke verplichting."
  beoogd_effect: "Verhoogde inclusiviteit, betere gebruikerservaring voor iedereen, en naleving van wettelijke verplichtingen. Toegankelijke websites zijn ook beter vindbaar in zoekmachines en werken beter op verschillende apparaten."
  risicos:
    - "Uitsluiting van burgers met een beperking van essentiële overheidsdiensten"
    - "Juridische risico's door niet-naleving van het Tijdelijk besluit digitale toegankelijkheid overheid"
    - "Reputatieschade voor de overheidsorganisatie"
    - "Hogere kosten door later moeten aanpassen van de website"

doelgroep:
  primaire_doelgroep:
    - "Frontend ontwikkelaars"
    - "UX/UI designers"
    - "Content managers"
    - "Product owners"
  handelingsperspectief:
    - doelgroep: "Frontend ontwikkelaars"
      handelingen: "Implementeer semantische HTML, ARIA-labels, en zorg voor keyboard navigatie. Test regelmatig met toegankelijkheidstools en screenreaders."
    - doelgroep: "UX/UI designers"
      handelingen: "Ontwerp met voldoende kleurcontrast, duidelijke focusindicatoren, en zorg voor logische tab-volgorde. Houd rekening met verschillende schermformaten en hulpmiddelen."
    - doelgroep: "Content managers"
      handelingen: "Schrijf duidelijke alt-teksten voor afbeeldingen, gebruik koppen op de juiste manier, en zorg voor begrijpelijke linkteksten."
    - doelgroep: "Product owners"
      handelingen: "Neem toegankelijkheidseisen op in de Definition of Done en zorg voor budget voor toegankelijkheidstesten en -verbeteringen."

implementatie:
  methoden_technieken:
    - naam: "Semantische HTML"
      beschrijving: "Gebruik correcte HTML elementen voor hun bedoelde doel (bijv. <button> voor knoppen, <nav> voor navigatie, <main> voor hoofdinhoud)"
      verplicht: true
    - naam: "ARIA attributen"
      beschrijving: "Gebruik ARIA (Accessible Rich Internet Applications) attributen om extra context te geven aan dynamische content en complexe widgets"
      verplicht: true
    - naam: "Keyboard navigatie"
      beschrijving: "Zorg dat alle functionaliteit beschikbaar is via het toetsenbord, met logische tab-volgorde en zichtbare focus-indicatoren"
      verplicht: true
    - naam: "Responsief ontwerp"
      beschrijving: "Ontwerp websites die goed werken op verschillende schermformaten en met verschillende zoom-niveaus (tot 200%)"
      verplicht: true
  tools:
    - naam: "axe DevTools"
      type: "Browser extensie"
      beschrijving: "Automatische detectie van toegankelijkheidsproblemen tijdens ontwikkeling"
      verplicht: false
      url: "https://www.deque.com/axe/"
    - naam: "WAVE"
      type: "Online validatietool"
      beschrijving: "Webgebaseerde tool voor het evalueren van toegankelijkheid van webpagina's"
      verplicht: false
      url: "https://wave.webaim.org/"
    - naam: "NVDA of JAWS"
      type: "Screenreader"
      beschrijving: "Test de website met een screenreader om de gebruikerservaring voor blinde gebruikers te evalueren"
      verplicht: true
      url: "https://www.nvaccess.org/"
    - naam: "Lighthouse"
      type: "Browser DevTool"
      beschrijving: "Geïntegreerde toegankelijkheidsaudit in Chrome DevTools"
      verplicht: false
      url: "https://developers.google.com/web/tools/lighthouse"
  subrichtlijnen:
    - titel: "Kleurcontrast"
      omschrijving: "Richtlijnen voor voldoende contrast tussen tekst en achtergrond (minimaal 4.5:1 voor normale tekst, 3:1 voor grote tekst)"
      link: "./subrichtlijnen/kleurcontrast.yaml"
    - titel: "Formuliertoegankelijkheid"
      omschrijving: "Richtlijnen voor toegankelijke formulieren met labels, foutmeldingen en validatie"
      link: "./subrichtlijnen/formulieren.yaml"
    - titel: "Multimedia toegankelijkheid"
      omschrijving: "Richtlijnen voor ondertiteling, audiodescriptie en transcripties van video- en audio-inhoud"
      link: "./subrichtlijnen/multimedia.yaml"

succescriteria:
  - criterium: "Alle afbeeldingen hebben betekenisvolle alt-tekst of zijn gemarkeerd als decoratief"
    voldaan: true
  - criterium: "Kleurcontrast voldoet aan WCAG 2.1 niveau AA (minimaal 4.5:1 voor normale tekst)"
    voldaan: true
  - criterium: "Alle functionaliteit is bereikbaar en bedienbaar via toetsenbord"
    voldaan: true
  - criterium: "Focusindicatoren zijn duidelijk zichtbaar"
    voldaan: true
  - criterium: "Formulieren hebben labels en duidelijke foutmeldingen"
    voldaan: true
  - criterium: "Website is getest met minimaal één screenreader"
    voldaan: true
  - criterium: "Toegankelijkheidsverklaring is beschikbaar en up-to-date"
    voldaan: false

toepassingsvoorwaarde:
  voorwaarden:
    - "Van toepassing op alle publiek toegankelijke overheidswebsites en -applicaties"
    - "Verplicht volgens het Tijdelijk besluit digitale toegankelijkheid overheid"
    - "Van toepassing op nieuwe websites vanaf 23 september 2020"
    - "Van toepassing op bestaande websites vanaf 23 september 2021"
    - "Ook van toepassing op mobiele applicaties van overheidsorganisaties"

bronnen:
  wetten:
    - naam: "Tijdelijk besluit digitale toegankelijkheid overheid"
      url: "https://wetten.overheid.nl/BWBR0040936"
    - naam: "EN 301 549 - Toegankelijkheidseisen voor ICT producten en diensten"
      url: "https://www.etsi.org/deliver/etsi_en/301500_301599/301549/03.02.01_60/en_301549v030201p.pdf"
  beleid:
    - naam: "Digitale Inclusie Agenda"
      url: "https://www.digitaleoverheid.nl/overzicht-van-alle-onderwerpen/digitale-inclusie/"
    - naam: "European Accessibility Act"
      url: "https://ec.europa.eu/social/main.jsp?catId=1202"
  standaarden:
    - naam: "WCAG 2.1 (Web Content Accessibility Guidelines)"
      url: "https://www.w3.org/TR/WCAG21/"
    - naam: "ARIA 1.2 (Accessible Rich Internet Applications)"
      url: "https://www.w3.org/TR/wai-aria-1.2/"
    - naam: "HTML Living Standard"
      url: "https://html.spec.whatwg.org/"
  communities:
    - naam: "Stichting Accessibility"
      url: "https://www.accessibility.nl/"
    - naam: "Kennisplatform Toegankelijkheid"
      url: "https://www.toegankelijkheidsverklaring.nl/"
    - naam: "Web Accessibility Initiative (WAI)"
      url: "https://www.w3.org/WAI/"
  literatuur:
    - titel: "Inclusive Design Patterns"
      auteurs:
        - "Heydon Pickering"
      url: "https://shop.smashingmagazine.com/products/inclusive-design-patterns"
    - titel: "Accessibility for Everyone"
      auteurs:
        - "Laura Kalbag"
      url: "https://abookapart.com/products/accessibility-for-everyone"
    - titel: "Don't Make Me Think, Revisited"
      auteurs:
        - "Steve Krug"
      url: "https://sensible.com/dont-make-me-think/"
  developer_overheid:
    - titel: "Toegankelijkheid testen met automatische tools"
      type: "blog"
      url: "https://developer.overheid.nl/blog/toegankelijkheid-automatisch-testen"
    - titel: "Checklist toegankelijkheid"
      type: "kennisbank"
      url: "https://developer.overheid.nl/kennisbank/toegankelijkheid-checklist"

gerelateerde_richtlijnen:
  - titel: "Gebruiksvriendelijkheid van Overheidswebsites"
    relatie: "Toegankelijkheid en gebruiksvriendelijkheid versterken elkaar. Een toegankelijke website is vaak ook gebruiksvriendelijker voor alle gebruikers."
    link: "./gebruiksvriendelijkheid.yaml"
  - titel: "Privacy en Beveiliging van Webapplicaties"
    relatie: "Privacy-functies (zoals cookie-banners en privacy-instellingen) moeten ook toegankelijk zijn."
    link: "./privacy-beveiliging.yaml"
  - titel: "Responsive Design Principes"
    relatie: "Responsive design is een belangrijke voorwaarde voor toegankelijkheid op verschillende apparaten."
    link: "./responsive-design.yaml"
```

## Changelog

### Version 0.1.0 (2025-10-01)
- Initiële versie van de NeRDS richtlijn template, zoals gedefinieerd in de [oorspronkelijke template](https://github.com/developer-overheid-nl/don-site/issues/387)
- JSON Schema voor validatie toegevoegd
- Validatie script toegevoegd voor YAML
