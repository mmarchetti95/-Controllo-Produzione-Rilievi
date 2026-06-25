# 🗺️ Controllo Produzione Rilievi — Portale Tool

> Portale web unificato per la gestione e l'accesso ai tool di produzione e rilievo di **Eagle Projects SRL**.

🔗 **[Apri il Portale](https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/)**

---

## 📋 Descrizione

Un'unica interfaccia centralizzata che raggruppa tutti i tool HTML dedicati al controllo della produzione, rilievi topografici e gestione dei work order. Sostituisce l'accesso frammentato a più file separati, offrendo un punto di accesso rapido e organizzato per il team.

---

## 🛠️ Tool disponibili

| Tool | Categoria | Descrizione |
|------|-----------|-------------|
| Dashboard Mobile Mapping | Rilievo | Monitoraggio produzione Mobile Mapping con mappa Leaflet e import shapefile |
| Drone Survey Dashboard | Rilievo | Dashboard produzione Drone Survey con pannelli laterali e mappa |
| GNSS Report | Report | Report giornaliero GNSS con import Excel/CSV ed export PDF |
| Produzione ATEX | Produzione | Gestione produzione ATEX con mappa e tabelle dati |
| Report WO / Work Orders | Report | Report produzione Work Orders con visualizzazione shapefile |

---

## 📁 Struttura del repository

```
/
├── index.html          # Portale principale (launcher)
└── tools/
    ├── dashboard_mobile_mapping_v2.html
    ├── drone_survey_dashboard.html
    ├── gnss_report_v1.html
    ├── Produzione_ATEX_-_v1.html
    └── report_produzione_WO_v12_1.html
```

---

## 🚀 Come utilizzarlo

### Accesso diretto
Apri il portale dal browser all'indirizzo:
```
https://mmarchetti95.github.io/-Controllo-Produzione-Rilievi/
```

### Condivisione interna
- **Teams**: incolla il link direttamente in una chat o canale
- **SharePoint**: aggiungi il link al menu di navigazione del sito aziendale
- **Browser**: salva come preferito per accesso rapido

> ✅ Compatibile con tutti i browser moderni (Edge, Chrome, Firefox).  
> ✅ Accessibile da qualsiasi dispositivo con connessione internet.

---

## ➕ Aggiungere un nuovo tool

1. Carica il file HTML nella cartella `tools/`
2. Apri `index.html` e individua l'array di configurazione dei tool (sezione `toolsConfig`)
3. Aggiungi un nuovo oggetto seguendo questo schema:

```javascript
{
  name: "Nome Tool",
  description: "Breve descrizione del tool",
  category: "Rilievo", // oppure "Produzione" o "Report"
  url: "./tools/nome_file.html",
  icon: "📊"           // emoji o classe icona
}
```

4. Fai commit e push — GitHub Pages si aggiorna automaticamente in pochi secondi.

---

## 🏢 Contesto aziendale

- **Azienda**: Eagle Projects SRL
- **Ambiente**: Microsoft 365
- **Hosting**: GitHub Pages
- **Utilizzo**: Team operativo produzione e rilievi

---

## 📄 Licenza

Uso interno Eagle Projects SRL — tutti i diritti riservati.
