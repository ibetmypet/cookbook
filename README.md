# Pappas Mat

En personlig, versionshanterad kokbok byggd för [Obsidian](https://obsidian.md/) och GitHub.

## Struktur

- [[Recept/Index|Recept]] – färdiga recept sorterade efter kategori
- [[Tekniker/Index|Tekniker]] – metoder, temperaturer och kökskunskap
- [[Menyer/Index|Menyer]] – kompletta måltider och serveringsplaner
- [[Ölprovning/Index|Ölprovning]] – öltyper, smakreferenser och provningar
- [[Mallar/Receptmall|Receptmall]] – mall för nya recept
- `Bilder/` – bilder som används i anteckningarna

## Arbetsflöde

1. Skapa nya recept från `Mallar/Receptmall.md`.
2. Lägg receptet i rätt undermapp under `Recept/`.
3. Länka till relevanta tekniker, tillbehör och menyer med Obsidian-länkar.
4. Uppdatera receptets anteckningar efter att det har lagats.
5. Commit:a förbättringarna till Git.

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
- `taggar`
- `status`

## Statusvärden

- `utkast` – ännu inte testat
- `testat` – lagat minst en gång
- `favorit` – ett etablerat recept att återkomma till
