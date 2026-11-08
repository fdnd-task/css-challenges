# Fonts intro  

<details>
  <summary>
    <h2>Web-safe fonts 👍</h2>
    <p>De makkelijkste manier om lettertypen in je ontwerp op te nemen is door web-safe fonts te gebruiken. Een web-safe font is een lettertype dat standaard op vrijwel alle computers, smartphones en tablets beschikbaar is. Hierdoor hoeft het lettertype niet te worden gedownload (maakt je website snel) en wordt de tekst overal op dezelfde manier weergegeven (maakt je website consistent).  </p>
  </summary>

  <p>De best ondersteunde web-safe fonts zijn:&nbsp;</p>
  <ul>
    <li>Arial</li>
    <li>Verdana</li>
    <li>Tahoma</li>
    <li>Trebuchet MS</li>
    <li>Times, New Roman</li>
    <li>Georgia</li>
    <li>Courier New</li>
  </ul>
  <p>CSS font stack houdt <a rel="noopener" href="https://www.cssfontstack.com/" target="_blank">een overzicht van alle web-safe fonts</a> bij met het percentage van de apparaten waar het font op aanwezig is.<strong></strong></p>

  <h3>font-family property</h2>


  <p>Op de volgende manier kun je een web-safe fonts in je CSS gebruiken:</p>

  <code>
    body { font-family:tahoma;}

    h2 { font-family:"courier new";}
  </code>


  <p>body {<br>&nbsp; font-family:tahoma;<br>}</span></code></span></p>
  <p><span style="font-size: 16px;"><code><span style="color: #008000;">h2 {<br>&nbsp; font-family:"courier new";<br>}</span></code></span></p>
  <p>HTML elementen erven de font-family van hun parent. Dat betekent dat als je voor de body een <em>font-family </em>declareert, alle kinderen van de body die <em>font-family</em> ook krijgen. Dat font wordt dan dus door de hele pagina gebruikt.</p>
  <p>Als er een spatie in de naam van het font staat moet je de naam tussen aanhalingstekens zetten. Dat mag altijd, maar voor font-namen met spaties moet het.</p>
  <p><iframe height="300" style="width: 98%;" scrolling="no" title="HWIVI - deep dive - css dive - web-safe fonts" src="https://codepen.io/editor/shooft/embed/019f55c1-9ced-72fb-8a84-1e7f496e0cd1?default-tab=css%2Cresult&amp;theme-id=-3">
    See the Pen <a rel="noopener" href="https://codepen.io/editor/shooft/pen/019f55c1-9ced-72fb-8a84-1e7f496e0cd1">
    HWIVI - deep dive - css dive - web-safe fonts</a> by Sanne (<a rel="noopener" href="https://codepen.io/shooft">@shooft</a>)
    on <a rel="noopener" href="https://codepen.io">CodePen</a>.
  </iframe></p>
  <h2 style="margin-top: 2.5em; padding-top: 1em; border-top: solid 1em YellowGreen;">Lettertype van het besturingssysteem</h2>
  <p>Als je wilt dat je website op het besturingsysteem (Windows, macOs, iOS, Android...) lijkt kun je het lettertype dat het besturingsysteem gebruiken in je CSS:</p>
  <p><span style="font-size: 16px;"><code><span style="color: #008000;">body {<br>&nbsp; font-family:system-ui;<br>}</span></code></span></p>
  <p>Op deze manier gebruik je Segoe op Windows, San Francisco op macOS en Roboto op Android. Je website ziet er dan dus op verschillende apparaten anders uit, maar lijkt wel altijd op het besturingsysteem.</p>
  <p><iframe height="300" style="width: 98%;" scrolling="no" title="HWIVI - deep dive - css dive - system font" src="https://codepen.io/editor/shooft/embed/019f55c6-6ef1-76dd-83d3-7f597c9751af?default-tab=css%2Cresult&amp;theme-id=-3">
    See the Pen <a rel="noopener" href="https://codepen.io/editor/shooft/pen/019f55c6-6ef1-76dd-83d3-7f597c9751af">
    HWIVI - deep dive - css dive - system font</a> by Sanne (<a rel="noopener" href="https://codepen.io/shooft">@shooft</a>)
    on <a rel="noopener" href="https://codepen.io">CodePen</a>.
  </iframe></p>
  <h2 style="margin-top: 2.5em; padding-top: 1em; border-top: solid 1em YellowGreen;">Font-stack</h2>
  <p>Je kunt ook een lijst met lettertypen toekennen aan de <em>font-family</em> property.&nbsp;</p>
  <p><span style="color: #008000; font-size: 16px;"><code>font-family: Georgia, Times, "Times New Roman", serif;</code></span></p>
  <p>De browser gebruikt dan het eerste lettertype uit de lijst dat beschikbaar is. Als het eerste lettertype niet beschikbaar is op het apparaat van de gebruiker, probeert de browser het volgende, enzovoort. Met een font-stack is de kans dat het lettertype dat gebruikt wordt lijkt op het lettertype dat je wilt het grootst.</p>
  <p>Als voorlaatste lettertype in de lijst neem je het web-safe font op dat het meest lijkt op het font van je voorkeur. Als laatste lettertype neem je de generieke letterfamilie op waarin het font van je voorkeur valt:</p>
  <ul>
  <li>serif – lettertypen met schreefjes (bijv. Times New Roman)</li>
  <li>sans-serif – zonder schreefjes (bijv. Arial)</li>
  <li>monospace – alle tekens even breed (bijv. Courier New)</li>
  <li>cursive – handschriftachtig</li>
  <li>fantasy – decoratieve lettertypen</li>
  </ul>
  <p><iframe height="300" style="width: 99%;" scrolling="no" title="HWIVI - deep dive - css dive - font-stack" src="https://codepen.io/editor/shooft/embed/019f559a-cf55-7efe-9c5f-7c6a82619357?default-tab=css%2Cresult&amp;theme-id=-3">
    See the Pen <a rel="noopener" href="https://codepen.io/editor/shooft/pen/019f559a-cf55-7efe-9c5f-7c6a82619357">
    HWIVI - deep dive - css dive - font-stack</a> by Sanne (<a rel="noopener" href="https://codepen.io/shooft">@shooft</a>)
    on <a rel="noopener" href="https://codepen.io">CodePen</a>.
  </iframe></p>
  <p>Op GitHub vind je een overzicht van <a rel="noopener" href="https://github.com/yesiamrocks/CSS-Fallback-Fonts" target="_blank">font-stacks voor veel gebruikte lettertypes</a>.</p>

</details>

