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

Kalvojen lähdemateriaali, demovideo ja agentti ovat projektissa
[`KnowledgeGoverned`](../KnowledgeGoverned/log.md) — täällä on vain julkaistu PDF.

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

### 2026-09-01 (jatko) — v2 QR-koodilla livenä

Kalle latasi uuden version vanhalla pitkällä nimellä; sisältö siirrettiin lukitun nimen
`pdf/trustworthy-ai.pdf` päälle. **QR-koodi dekoodattiin** (OpenCV, kaikki 23 kalvoa
skannattu): kalvolla 2, osoite `https://spiik.github.io/session-slides/pdf/trustworthy-ai.pdf`
— merkilleen oikein. Tämä on ainoa tapa todentaa QR ennen kuin joku salissa skannaa sen.

Kalvon 2 tekstikerroksessa lukee yhä *"ADD QR CODE HERE"*, mutta QR-kuva peittää sen
kokonaan — todennettu renderöimällä kalvo kuvaksi. Ei toimenpiteitä.

✅ Pages tarjoilee uuden version (1 830 403 tavua). Valmis esityksiin 2.9. ja 4.9.

### 2026-09-19 — Nordic Summit -versio

Kalle toi `pdf/From_Smart_Answers_to_Trustworthy_AI-NordicSummit.pdf` (27 kalvoa, Nordic
Summit -pohja). Sama sisältö kuin `trustworthy-ai.pdf`, uusi pohja. Julkaistu lukitulla
nimellä **`pdf/trustworthy-ai-nordic-summit.pdf`** — sama sääntö kuin ennen: uusi versio
(QR-koodi lisättynä) tallennetaan täsmälleen tällä nimellä, ei muulla.

**Sisältötarkistus:** teksti ajettu CGI-asiakasrekisterin 178 aliasta vastaan, 0 osumaa.
Ei tenant-tunnuksia, ei PGI-aineistoa. Kalvolla 3 lukee vielä *"ADD QR CODE HERE"* — QR
puuttuu, koska osoite syntyy vasta tästä julkaisusta.

⚠️ PDF:n metadatassa `Title: Nordic Summit 2025`, `Author: Guro Faller` — pohjan
tekijän jäänne, ei asiakastietoa. Kerrottu Kallelle; korjataan jos hän haluaa.

**QR-koodin osoite:** `https://spiik.github.io/session-slides/pdf/trustworthy-ai-nordic-summit.pdf`
Alkuperäinen pitkänniminen tiedosto jätetty työkansioon commitoimatta.

### 2026-09-19 (jatko) — v2 QR-koodilla livenä

Kalle toi uuden version samalla pitkällä nimellä; sisältö siirretty lukitun nimen
`pdf/trustworthy-ai-nordic-summit.pdf` päälle. Muutokset: puhujakalvo uusittu, QR lisätty.
**QR dekoodattu** (OpenCV, kaikki 27 kalvoa 300 dpi): kalvolla 4, osoite
`https://spiik.github.io/session-slides/pdf/trustworthy-ai-nordic-summit.pdf` — oikein.
Tekstikerroksessa yhä *"ADD QR CODE HERE"*, QR-kuva peittää sen kuten edelliselläkin kerralla.
Metadata edelleen pohjan tekijän (Guro Faller / Nordic Summit 2025).
