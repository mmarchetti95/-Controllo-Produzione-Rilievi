# Come aggiungere un nuovo tool al portale

## Cosa ti serve
- Il file HTML del nuovo tool
- Accesso a GitHub (github.com) con l'account mmarchetti95

---

## Passo 1 — Carica il file HTML su GitHub

1. Vai su **github.com** e apri il repository **-Controllo-Produzione-Rilievi**
2. Clicca sulla cartella **`tools`**
3. Clicca **"Add file"** → **"Upload files"**
4. Trascina il tuo file HTML oppure clicca "choose your files"
5. In fondo alla pagina clicca il pulsante verde **"Commit changes"**

---

## Passo 2 — Modifica index.html

1. Torna alla root del repository (clicca **-Controllo-Produzione-Rilievi** in alto)
2. Clicca su **`index.html`**
3. Clicca l'icona della **matita ✏️** in alto a destra per modificare
4. Trova questa sezione nel file (circa a metà):

```js
// ═══════════════════════════════════════════════
//  CONFIG — modifica qui per aggiungere tool
// ═══════════════════════════════════════════════
const TOOLS = [
```

5. Scorri fino alla **fine dell'array**, prima della riga `];`
6. Aggiungi una virgola dopo l'ultimo tool e incolla questo blocco:

```js
  {
    id: "nome-univoco",
    nome: "Nome del Tool",
    sub: "Descrizione breve",
    icona: "ti-chart-bar",
    cat: "Report",
    colore: "#34d058",
    url: "https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/tools/nome-file.html"
  },
```

---

## Passo 3 — Personalizza i campi

| Campo | Cosa mettere | Esempio |
|-------|-------------|---------|
| `id` | Nome univoco senza spazi | `"nuovo-report"` |
| `nome` | Nome visualizzato nel portale | `"Report Mensile"` |
| `sub` | Sottotitolo descrittivo | `"Riepilogo mensile"` |
| `icona` | Icona da Tabler Icons | `"ti-chart-bar"` |
| `cat` | Categoria nella sidebar | `"Rilievo"` o `"Produzione"` o `"Report"` |
| `colore` | Colore esadecimale dell'icona | `"#34d058"` |
| `url` | URL completo del file | vedi sotto |

### URL del file
Sostituisci `nome-file.html` con il nome esatto del file che hai caricato:
```
https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/tools/nome-file.html
```

### Icone disponibili
Vai su **tabler.io/icons**, cerca l'icona che vuoi e copia il nome.
Esempi utili:
- `ti-map-2` — mappa
- `ti-drone` — drone
- `ti-satellite` — GNSS
- `ti-chart-bar` — grafico
- `ti-file-description` — report
- `ti-tool` — strumento
- `ti-flame` — ATEX
- `ti-clipboard-list` — work order
- `ti-camera` — fotografia
- `ti-ruler` — misura

### Colori suggeriti
- Arancione: `#f0a500`
- Verde acqua: `#00d4aa`
- Blu: `#4d8fff`
- Blu scuro: `#1a5fa8`
- Viola: `#a78bfa`
- Verde: `#34d058`
- Rosso: `#ff5c5c`
- Arancione chiaro: `#fb923c`

---

## Passo 4 — Salva le modifiche

1. In fondo alla pagina di modifica clicca **"Commit changes"**
2. Nella finestra che appare clicca di nuovo **"Commit changes"**
3. Aspetta **1-2 minuti** che GitHub Pages si aggiorni
4. Apri il portale — il nuovo tool apparirà nella sidebar e nella home

---

## Esempio completo

Vuoi aggiungere un tool chiamato "Report Mensile" con il file `report_mensile.html`:

```js
  {
    id: "report-mensile",
    nome: "Report Mensile",
    sub: "Riepilogo produzione",
    icona: "ti-chart-bar",
    cat: "Report",
    colore: "#34d058",
    url: "https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/tools/report_mensile.html"
  },
```

---

## Attenzione ai nomi file con spazi

Se il nome del file contiene spazi (es. `Report Mensile.html`), nell'URL sostituisci gli spazi con `%20`:

```
url: "https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/tools/Report%20Mensile.html"
```

Oppure, più semplice: rinomina il file senza spazi prima di caricarlo (`report_mensile.html`).

---

*Portale Controllo Produzione Rilievi — v1.0*
