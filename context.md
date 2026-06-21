# Vitalma — kontext projektu

> Stav k 21. 6. 2026. Tento soubor slouží k navázání práce (i v nové session / přes GitHub).

## O co jde
Tvorba **vizuální identity pro domov seniorů Vitalma** + **prezentační microsite**, kterou se brand odprezentuje klientovi. Jde o **tender** proti stávajícímu dodavateli (jeho cena: 90 000 Kč). Naše strategie: překvapit kvalitou + konkurovat cenou. Při výhře navazuje kompletní identita + brand manuál + jednotlivé vizuály.

## Brand brief (esence)
- **Pocity:** důvěra, klid, bezpečí, důstojnost, zázemí, odbornost, péče.
- **Dvojí cílovka:** senior (primární — musí se mu to hlavně líbit, řešit čitelnost) + jeho děti 40–50 (rozhodují, chtějí moderní/stylové).
- **Tonalita:** hezké a stylové ANO; prémiové NE; agresivně zdravotnické (červený PROMEDICUS) NE.
- Plný brief: [Vitalma_zadani_brand.md](Vitalma_zadani_brand.md)

## Designová rozhodnutí
- **Název:** Vitalma (zadán, neměnit).
- **Logo:** měkký geometrický wordmark s otevřenými zaoblenými tvary. Motiv = **apex (špička V/A/M) + tečka**. Tečka = „jiskra života / člověk".
  - Vývoj: v1 = tenký ostrý → zamítnuto (špatná čitelnost pro seniory, chladné). **v2 = bold + rounded + tečky nad apexy = zvolený směr.**
  - **Brandmark:** z písmene **V + tečka** lze odvodit samostatný symbol (ikona/favicon/odznak). Doporučeno.
- **Barvy:**
  - Zelená (primární): `#4A7A4A`
  - Krémová (podklad): `#F5EDD8`
  - Tmavá zelená (pattern/hloubka): `#376337`
  - Akcent modrá (tečka): `#6FA8C7` — **PLACEHOLDER, čeká na přesný HEX z loga**
- **Typografie:**
  - Wordmark: custom měkký geometrický sans (v prezentaci dočasně Fredoka jako placeholder).
  - Claim/nadpisy: **Marcellus** (doporučeno — římské kapitálky, důstojné, čitelnější než původní Bely). Alternativa Fraunces. Zvažoval se i sans claim (cohesive, ale tenký/studenější).
  - Text: **Outfit**.
  - Od **Bely** (high-contrast serif) doporučeno odejít — tenké tahy mizí v malém, vyznívá premium.
- **Claim:** zatím nefinalizován („Feels like home" byl jen placeholder).
- **Pattern:** `SVG/pattern.svg` = opakovaný motiv V+tečka, fill `#376337`.

## Deliverable: prezentační web
- **`web/index.html`** — editorial brand-prezentace, 9 sekcí (inspirace: https://altrum-template.webflow.io/).
  - Hero → 01 Koncept (7 pocitů) → 02 Logo → 03 Symbol → 04 Barvy → 05 Typografie → 06 Pattern → 07 Aplikace (hlavičkový papír, smlouva, social post) → závěr.
- **`web/pattern.svg`** — kopie patternu (web je self-contained).
- Lokální náhled: `server.js` + `.claude/launch.json` (Node static server, port 8137).

## Co je placeholder / čeká na doplnění
1. **Logo** ✅ DODÁNO (`SVG/logo.svg`, monochromatický krémový wordmark) a zapojené do prezentace přes CSS mask. Pozor: žádná modrá tečka — logo je jednobarevné.
2. **V-symbol (brandmark)** — v sekci 03 zatím **crop wordmarku přes mask** (odhadnuté souřadnice). Ideálně dodat samostatné SVG symbolu.
3. **Claim** (text + finální font serifa/sans) — všude „Claim placeholder".
4. **Texty** — koncept a popisky jsou návrh, k přepsání.
5. **Credit** v závěru („eVisions").

## Stav assetů
- `SVG/pattern.svg` ✅ (+ kopie `web/pattern.svg`)
- `SVG/logo.svg` ✅ (+ kopie `web/logo.svg`) — krémový wordmark, viewBox 780×155
- `JPG/` mockupy (pattern, signage, logo), `psd/` zdrojové soubory
- Samostatný V-symbol ❌ (zatím crop z wordmarku)

## Reference
- Inspirace web: https://altrum-template.webflow.io/
- Rešerše 15 evropských brandů domovů seniorů (barvy, loga, positioning) — viz historie session / artifact.

## Další kroky
- Dodat logo SVG + hexy → finalizovat prezentaci.
- Rozhodnout claim (font + text).
- Volitelně přidat sekce: varianty loga na podkladech, dos & don'ts, proces.
