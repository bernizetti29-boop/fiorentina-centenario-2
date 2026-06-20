# AGGIORNAMENTO — Fiorentina Centenario (copia di lavoro `-2`)

> Fonte di verità sullo stato del progetto. Leggere all'inizio e aggiornare alla fine di ogni intervento.

**Ultimo aggiornamento:** 2026-06-19

## Cos'è
Pagina celebrativa a file singolo per il **centenario della Fiorentina (1926–2026)**.
Un'unica pagina HTML statica (`index.html`) con tutto incluso: stile CSS inline, dati e
schede di approfondimento (modali) in un oggetto JavaScript `CUR`, e immagini in `assets/img/`.

- `index.html` — la pagina completa (storia, cronostoria, trofei, undici leggende, campioni,
  Astori, Era Commisso, dirigenza, sezione "Per i Tifosi"). Le schede cliccabili aprono un
  modale con curiosità e foto.
- `assets/img/` — tutte le immagini (foto storiche, ritratti, stemmi).
- `CREDITS.md` — crediti e licenze delle immagini (anche elencati nel footer della pagina).
- `qr-centenario.png` — QR del progetto.

## ⚠️ Relazione con l'originale (QR code)
Esistono **due copie indipendenti**:
- `~/fiorentina-centenario` = **ORIGINALE**, quello puntato dal **QR code** (GitHub Pages). 🔒 **NON va MAI modificato.**
- `~/fiorentina-centenario-2` (questa) = **copia di lavoro ATTIVA**. **Tutte** le modifiche vanno fatte QUI.
  Dal 2026-06-19 è anch'essa **pubblica** e pubblicata su GitHub Pages:
  https://bernizetti29-boop.github.io/fiorentina-centenario-2/ (QR: `qr-seconda-versione.png`).

## Come si avvia
È una pagina statica: basta aprire `index.html` in un browser
(`open index.html`). Nessun build, nessuna dipendenza esterna a runtime
(i font sono caricati da Google Fonts via CDN).

## Ambiente
- Repo Git: `origin` → https://github.com/bernizetti29-boop/fiorentina-centenario-2.git (repo privato)
- Nessun toolchain richiesto per modificare/visualizzare la pagina.

## Registro operazioni
- **2026-06-20 — Claude (agente)** — **PUBBLICATE ONLINE tutte le modifiche** del giorno (commit `3fcffc5`
  su `main`, push su GitHub). Verificato che il sito pubblico è aggiornato:
  https://bernizetti29-boop.github.io/fiorentina-centenario-2/ (trovati i nuovi contenuti "Settore Giovanile"
  e pannello Viola Park). Il sito è ospitato da **GitHub Pages**, quindi accessibile 24/7 anche con il
  computer dell'utente spento e offline. Il QR da consegnare alla giuria è `qr-seconda-versione.png` (punta a
  quell'URL pubblico). Le note "non ancora pubblicato online" delle righe precedenti sono quindi superate.
- **2026-06-20 — Claude (agente)** — Sezione **Viola Park**: aggiunto un pannello descrittivo in evidenza
  (`.vp-gioiello`, grafica viola/oro con giglio decorativo) che amplia il racconto sul Viola Park come
  **gioiello architettonico** e **uno dei centri sportivi più moderni d'Europa** (progetto Studio Archea /
  Marco Casamonti, >120 M€ di capitali privati, modello ammirato nel mondo), sottolineando che è oggi uno
  degli elementi che rendono la Fiorentina invidiata in Europa e nel mondo. Posizionato subito sotto la
  presentazione, prima delle statistiche. Verifica visiva headless. NOTA: non ancora pubblicato online.
- **2026-06-20 — Claude (agente)** — Ampliati contenuti (dati verificati su Wikipedia, incrociati su più fonti
  da agenti di ricerca): (1) **Albo d'Oro** — aggiunti due blocchi di card cliccabili: **Settore Giovanile**
  (Campionato Primavera ×4 [1971·1980·1983·2026], Coppa Italia Primavera ×8, Supercoppa Primavera ×3,
  Torneo di Viareggio ×9) e **Fiorentina Femminile** (Scudetto 2016-17, Coppa Italia ×2 [2016-17·2017-18],
  Supercoppa 2018), ognuna con scheda di approfondimento (7 nuove voci `CUR`). Nuovo CSS `.albo-sub`,
  `.trofeo.giov/.femm`. (2) **Scheda Stadio Franchi**: +3 fatti (capienza ~43.000, scale elicoidali e vincolo
  1983, restyling 2024 per il centenario). (3) **Scheda Curva Fiesole**: +2 fatti (curva nord, spostamento in
  Curva Ferrovia dal 2024; gemellaggio col Verona 1976 e Torino). (4) **Sezione Viola Park**: nuovo blocco con
  i due stadi interni (Curva Fiesole ~3.000 / Davide Astori ~1.500) e "una casa per tutta la Viola"
  (maschile+femminile+giovanili, foresteria, ecc.). `CUR` rivalidato (JSON ok, 64 voci, nessuna card orfana).
  Verifica visiva headless. NOTA: non ancora pubblicato online.
- **2026-06-20 — Claude (agente)** — **Vincenzo Italiano: rimossa la foto.** Verificato su Wikimedia Commons
  che NON esiste alcuna foto libera di Italiano **da allenatore** senza un'altra società: esistono solo la
  foto 2024 in contesto Bologna e foto da giocatore del Padova (a figura intera ma altra società). Su
  indicazione dell'utente ("se non c'è una foto da allenatore, non mettere immagini"), tolta del tutto la foto
  dalla scheda `c-italiano` (eliminato `assets/img/c-italiano.jpg`, rimossi `img`/`credit` e la voce dai
  crediti). Conteggio crediti footer → 32. CUR rivalidato. NOTA: non ancora pubblicato online.
- **2026-06-20 — Claude (agente)** — Revisione foto di alcune persone (ricerca su Wikimedia Commons, solo
  immagini libere): (1) **Cecchi Gori** — aggiunta foto che prima mancava: `assets/img/p-cecchigori.png`
  (Vittorio Cecchi Gori, Nastro d'Argento 1989, Pubblico Dominio); collegata al modale `p-cecchigori` e
  aggiunta ai crediti. (2) **Ujfalusi** — su scelta utente **rimossa del tutto** la foto: era in maglia
  Galatasaró (partita contro la Fiorentina), e su Commons NON esiste alcuna foto libera in maglia viola;
  eliminato il file `assets/img/l-ujfalusi.jpg`, tolti `img`/`credit` dal modale e la voce dai crediti.
  Conteggio crediti footer aggiornato (resta 33). (3) **Italiano, Prandelli, Della Valle** — verificato che
  le foto attuali sono GIÀ le migliori libere disponibili (Prandelli è addirittura di Parma-Fiorentina 2008,
  vero contesto viola): nessun cambio. Oggetto dati `CUR` rivalidato (JSON ok, 57 voci). NOTA: non ancora
  pubblicato online.
- **2026-06-20 — Claude (agente)** — Sostituito il giglio sotto ogni titolo di sezione: la regola CSS
  `.sezione-titolo h2::after` usava il `⚜` testuale (U+269C, reso "fatto male"); ora usa l'emoji **`⚜️`**
  (coerente con i gigli dell'hero). Vale per tutte le sezioni. NOTA: non ancora pubblicato online. Restano in
  versione testuale alcuni piccoli `⚜` inline (es. "⚜ Modulo 4-3-3", "⚜ Trofei per competizione", eyebrow
  modali): non toccati perché non richiesti.
- **2026-06-20 — Claude (agente)** — Uniformati i gigli dell'hero: i due ai lati del badge "CENTENARIO ·
  DAL 1926 AL 2026" erano in versione testuale `⚜` (U+269C) e ora sono in versione **emoji `⚜️`**
  (U+269C+U+FE0F), identica al giglio sotto "A.C.F. Fiorentina" (`giglio-grande`). Nell'hero non restano
  altri gigli da convertire. NOTA: non ancora pubblicato online.
- **2026-06-20 — Claude (agente)** — Nell'hero spostata la scritta "👆 Tocca ogni scheda…": prima appariva
  affiancata al badge "CENTENARIO · DAL 1926 AL 2026" (stessa riga, per via di `display:inline-block`), ora è
  su una **riga dedicata sotto** il badge (incapsulati entrambi in un `div` blocco). Verifica visiva headless.
  NOTA: non ancora pubblicata online.
- **2026-06-20 — Claude (agente)** — Rimosso dall'hero (pagina d'apertura) il **giglio ⚜ grande sfocato di
  sfondo** (l'elemento `.giglio-bg`), su richiesta dell'utente. Lo sfondo dell'hero ora mostra solo lo
  skyline di Firenze; restano il piccolo giglio nitido sopra gli anni e il resto invariato. Verifica visiva
  con screenshot headless. NOTA: modifica non ancora pubblicata online (serve commit + push).
- **2026-06-19 — Claude (agente)** — **PUBBLICATA ONLINE la seconda versione** (su richiesta utente, per
  poterla inviare a una persona che deve valutarla): reso **pubblico** il repo `fiorentina-centenario-2` e
  attivato **GitHub Pages** (branch `main`, root). Sito raggiungibile da chiunque a
  **https://bernizetti29-boop.github.io/fiorentina-centenario-2/** (verificato HTTP 200, titolo corretto).
  Rigenerato `qr-seconda-versione.png` (QR viola #5a1a6e con didascalia "Seconda Versione") in modo che ora
  punti all'**URL pubblico** (non più al file locale). Link e QR sono condivisibili su WhatsApp/email.
- **2026-06-19 — Claude (agente)** — [superato dalla riga sopra] Prima generato un QR solo locale che
  puntava a `file://.../index.html`; sostituito perché non raggiungibile da altri dispositivi.
- **2026-06-09 — Claude (agente)** — Terzo intervento (autonomo, solo su `-2`): aggiunta una **sezione
  dedicata "Il Viola Park"** in fondo (dopo "Per i Tifosi", con voce di menu). Contiene: foto del
  risultato finale (tribuna gremita, FacolCup CC0), testo introduttivo, **6 card statistiche** (31 ettari,
  12 campi, 2 stadi/4.500 posti, 12 edifici, ~120 M€, 2023), un **grafico a barre** sul costo
  (preventivo 70 M€ → spesa finale ~112 M€), un **grafico a ciambella** sui 12 campi (7 naturali / 5
  ibridi) e una **timeline del cantiere** (2019 progetto → 5 feb 2021 inizio lavori → 4 ago 2023 fine
  lavori → 11 ott 2023 inaugurazione). Dati verificati su Wikipedia IT (progetto arch. Marco Casamonti,
  Studio Archea). NOTA: su Wikimedia Commons **non esistono foto libere del cantiere**, quindi la fase di
  costruzione è rappresentata dalla timeline. Rimossa la vecchia card "Il Viola Park" dalla griglia
  "Per i Tifosi" (ora superflua). Verifica visiva fatta con screenshot headless (Playwright).
- **2026-06-09 — Claude (agente)** — Secondo intervento (sempre solo su `-2`): (1) aggiunta foto
  all'allenatore **Fulvio Bernardini** (ritratto 1974, nessun club mostrato — su Commons non esiste
  una sua foto in maglia/contesto Fiorentina); per **Vincenzo Italiano** (su
  Commons solo foto col Bologna o da giocatore) l'utente ha scelto un **ritaglio stretto sul volto** della
  foto 2024, in modo che lo stemma del Bologna non sia visibile. (2) Risolto il
  **taglio della foto di Commisso** nella sezione "Era Commisso" (`object-position: center 20%` sulle
  `.prop-foto`). (3) Sostituita la foto di **Joe Barone** con un primo piano da solo, ritagliato in alta
  risoluzione dalla foto della conferenza stampa (andtrap, CC BY-SA 4.0). (4) In "Le Origini" rimossa la
  **foto di squadra** del 1931-32 e messo il ritratto del fondatore **Luigi Ridolfi** (immagine 1936, già
  nel progetto); per non duplicarla, il modale di Ridolfi in "Dirigenza" ora usa un altro ritratto
  (Ridolfi alla scrivania). Aggiornati alt-text e crediti (ora 32).
- **2026-06-09 — Claude (agente)** — Su richiesta utente, modifiche solo sulla copia `-2`:
  (1) ampliato l'approfondimento del **Viola Park** nel modale `i-violapark` (da 3 a 6 punti:
  inaugurazione 11/10/2023, investimento privato >100M€, ~25 ettari e dotazioni, prima squadra +
  femminile + giovanili in un'unica sede, i due stadi Curva Fiesole e Davide Astori, ruolo di Joe Barone);
  (2) sostituita l'immagine della **Curva** (`assets/img/i-curva.jpg`) da stadio vuoto a **tifosi in curva**
  (Curva Fiesole gremita — Pedro Varela, CC BY-SA 2.0);
  (3) rimossa dalla sezione **"Per i Tifosi"** la scheda "Il Simbolo / Giglio" (era ripetizione della
  sezione Origini); (4) sostituita la foto di **Joe Barone** (`assets/img/barone.jpg`) con una più bella
  (rinnovo Milenković, andtrap, CC BY-SA 4.0). Aggiornati alt-text e crediti nel footer.
- **2026-06-02 — (commit precedenti)** — Foto in maglia viola per i campioni mancanti e foto per Joe Barone;
  nuova sezione "L'Era Commisso" (Rocco Commisso + Joe Barone in memoria); sezione Origini con immagini migliori.
