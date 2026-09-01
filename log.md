# Session slides — projektiloki

## Projektin tavoite
Konferenssi- ja community-sessioiden kalvot (PDF) yhdessä paikassa.

**Konteksti:** henkilökohtainen / Karlex Oy. GitHub-tili `spiik`.
**⚠️ Repo on JULKINEN** — kaikki mikä committoidaan on maailman luettavissa
pysyvästi, myös jos se myöhemmin poistetaan.

## Tilanne

### 2026-09-01 — Projekti perustettu
- Kansio `~/private/Session slides/`, julkinen repo `github.com/spiik/session-slides`.
- Runko: `pdf/` kalvoille, `README.md`, tämä loki.
- Käyttötarkoitus selvisi heti: **kalvot jaetaan yleisölle QR-koodilla** esityksen
  aikana. Repo on siis jakelukanava, ei arkisto.

### 2026-09-01 — Ensimmäiset kalvot: Trustworthy AI (projekti KnowledgeGoverned)

`pdf/trustworthy-ai.pdf` — *From Smart Answers to Trustworthy AI: Designing Governed
Copilot Studio Agents*, 23 kalvoa. Esitetään **2.9. ja 4.9.2026**.

**Sisältötarkistus ennen julkista pushia:** ei asiakasnimiä, ei tenant-tunnuksia, ei
MVP-/NDA-aineistoa. Metadatassa vain Kallen oma nimi ja PowerPoint-tuottaja. Kalvoilla
oleva evaluaatiodata (24/43 → 31/43 ilman muutoksia) on anonyymiä. → julkaisukelpoinen.

**GitHub Pages otettu käyttöön** (`main` / juuri), koska raw.githubusercontent tarjoilee
PDF:n `application/octet-stream`-tyyppisenä eli puhelin lataa sen sen sijaan että avaisi.
Pagesin kautta content-type on `application/pdf` ja kalvot aukeavat suoraan selaimeen.

**QR-koodin osoite:** `https://spiik.github.io/session-slides/pdf/trustworthy-ai.pdf`
Juuressa `index.html` listaa kalvot, jos joku menee osoitteen tyveen.

⭐ **Tiedostonimi on lukittu QR-koodiin.** Kun kalvoista tulee uusi versio (QR-koodi
lisättynä), se tallennetaan **täsmälleen samalla nimellä** `pdf/trustworthy-ai.pdf`.
Nimen vaihtaminen rikkoo painetun/kalvolla olevan QR-koodin. Pages päivittyy noin
minuutissa pushista.
