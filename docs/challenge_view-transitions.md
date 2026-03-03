[← overzicht](CHALLENGES.md)

---

# CSS challenge: View transitions



<a href="pres/vt.zip" target="_blank" rel="noopener noreferrer">code voor jouw</a> (zip)

---

## Cross document view transitions

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

Zorg dat de wipe-out animatie eindigt met translate:-100% (links uit beeld schuiven)

Koppel de animatie aan de oude view.  
Dat doe je in de selector: `::view-transition-old(root) { }`  
Gebruik een stuiterende ease voor animation-timing-function  
BRON: [open props easing](https://github.com/argyleink/open-props/blob/main/src/props.easing.css)  

Zorg dat de wipe-in animatie start met translate:100% (vanaf rechts in beeld schuiven)

Koppel de animatie aan de oude view.
Dat doe je in de selector: `::view-transition-new(root) { }`
Gebruik een stuiterende ease voor animation-timing-function  

#### Stap 4b (CSS): 
Een custom animation maken voor root (eerst in index.css)

Zorg dat de wipe-out animatie eindigt met translate:100% (rechts uit beeld schuiven)

Koppel de animatie aan de oude view.  
Dat doe je in de selector: `::view-transition-old(root) { }`  
Gebruik een stuiterende ease voor animation-timing-function   

Zorg dat de wipe-in animatie start met translate:-100% (vanaf links in beeld schuiven)

Koppel de animatie aan de oude view.
Dat doe je in de selector: `::view-transition-new(root) { }`
Gebruik een stuiterende ease voor animation-timing-function  

#### Stap 5 (CSS): 
Houdt rekening met prefers-reduced-motion  

Omring de `@view-transition` boven in de css documenten met een media querie.

---

### Oefening 2: Overview and detail page

<a href="https://shooft.github.io/vt/2-overview-and-detail/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

---

## Same document view transitions

---

### Oefening 3: My first cross document view transition

<a href="https://shooft.github.io/vt/3-my-first-sdvt/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  
---

### Oefening 4: Layout change

<a href="https://shooft.github.io/vt/4-layout-change/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  
---

### Oefening 5: Filters

<a href="https://shooft.github.io/vt/5-filters/index.html" target="_blank" rel="noopener noreferrer">voorbeeld</a>  

---

📗 ⸺
<a href="pres/FDND-CSSchallenge7-Fonts-intro.pdf" target="_blank" rel="noopener noreferrer">Fonts en font-properties intro</a> 
(pdf 3MB)   

---

## Code

🧑‍💻 ⸺ <a href="https://github.com/fdnd-task/css-challenge-typografie" target="_blank" rel="noopener noreferrer">Code voor oefening 1, 2 en 3</a> (GitHub - even forken)

---

## Oefening 1: 🌱 Fonts en font-properties (opwarmen)

📊 ⸺ 🟦 🟥

📙 ⸺ 
<a href="pres/FDND-CSSchallenge7-Fonts-oefening1.pdf" target="_blank" rel="noopener noreferrer">Typografie oefening 1</a> 
(pdf)

🧑‍💻 ⸺
<a href="https://codepen.io/shooft/pen/jOgRZZJ" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---

## Oefening 2: 🦚 Mini posters

📊 ⸺ 🟦 🟥 ⬛️  

📙 ⸺ 
<a href="pres/FDND-CSSchallenge7-Fonts-oefening2.pdf" target="_blank" rel="noopener noreferrer">Typografie oefening 2</a> 
(pdf 3MB)

🧑‍💻 ⸺
<a href="https://codepen.io/shooft/pen/jOgRZeo" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)  
🧑‍💻 ⸺
<a href="https://codepen.io/shooft/pen/yLmrvQB" target="_blank" rel="noopener noreferrer">Uitwerking met extra's</a>
(CodePen)

niet meteen spieken 🫣  

---

## Oefening 3: 🦋 Variabele fonts

📊 ⸺ 🟦 🟥 ⬛️  

📙 ⸺ 
<a href="pres/FDND-CSSchallenge7-Fonts-oefening3.pdf" target="_blank" rel="noopener noreferrer">Typografie oefening 3</a> 
(pdf 3MB)

🧑‍💻 ⸺
<a href="https://codepen.io/shooft/pen/BaXEYBm" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)  
🧑‍💻 ⸺
<a href="https://codepen.io/shooft/pen/eYqoZgO" target="_blank" rel="noopener noreferrer">Uitwerking met extra's</a>
(CodePen)

niet meteen spieken 🫣  

---
 
## Links

🎯 ⸺ [web-safe fonts](https://web.mit.edu/jmorzins/www/fonts.html) (www 🧑‍💻)   

🎯 ⸺ [@font-face intro](https://www.w3schools.com/CSSref/atrule_font-face.php) (w3schools 🐥)     
🎯 ⸺ [@font-face uitgebreider](https://hacks.mozilla.org/2009/06/beautiful-fonts-with-font-face/) (MDN 🦊)    

🎯 ⸺ [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-weight) (MDN 🦊)    
🎯 ⸺ [font-style](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-style) (MDN 🦊)    
🎯 ⸺ [font-strectch](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-stretch) (MDN 🦊)    
🎯 ⸺ [font-display](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-display) (MDN 🦊)    
🎯 ⸺ [font-variation-settings](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-variation-settings) (MDN 🦊)    

🎯 ⸺ [variabele fonts intro](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_fonts/Variable_fonts_guide) (MDN 🦊)  
🎯 ⸺ [variabele fonts collectie](https://fonts.google.com/?categoryFilters=Technology:%2FTechnology%2FVariable) (Google fonts🦖)  
🎯 ⸺ [variabele fonts voorbeelden](https://speckyboy.com/variable-font-examples/) (www 🧑‍💻)  

🎯 ⸺ [wakamaifondue - de font info tool](https://wakamaifondue.com/beta/) (roel niekskens 🤴)  
🎯 ⸺ [Font Squirrel - font generator](https://www.fontsquirrel.com/tools/webfont-generator) (www 🐿️)  

🎯 ⸺ [FOIT vs FOUT](https://www.hoppinger.com/nl/insights/loading-webfonts#:~:text=Maar%20hoe%20voorziet%20een%20browser,of%20Unstyled%20Text%20(FOUT).) (www 🧑‍💻)  
🎯 ⸺ [Google fonts illegaal in EU](https://slik.nl/blog/google-fonts/) (www 🧑‍💻)   