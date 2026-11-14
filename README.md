# Castra (repo: Vloedklok)

Mobiel strategiespel in Romeinse stijl, in 3D. Eén bestand (`index.html`), geen build. Three.js wordt van cdnjs geladen, dus er is internet nodig; zonder WebGL valt het spel terug op een platte 2D-weergave.

- **Kern:** bouw je stad, train soldaten en val steden van andere spelers aan. Een aanval loopt over drie wegen; 2 van de 3 vaandels veroveren is winst. Bekers vormen de ranglijst.
- **Stad:** negen bouwplaatsen (rand / heuvel / centrum, bonus op voorkeursterrein). Gebouwen: Stadhuis, Bank, Goudmijn, Kazerne, Boogschutterskamp, Muur, Wachttoren, Taverne, Smederij.
- **Niveaus:** elk gebouw heeft 20 niveaus. Kosten x1,45 en bouwtijd x1,55 per niveau (15 s tot 8 uur), één bouwer tegelijk. Het uiterlijk verandert op niveau 5, 10 en 15: hout, steen, groot steen, marmer met goud. De Muur loopt om de hele stad: palissade, lage stenen muur, hoge muur met kantelen en hoektorens, en ten slotte torens met daken en patrouilles.
- **Vereisten:** niets kan hoger dan het Stadhuis. Stadhuis niveau L vraagt Goudmijn en Bank op L-1 (en vanaf 4 de Muur op L-2). Muur niveau L (vanaf 3) vraagt Bank en Goudmijn op L-1.
- **Leger:** Legionair (Kazerne), Boogschutter (Boogschutterskamp), Stormram (Kazerne niveau 3). Taverne, Smederij en Wachttoren versterken het leger.
- **Verdediging:** verdeel verdedigingspunten (uit de Muur) over je drie wegen: wachters, adelaars, ballista.
- **Veldtocht:** de 2D-platformer (tik = springen, omlaag vegen = bukken) is een bijverdienste voor goud; je rent voor lava uit.
- **Andere spelers:** werkt alleen in de gepubliceerde Claude-pagina (gedeelde database via `claude.use('db')`). Lokaal vecht je tegen computerkampen. Zonder eigen server is valsspelen mogelijk.
- **Winkel:** diamanten voor goud, parels, een tweede kans en het afmaken van bouwklussen. Echte betalingen zijn **niet** gekoppeld (`PAY.buy`); `?dev=1` simuleert aankopen.

Voortgang staat in `localStorage` (`vloedklok.v1`).
