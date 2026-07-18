# Näring

Här dokumenteras modellen för att räkna energi, protein, kolhydrater och fett i recept och matlådor.

## Princip

Beräkningen görs i tre steg:

1. Registrera faktisk använd vikt och näringsvärde per 100 g för varje ingrediens.
2. Summera hela satsens energi och makron.
3. Väg den färdiga satsen och fördela näringen efter faktisk portionsvikt.

## Formler

För varje ingrediens:

`total energi = vikt i gram × kcal per 100 g / 100`

Samma formel används för protein, kolhydrater och fett.

När hela satsen är färdig:

`värde per 100 g = satsens total × 100 / färdig satsvikt`

För en matlåda:

`värde i matlådan = satsens total × matlådans vikt / färdig satsvikt`

## Varför färdig vikt behövs

Vatten försvinner eller tillkommer under matlagning. Näringen försvinner normalt inte i samma proportion. Därför kan rå ingrediensvikt inte användas som slutlig portionsvikt. Väg gryta eller form tom, väg den färdiga maten och subtrahera kärlets vikt.

## Datakvalitet

Prioritera källor i denna ordning:

1. Näringsdeklarationen på den produkt som faktiskt används.
2. En dokumenterad livsmedelsdatabas.
3. Ett tydligt markerat standardvärde eller en uppskattning.

Dokumentera särskilt:

- avrunnen vikt för konserver
- fetthalt på köttfärs och mejeriprodukter
- faktisk mängd olja, smör, ost och sås
- om marinad eller stekfett lämnas kvar
- tillbehör som ris, bröd och gräddfil separat från huvudrätten

## Matlådor

Det mest flexibla är att lagra näring **per 100 g färdig mat** och sedan väga varje matlåda. Då kan olika personer eller dagar ha olika portionsstorlek.

Exempel: Om grytan innehåller 4 800 kcal och väger 3 000 g färdig är den 160 kcal per 100 g. En matlåda på 450 g innehåller då 720 kcal.

## Verktyg

Markdown-tabellen i [[../Mallar/Receptmall|Receptmallen]] är den beständiga dokumentationen. Excel eller Google Kalkylark kan fortfarande användas som räknemotor. Senare kan systemet kompletteras med ett CSV-register eller ett litet skript som räknar direkt från strukturerad ingrediensdata.
