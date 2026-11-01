[← overzicht](CHALLENGES.md)

---

# CSS challenge: View transitions



<a href="pres/vt.zip" target="_blank" rel="noopener noreferrer">code voor jouw</a> (zip)

---

## Cross document view transitions

Een transitie van een webpagina naar een andere webpagina.  
Alleen CSS - geen jS nodig.  

---

### Oefening 1: My first view transition

<a href="https://shooft.github.io/vt/1-my-first-vt/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

#### Stap 1 (CSS): 
Cross-document VT's aanzetten  

Dat doe je met:  

```
@view-transition {
	navigation: auto;
}
```

nb. Dat is voor oefening 1 al gedaan in zowel index.css als andere.css  

#### Stap 2 (CSS): 
De duration voor root langer maken (in zowel index.css als andere.css)

Dat doe je in de selector: `::view-transition-group(root) { }`

#### Stap 3 (CSS): 
DE H1 een view-transition-naam geven (in zowel index.css als andere.css)

Dat doe je met: `view-transition-name` (gebruik de naam howdy)

#### Stap 3b (CSS): 
De duration voor de h1 langer maken (in zowel index.css als andere.css)

Dat doe je in de selector: `::view-transition-group(howdy) { }`

#### Stap 4a (CSS): 
Een custom animation maken voor root (eerst in andere.css)

Zorg dat de wipe-out animatie eindigt met `translate:-100%` (links uit beeld schuiven)

Koppel de animatie aan de oude view.  
Dat doe je in de selector: `::view-transition-old(root) { }`  
Gebruik een stuiterende ease voor `animation-timing-function`  
Bron: [open props easing](https://github.com/argyleink/open-props/blob/main/src/props.easing.css)  

Zorg dat de wipe-in animatie start met `translate:100%` (vanaf rechts in beeld schuiven)

Koppel de animatie aan de oude view.
Dat doe je in de selector: `::view-transition-new(root) { }`
Gebruik een stuiterende ease voor `animation-timing-function`  

#### Stap 4b (CSS): 
Een custom animation maken voor root (eerst in index.css)

Zorg dat de wipe-out animatie eindigt met `translate:100%` (rechts uit beeld schuiven)

Koppel de animatie aan de oude view.  
Dat doe je in de selector: `::view-transition-old(root) { }`  
Gebruik een stuiterende ease voor `animation-timing-function`  

Zorg dat de wipe-in animatie start met `translate:-100%` (vanaf links in beeld schuiven)

Koppel de animatie aan de oude view.
Dat doe je in de selector: `::view-transition-new(root) { }`
Gebruik een stuiterende ease voor `animation-timing-function`  

#### Stap 5 (CSS): 
Houdt rekening met prefers-reduced-motion  

Omring de `@view-transition` boven in de css documenten met een media querie.

---

### Oefening 2: Overview and detail page

#### Stap 1 (CSS): 
<a href="https://shooft.github.io/vt/2-overview-and-detail/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

Cross-document VT's aanzetten (in zowel index.css als details.css)

Dat doe je met:  

```
@view-transition {
	navigation: auto;
}
```

nb. Houdt gelijk rekening met prefers-reduced-motion  

#### Stap 2 (CSS): 
De duration voor root langer maken (in zowel index.css als details.css)

Dat doe je in de selector: `::view-transition-group(root) { }`  


#### Stap 3 (CSS): 
De wolf soepel heen en weer terug laten bewegen

Daarvoor moet je volgende doen in index.css:
- de h2 in de eerste li een `view-transition-name` geven
- de img in de eerste li een `view-transition-name` geven
- de `view-transition-group` van de h2 een duration geven
- de `view-transition-group` van de img een duration geven

En het volgende doen in details.css:
- de h1 in de eerste li een `view-transition-name` geven
- de img in de eerste li een `view-transition-name` geven
- de `view-transition-group`van de h1 een duration geven
- de `view-transition-group` van de img een duration geven

#### Stap 4 (CSS): 
Nu de wolf en het biggetje

Daarvoor zou je hetzelfde als bij stap 3 nog een keer kunnen doen voor het biggetje. Maar dat wordt dan wel heel veel code als je het voor alle sprookjesfiguren wilt doen. Begin met de code die je voor de wolf geschreven hebt uit te commenten.

Je gaat daarvoor custom properties gebruiken. Die zijn al opgenomen index.html, wolf.html en big.html. Je vind daar bij de headings en images steeds een custom property: `--vt`.

In index.css het volgende doen:
- de h2's een `view-transition-name` geven (gebruik daarvoor `var(--vt)`)
- de img's `view-transition-name` geven (gebruik daarvoor `var(--vt)`)
- de h2's een `view-transition-class` geven (gebruik daarvoor `title`). De class kun je gebruiken om een animatie voor alle h2's tegelijk te definieren (dan hoeft dat niet los voor elk karakter)
- de image's een `view-transition-class` geven (gebruik daarvoor `image`).
- de `view-transition-group` van de h2's een duration geven (gebruik de `view-transition-class`)
- de `view-transition-group` van de img's een duration geven (gebruik de `view-transition-class`)

En het volgende doen in details.css:
- de h1 een `view-transition-name` geven (gebruik daarvoor `var(--vt)`)
- de img `view-transition-name` geven (gebruik daarvoor `var(--vt)`)
- de h1 een `view-transition-class` geven (gebruik daarvoor `title`). De class kun je gebruiken om een animatie voor alle h2's tegelijk te definieren (dan hoeft dat niet los voor elk karakter)
- de image's een `view-transition-class` geven (gebruik daarvoor `image`).
- de `view-transition-group` van de h1 een duration geven (gebruik de `view-transition-class`)
- de `view-transition-group` van de img een duration geven (gebruik de `view-transition-class`)

Hatsiekiedee, klaar.

---

## Same document view transitions  

Een transitie op een webpagina zelf.  
Nog steeds veel CSS, maar ook JS.  

---

### Oefening 3: My first cross document view transition

<a href="https://shooft.github.io/vt/3-my-first-sdvt/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

#### Stap 1 (CSS): 
Geef de img een `view-transition-name` (raket)

#### Stap 2 (JS): 
Een view transitie starten met JS  

De raket en debutton zijn al voor je opgezocht. Er is al een eventlistener. Een ook een callback function waarin je de view transitie gaat starten. In de functie vind je ook al een `if else` statement om te checken of de browser view transities ondersteunt.

In het if deel ga je de view transitie starten. Op het blog piccalilli vind je [een artikel van ene Cyd Stumpel hou je een view transitie kunt starten](https://piccalil.li/blog/start-implementing-view-transitions-on-your-websites-today/)


#### Stap 3 (JS): 
In het else deel kun je een `alert()` tonen dat de browser geen view transities ondersteunt.

#### Stap 4 (CSS): 
De duration voor raket langer maken, met `::view-transition-group(raket) { }`  

Maak de animatie wat interessanter met een `cubic-bezier() animation-timing-function`  
Lea Verou heeft [een goede cubic-bezier() generator](https://cubic-bezier.com/) gemaakt.  

---

### Oefening 4: Layout change

<a href="https://shooft.github.io/vt/4-layout-change/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

nb. Het husselen werkt al. Je gaat dat er alleen wel leuker uit laten zien met view transities.  

#### Stap 1 (CSS): 
Geef de li's een `view-transition-name`.

`view-transition-name` moeten uniek zijn. Dat zou heel veel werk betekenen om dat voor alle li's te doen. Daar is een oplossing voor bedacht. Je kunt `match-element` als `view-transition-name` gebruiken. Dan zorgt de browser er achter de schermen magisch voor dat elke li een unieke naam krijgt.  

Geef de li's een `view-transition-class` (item). Die class kun je zo gebruiken om in één keer een animatie te definiëren voor alle li's tegelijk.

#### Stap 2 (JS): 
Een view transitie starten met JS. Spiek even bij sommetje 3 hoe je dat doet.  

#### Stap 3 (CSS): 
De duration voor de li's langer maken, met `::view-transition-group`. Gebruik daarvoor de class die je bij stap 1 hebt aangemaakt.

#### Bonus
De button disablen als de li's aan het husselen zijn.  

#### Stap 4 (JS):  
Roep in de functie disableButton aan bij het starten van de view transitie.

#### Stap 5 (CSS):  
Stijl de button als die disabled is. De secletoren daarvoor staan al in de CSS.  

#### Stap 6/7 (JS):  
Als de view transitie klaar is roep je de functie enableButton aan. 

Op MDN staat een artikel [hoe je iets doet als de view transitie klaar is] (https://developer.mozilla.org/en-US/docs/Web/API/ViewTransition/finished).  

---

### Oefening 5: Filters

<a href="https://shooft.github.io/vt/5-filters/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

nb. Het toevoegen en verwijderen van filters werkt al. Je gaat dat er alleen wel leuker uit laten zien met view transities.  

#### Stap 1 (CSS): 
Geef de de buttons in de div een `view-transition-name` en `view-transition-class`.

#### Stap 2 (JS): 
Start een view transitie in de callback functie addFilter() die wordt aangeroepen als op de + wordt geklikt.  

#### Stap 3 (JS): 
Start een view transitie in de callback functie removeFilter() die wordt aangeroepen als op een button in de div wordt geklikt.  

#### Stap 4 (CSS): 
De duration voor de buttons langer (.33s) maken, met `::view-transition-group`. Gebruik daarvoor de class die je bij stap 1 hebt aangemaakt.

Geef de buttons ook een hele korte delay (.075s).  

#### Bonus
Nu nog een mooie fadeIn en fadeOut animatie toevoegen voor de buttons.

#### Stap 5 (CSS): 
Met de selector `::view-transition-new(.filter):only-child` kun je de button die wordt toegevoegd selecteren. Die heeft namelijk alleen een nieuwe state (want hij bestond nog niet in de oude state).  

Maak de animatie `--is-coming` af zodat de button van 0% naar 100% schaalt.  
Koppel de animatie aan de `::view-transition-new(.filter):only-child` selector met een duration van .33s en een delay van 0s.

nb. Cyd heeft wederom een goed artikel geschreven waarin ze in meer detail uitlegt [hoe je verschijnende en verdwijnende elementen kunt selecterent](https://cydstumpel.nl/being-lazy-with-view-transition-old-and-new/).  

#### Stap 6 (CSS): 
Met de selector `::view-transition-old(.filter):only-child` kun je de button die wordt verwijderd selecteren. Die heeft namelijk alleen een oude state (want hij bestaat niet meer in de nieuwe state).  

Maak de animatie `--is-going` af zodat de button van 100% naar 0% schaalt.  
Koppel de animatie aan de `::view-transition-new(.filter):only-child` selector met een duration van .33s en een delay van 0s.

#### Stap 7 (CSS): 
Als je snel op de + button wilt kunnen klikken moet je nog wat doen. De view transities animeren in de top-layer (de laag boven alle z-indexen) en dekken de button tijdens het animeren af.

Bramus van Damme heeft een artikel geschreven [hoe je door de view transities heen kunt klikken](https://www.bram.us/2025/01/29/view-transitions-page-interactivity/).   

---
 
## Links

🎯 ⸺ [text](https://developer.chrome.com/docs/web-platform/view-transitions) (chrome)  
🎯 ⸺ [Some practical examples of view transitions to elevate your UI](https://piccalil.li/blog/some-practical-examples-of-view-transitions-to-elevate-your-ui/) (piccalilli)
🎯 ⸺ [View Transition API](https://developer.mozilla.org/en-US/docs/Web/API/View_Transition_API) (MDN)
