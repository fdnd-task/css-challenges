[← overzicht](CHALLENGES.md)

---

# CSS challenge 13: GSAP voor gevorderden

🗓️ ⸺ **Dinsdag 20 mei**  
⏰ ⸺ **9:30 - ca 11:30 uur**  

---

## Oefening 1: 🐁 Starten met mouse events 🐁
📊 ⸺ 🟦🟦🟥  
Opdracht: animeer `.cursor` zodat het element de muis volgt.

https://github.com/user-attachments/assets/ab5bb6b5-bc54-4072-9172-3d44a8373d82

👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/KwwYdyW" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/vEEPOgr" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---
## Oefening 2: 💅 Reactieve custom cursors 💅
📊 ⸺ 🟦🟥🟥
Opdracht: animeer `.cursor` op basis van waar je overheen hovert.

https://github.com/user-attachments/assets/91c88797-c276-4495-89f7-54fb0b1a2436

In de event parameter staat een stuk meer informatie dan alleen de clientX en clientY. Ooit gehoord van target bijvoorbeeld?

###### Kom je er niet uit?
Log eens wat er in e.target zit (`console.log(e.target)` in de event listener functie). Wat als we willen weten over wat voor element we heen hoveren, kunnen we dat opvragen vanuit e.target? (Spoiler: JA dat kan!)

👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/xbbewzy" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/YPPgLox" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---
## Oefening 3: 🏞️ Image trails intro 🏞️
📊 ⸺ 🟥🟥🟥

Opdracht: animeer de foto zodat het midden van de foto de muis volgt.

https://github.com/user-attachments/assets/1445b02d-53b0-4a73-930e-9c2bffd38473

Wanneer je een mouse event-listener op een element zet zijn de clientX en clientY waarden nog steeds gelijk aan de x en y as van de window. Dat betekent dat je voor deze animatie zowel e.clientX/e.clientY als de breedte en hoogte van de button nodig hebt.
Dit kan je op verschillende manieren opvragen; google eens 'How to get width of element js'.

Hier een visuele weergave:

![work sketches-12](https://github.com/user-attachments/assets/af1354ae-390e-49ec-a740-74622b0da913)

👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/ByyEjRd" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/xbbBzbR" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---
## Oefening 4: 🤩 Mouse events op elementen 🤩
📊 ⸺ 🟥⬛️⬛️
Opdracht: animeer het clip-path in de button op basis van waar de muis entert (en BONUS: leavet).

https://github.com/user-attachments/assets/0d39c432-ec26-4206-bee8-d443b5ba28a8

Wanneer je een mouse event-listener op een element zet zijn de clientX en clientY waarden nog steeds gelijk aan de x en y as van de window. Dat betekent dat je voor deze animatie zowel e.clientX/e.clientY als de x en y positie van de button nodig hebt.
Dit kan je op verschillende manieren opvragen; google eens 'How to get x position of element js'.

Wanneer je client x/y aftrekt van de x/y positie van het element krijg je de coordinaten die je kan gebruiken om de clip path in te starten.

Clip path circle werkt als volgt: `clip-path({circle-size} at {x positie} {y positie})`

👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/VYYNvOZ" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/pvvYKeo" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---
## Oefening 4: 🌠🌃🎆 MEERDERE IMAGES IN EEN TRAIL 🌠🌃🎆
📊 ⸺ ⬛️⬛️⬛️
Opdracht: animeer meerdere afbeeldingen die de muis volgen 💅🤩

https://github.com/user-attachments/assets/65ed7166-d287-415a-a7d4-27f3bd4d62d4

Image trails 😍, een echte uitdaging, maar leuke (tikkeltje irritante) toevoeging op websites!

👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/PwwgZJj" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/raaRVwW" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

niet meteen spieken 🫣  

---

### Oefening 5: 💬 SplitTexts 💬
📊 ⸺ ⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️⬛️
Opdracht: animeer de splittexts zoals jij wil 💪

https://github.com/user-attachments/assets/221facfb-5f28-4440-a1ff-b5d6eb7e6679


👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/WbbWrWa" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/NPPJzQq" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)

### Oefening 6: (Te) Gekke dingen met SplitText en Draggable
Opdracht: gekke dingen maken!! 

<img width="1311" alt="image" src="https://github.com/user-attachments/assets/3931a5d3-6aa6-418a-a5a6-86d2e6826b71" />


👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/yyyrOem" target="_blank" rel="noopener noreferrer">Code voor jou</a>
(CodePen)  
👩🏻‍💻 ⸺
<a href="https://codepen.io/Sidstumple/pen/vEEMLwZ" target="_blank" rel="noopener noreferrer">Uitwerking</a>
(CodePen)


 
## Links
🎯 ⸺ [GSAP website](https://gsap.com/) (GSAP 💚🧦)  
🎯 ⸺ [GSAP docs](https://gsap.com/docs/v3/) (GSAP 💚🧦)  

🎯 ⸺ [GSAP plugins](https://gsap.com/docs/v3/Installation/?tab=cdn&module=esm&require=false) (GSAP 💚🧦)  
