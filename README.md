# 🗺️ Itinerář Francie & Španělsko 2026

Webový itinerář na cestu po Francii a Španělsku, léto 2026.  
Vytvořeno jako HTML stránka s vizuálním přehledem po etapách.

🔗 **Živá stránka:** https://andostalkova.github.io/itinerar2026/

---

## Termín a trasa

**16. července – 7. srpna 2026** · 23 dní

```
Praha → Lago di Garda → Côte d'Azur → Provence → Barcelona → San Sebastián → La Rochelle → Paříž → Praha
```

| Etapa | Místo | Termín | Nocí | Ubytování |
|-------|-------|--------|------|-----------|
| I. | Lago di Garda / Verona | 17. 7. | 1 | Booking + snídaně |
| II. | Côte d'Azur | 18.–20. 7. | 3 | Camp du Domaine |
| III. | Provence / Luberon | 21.–23. 7. | 3 | Camping Verbéla Village |
| IV. | Barcelona / Tamarit | 25. 7. – 1. 8. | 8 | Tamarit Beach Resort |
| V. | San Sebastián | 2. 8. | 1 | dořešit |
| V. | La Rochelle | 3. 8. | 1 | dořešit |
| V. | Paříž | 4.–5. 8. | 2 | Booking + snídaně |

---

## Soubory v repozitáři

| Soubor | Popis |
|--------|-------|
| `index.html` | Hlavní itinerář — barevný přehled po etapách, kompaktní layout |
| `Francie_Spanelsko_2026_tisk.html` | Verze pro tisk — čistá tabulka na A4, černobílá |
| `README.md` | Tento soubor |

---

## Jak stránku upravit

Všechny úpravy se dělají přímo v HTML souboru. Nejjednodušší způsob:

1. Klikni na soubor v repozitáři
2. Klikni na **ikonu tužky** (Edit this file)
3. Uprav co potřebuješ
4. Klikni **Commit changes**
5. Stránka se automaticky aktualizuje za 1–2 minuty

### Co nejčastěji budeš chtít změnit

**Přidat odkaz na ubytování:**
```html
<!-- najdi řádek s ubytováním, např.: -->
<div class="day-stay">Booking + snídaně</div>

<!-- a přidej odkaz: -->
<div class="day-stay"><a href="https://www.booking.com/..." target="_blank" rel="noopener">Booking + snídaně</a></div>
```

**Přidat bistro nebo restauraci** — až doplníš tipy, přidej je do sloupce `day-program`:
```html
<div class="day-program">Pláž, odpočinek · 🍽️ Le Petit Bistro (Tripadvisor 4.8)</div>
```

**Odškrtnout položku v „K dořešení"** — najdi příslušné `<li>` v sekci `.todo` a buď ho smaž, nebo přidej přeškrtnutí:
```html
<li><s>Rezervace Camp du Domaine</s> ✓</li>
```

---

## Jak použít pro další cestu

1. Klikni na **Code → Download ZIP** a ulož si kopii
2. Nebo v GitHubu použij **Fork** (tlačítko vpravo nahoře) — vytvoří ti kopii repozitáře
3. Přejmenuj repozitář (Settings → Repository name)
4. V `index.html` najdi a nahraď:
   - název cesty v `<title>` a `<h1>`
   - data a destinace v sekci `header` a `.route`
   - jednotlivé `.etapa` sekce s novými dny
   - ubytování a program
5. Nezapomeň aktualizovat README (tento soubor) 😊

---

## Technické poznámky

- Stránka nepoužívá žádné externí závislosti kromě Google Fonts
- Fonty: Fraunces, Cormorant Garamond, JetBrains Mono
- Responzivní — funguje na mobilu i desktopu
- Tisková verze má vlastní `@media print` stylesheet
- Hostováno přes **GitHub Pages** (větev `main`, kořenová složka)

---

*Vytvořeno: květen 2026*
