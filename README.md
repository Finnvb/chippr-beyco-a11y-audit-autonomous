
# Rapportage webtoegankelijkheid-test voor Chippr-Beyco

Dit document is een template voor een webtoegankelijkheid-test volgens de Web Content Accessibility Guidelines (WCAG). Een consistente rapportage helpt bij het uitvoeren van een evaluatie en zorgt er voor dat verschillende tests kunnen worden vergeleken.

In deze rapportage wordt het **detail pagina** getest aan de hand van de checklist van het a11y project.  

Datum webtoegankelijkheid-test: 28-10-2021

Webtoegankelijkheid-test uitgevoerd door: Finn van Bekkum

## Inhoudsopgave

  * [Samenvatting](#samenvatting)
  * [Achtergrond bij de evaluatie](#achtergrond-bij-de-evaluatie)
  * [Afbakening](#afbakening)
  * [Beoordelaars](#beoordelaars)
  * [Beoordelingsproces](#beoordelingsproces)
  * [Testresultaten en aanbevelingen](#testresultaten-en-aanbevelingen)
  * [Bijlagen](#bijlagen)
  * [Licentie](#licentie)
  


## Samenvatting

Dit rapport beschrijft in hoeverre de website beyco.nl overeenstemt met de Web Content Accessibility Guidelines (WCAG) van het W3C.

Conslusie van deze test luidt dat de Beyco website niet voldoet de WCAG 2.1, op niveau AA. Gedetailleerde resultaten en aanbevelingen zijn verderop in dit document beschikbaar en in de referenties vindt u bronnen voor eventuele vervolgstudie. Wij stellen feedback op deze evaluatie zeer op prijs.


## Achtergrond bij de evaluatie

De webtoegankelijkheid-test vereist een combinatie van semi-geautomatiseerde en handmatig uitgevoerde evaluatie tools door een ervaren beoordelaar. De beoordelingsresultaten in dit rapport zijn gebaseerd op een beoordeling welke is uitgevoerd op 1-11-2021. De website kan ondertussen aangepast zijn.

##  Afbakening

https://beyco.nl/

Beyco zorgt voor een platform waar verkopers en inkopers met elkaar in contact kunnen komen.

https://test.beyco.chippr.dev/

https://test.beyco.chippr.dev/trade/offers/8f3622d6-75a1-43b8-a960-3daecc5c880a


![afbeelding](https://user-images.githubusercontent.com/26089533/139905279-a3b2f2b0-eeeb-4d05-b702-e08625cc5502.png)

Test data:

   * 28-10-2021
   * 29-10-2021
   * 01-11-2021

Taal van website: Engels

## Beoordelaars

Finn van Bekkum

Student

finn.van.bekkum@hva.nl

Nederlands

## Beoordelingsproces

Deze beoordelings is uitgevoerd op WCAG 2.1 Niveau AA

De tools die zijn gebruikt voor deze beoordeling zijn de volgende:

   
 * [A11Y Checklist](https://www.a11yproject.com/checklist/)
 *  [WCAG Guidelines Overview](https://www.w3.org/WAI/standards-guidelines/wcag/)
 * [Google Lighthouse](https://developers.google.com/web/tools/lighthouse)


## Testresultaten en aanbevelingen

De detail pagina van Beyco voldoet niet aan nivea AA van de WCAG 2.1.

#### Sterke punten
* Beschrijving van buttons en links zijn duidelijk.
* Images maken gebruik van de alt attribute.
* Headings worden in een logische volgorde gebruikt en worden niet overgeslagen.
* Met het tabben door de pagina kun je duidelijk zien welke link actief is. 

#### Ontoegankelijke punten
* In de code staan veel lege div elementen.
* Vermijd het gebruik van het autofocus attribuut bij de iframe van de kaart.
* Bij de iframe van de kaart wordt er een aantal keer getabt op elementen die niet zichtbaar zijn.
* De social media logo's in de footer krijgen geen focus style bij het tabben.

### Checklist

#### Content 
✓ Voldoet

#### Global code

* Validate your HTML

![afbeelding](https://user-images.githubusercontent.com/26089533/139850400-5f48eb59-ad06-4ce7-af1a-0be8239c470c.png)

Hij geeft aan dat er geen lang attribute aanwezig is in de HTML start tag. Maar als ik zelf in de inspector kijk zie ik wel een lang attribute staan. Misschien dat lang="en-us" een ongeldige waarde is. Ook kom ik veel lege div elementen tegen in de code. 
Verder staat er geen heading in de body element. Deze staan overigens wel in de main element. 


* Avoid using the autofocus attribute.

Mensen die blind of slechtziend zijn, kunnen gedesoriënteerd raken wanneer de focus zomaar wordt verplaatst. Ook kan het voor mensen met een motorische handicap voor problemen zorgen, omdat het voor hen extra werk kan opleveren om vanuit het autofocusgebied naar andere locaties op de pagina te navigeren.

#### Keyboard

* Make sure there is a visible focus style for interactive elements that are navigated to via keyboard input.

In de footer komt bij de social media logo's geen focus style zoals bij de links.

* Remove invisible focusable elements.

Bij de iframe van de kaart wordt er een aantal keer getabt op elementen die niet zichtbaar zijn.

#### Images
✓ Voldoet

#### Headings
✓ Voldoet

#### Lists

* Use list elements (ol, ul, and dl elements) for list content.

In de header wordt bij de nav geen ul gebruikt en in de footer ook niet.

#### Controls

*  Provide a skip link and make sure that it is visible when focused.

Maak gebruik van skip links voor screen readers en keyboard-only gebruikers.

#### Tables
n.v.t.

##  Bijlagen
Dit is de huidige score van de detail pagina van Beyco voor desktop en mobile.
### Lighthouse Desktop
![afbeelding](https://user-images.githubusercontent.com/26089533/139872821-31dd8b4b-8d59-4b95-b138-1154ad54bc5f.png)

### Lighthouse Mobile
![afbeelding](https://user-images.githubusercontent.com/26089533/139873260-ad64d57d-83fd-4b5a-923a-0b0bfaa46639.png)

## Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
