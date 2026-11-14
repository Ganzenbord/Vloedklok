# Vloedklok

One-thumb mobiele platformer met een dorp-upgradelaag. Eén bestand, geen build, geen dependencies.

- **Spelen:** open `index.html` in een (mobiele) browser.
- **Besturing:** tik = springen, vasthouden = hoger, tik in de lucht = dubbelsprong, omlaag vegen (en vasthouden) = bukken. Op desktop: spatie en pijl omlaag.
- **Doel:** blijf de vloedgolf voor en luid de klok aan het eind van elke expeditie.
- **Kern:** bouw je dorp, train wachters en val dorpen van andere spelers aan (3 paden, 2 van 3 nesten = winst, bekers als ranglijst). Expedities (de platformer) zijn de manier om goud te verdienen.
- **Dorp:** kaart met negen bouwplaatsen (kust/heuvel/centrum, bonus op voorkeursterrein). Gebouwen: Stadhuis, Bank, Goudmijn, Kazerne, Boogschutterskamp, Muur, Vuurtoren, Herberg, Werkplaats.
- **Bouwen:** elke bouw/upgrade kost tijd (15 s tot 80 min, oplopend per niveau), één bouwer tegelijk. Niets kan hoger dan het Stadhuis; Stadhuis en Muur vragen bepaalde niveaus van Bank, Goudmijn en Kazerne.
- **Verdediging:** verdeel verdedigingspunten (uit de Muur) over je drie paden.
- **Andere spelers:** werkt alleen in de gepubliceerde Claude-pagina (gedeelde database via `claude.use('db')`). Lokaal geopend vecht je tegen computerdorpen. De client is niet te vertrouwen: zonder eigen server is valsspelen mogelijk.
- **Winkel:** diamanten besteden aan goud, parels, een tweede kans en het afmaken van bouwklussen. Echte betalingen zijn **niet** gekoppeld (`PAY.buy`). Met `?dev=1` worden aankopen gesimuleerd.

Levels zijn deterministisch per nummer gegenereerd. Voortgang staat in `localStorage` (`vloedklok.v1`).
