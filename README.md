# New York 2026 · putni pratilac

Web aplikacija za putovanje u New York od 5. do 14. prosinca 2026., napravljena prema putnom vodiču.

**Što sadrži**
- **Danas**: odbrojavanje do polaska, a za vrijeme puta plan tekućeg dana s oznakom što je „sada“ (po njujorškom vremenu)
- **Plan**: svih 10 dana, s kvačicama, savjetima, mjestima i Google Maps rutama
- **Troškovi**: unos po danima u $ ili €, slikanje računa, porez i napojnica, budžet po kategorijama
- **Popisi**: prije puta, pakiranje i shopping (možete dodati i svoje stavke)
- **Info**: letovi, hoteli, kalkulator dolara i napojnice, postavke i sigurnosna kopija

## Podaci

Sve se sprema **samo na uređaju** (localStorage za podatke, IndexedDB za slike računa). Nema servera ni prijave: svatko tko otvori aplikaciju ima svoju verziju. Pri prvom otvaranju aplikacija pita za ime.

Ako se obrišu podaci preglednika, brišu se i podaci aplikacije. Zato redovito napravite **Info → Sigurnosna kopija → Izvezi kopiju**. Kopiju možete vratiti na istom ili drugom uređaju.

## Instalacija na mobitel

- **iPhone (Safari):** Dijeli → Dodaj na početni zaslon
- **Android (Chrome):** izbornik ⋮ → Instaliraj aplikaciju / Dodaj na početni zaslon

Nakon prvog otvaranja aplikacija radi i bez interneta, osim Google Maps ruta.

## Objava (GitHub Pages)

Settings → Pages → Source: *Deploy from a branch* → Branch: `main`, mapa `/ (root)` → Save.
Aplikacija je zatim na `https://barbararacki.github.io/Newyork/`.

Kod promjene aplikacije povećajte `VERSION` u `sw.js` kako bi mobiteli preuzeli novu verziju.

## Datoteke

| Datoteka | Namjena |
|---|---|
| `index.html` | cijela aplikacija (HTML, CSS, JavaScript i podaci o putovanju) |
| `sw.js` | rad bez interneta |
| `manifest.webmanifest`, `icons/` | instalacija na početni zaslon |
