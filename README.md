# Pappas Mat

En personlig, versionshanterad kokbok byggd för [Obsidian](https://obsidian.md/) och GitHub.

## Struktur

- [[Recept/Index|Recept]] – färdiga recept sorterade efter kategori
- [[Näring/Index|Näring]] – metod och underlag för kalorier och makron
- [[Tekniker/Index|Tekniker]] – metoder, temperaturer och kökskunskap
- [[Ratios/Index|Ratios]] – grundförhållanden som gör recept skalbara
- [[Menyer/Index|Menyer]] – kompletta måltider och serveringsplaner
- [[Event/Index|Event]] – planerade mat- och dryckesevent, exempelvis ölprovningar
- [[Mallar/Receptmall|Receptmall]] – mall för nya recept
- `Bilder/` – bilder som används i anteckningarna

## Arbetsflöde

1. Skapa nya recept från `Mallar/Receptmall.md`.
2. Lägg receptet i rätt undermapp under `Recept/`.
3. Dokumentera använda vikter när näringsvärden ska beräknas.
4. Väg den färdiga satsen och räkna per 100 g eller per matlåda.
5. Länka till relevanta tekniker, ratios, tillbehör, menyer och event med Obsidian-länkar.
6. Uppdatera receptets anteckningar efter att det har lagats.
7. Commit:a förbättringarna till Git.

## Näringsmodell

Näringsvärden ska i första hand beräknas från den faktiska mängden av varje ingrediens:

`ingrediensens total = använd vikt i gram × värde per 100 g / 100`

När hela satsens energi och makron är summerade vägs den färdiga maten:

`per 100 g färdig mat = satsens total × 100 / färdig vikt`

`per matlåda = satsens total × matlådans vikt / färdig vikt`

Det gör att matlådor kan väga olika mycket utan att näringsberäkningen behöver göras om. Se [[Näring/Index|Näring]].

## Metadata

Recept använder YAML-frontmatter för att kunna sökas och filtreras i Obsidian:

- `kategori`
- `portioner`
- `aktiv_tid`
- `total_tid`
- `svårighet`
- `matlåda`
- `frysbar`
- `metoder`
- `ratios`
- `näringsberäknad`
- `taggar`
- `status`

## Statusvärden

- `utkast` – ännu inte testat
- `testat` – lagat minst en gång
- `favorit` – ett etablerat recept att återkomma till
