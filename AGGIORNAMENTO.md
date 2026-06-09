# AGGIORNAMENTO — Fiorentina Centenario (copia di lavoro `-2`)

> Fonte di verità sullo stato del progetto. Leggere all'inizio e aggiornare alla fine di ogni intervento.

**Ultimo aggiornamento:** 2026-06-09

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

## Come si avvia
È una pagina statica: basta aprire `index.html` in un browser
(`open index.html`). Nessun build, nessuna dipendenza esterna a runtime
(i font sono caricati da Google Fonts via CDN).

## Ambiente
- Repo Git: `origin` → https://github.com/bernizetti29-boop/fiorentina-centenario-2.git (repo privato)
- Nessun toolchain richiesto per modificare/visualizzare la pagina.

## Registro operazioni
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
