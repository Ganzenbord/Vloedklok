# Vloedklok

One-thumb mobiele platformer met een dorp-upgradelaag. Eén bestand, geen build, geen dependencies.

- **Spelen:** open `index.html` in een (mobiele) browser.
- **Besturing:** tik = springen, vasthouden = hoger, tik in de lucht = dubbelsprong, omlaag vegen (en vasthouden) = bukken. Op desktop: spatie en pijl omlaag.
- **Doel:** blijf de vloedgolf voor en luid de klok aan het eind van elke expeditie.
- **Dorp:** kaart met zes bouwplaatsen voor Goudmijn (passief goud, ook offline), Dijk, Vuurtoren, Herberg en Werkplaats.
- **Terrein:** elke bouwplaats is kust, heuvel of centrum; een gebouw op zijn voorkeursterrein krijgt een bonus. Verplaatsen/ruilen kost goud.
- **Leger & strooptochten:** train wachters in de Kazerne (Dijkwerker, Boogschutter, Sloper) en zet ze in op drie paden van een vijandig eiland voordat de vloed komt. 2 van 3 nesten = volgend eiland. Herberg, Werkplaats, Dijk en Vuurtoren versterken het leger.
- **Oneindig:** eindeloze expeditie die steeds sneller gaat; je record wordt bewaard.
- **Winkel:** diamanten besteden aan goud, parels en een tweede kans. Echte betalingen zijn **niet** gekoppeld: `PAY.buy` in `index.html` is de plek om Play Billing / StoreKit / Stripe aan te sluiten. Met `?dev=1` worden aankopen gesimuleerd.

Levels zijn deterministisch per nummer gegenereerd. Voortgang staat in `localStorage` (`vloedklok.v1`).
