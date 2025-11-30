# Coming Soon Page

Una pagina "Coming Soon" moderna e responsive, ottimizzata per il deployment su Railway.

## Caratteristiche

- Design moderno e responsive
- Animazioni fluide
- Link ai social media (Facebook, Twitter, YouTube)
- Ottimizzato per mobile e desktop
- Pronto per il deployment su Railway

## Setup Locale

1. Installa le dipendenze:
```bash
npm install
```

2. Avvia il server di sviluppo:
```bash
npm start
```

3. Apri il browser su `http://localhost:3000`

## Deployment su Railway

### Prerequisiti
- Account Railway
- Repository Git (GitHub, GitLab, etc.)

### Passi per il Deploy

1. **Collega il repository a Railway:**
   - Vai su [Railway](https://railway.app)
   - Clicca su "New Project"
   - Seleziona "Deploy from GitHub repo"
   - Scegli questo repository

2. **Railway rileverà automaticamente:**
   - Il file `package.json` per le dipendenze
   - Lo script `start` per avviare il server
   - La porta da usare (Railway imposterà automaticamente `PORT`)

3. **Variabili d'ambiente (opzionale):**
   - Railway imposterà automaticamente `PORT`
   - Non sono necessarie altre configurazioni

4. **Deploy:**
   - Railway eseguirà automaticamente `npm install` e `npm start`
   - Il sito sarà disponibile su un URL Railway generato automaticamente

### Best Practices Implementate

✅ **Server Express** - Server Node.js per servire file statici  
✅ **Port dinamica** - Usa `process.env.PORT` per compatibilità Railway  
✅ **package.json** - Configurato con script e engines  
✅ **File statici** - Serviti correttamente tramite Express  
✅ **.gitignore** - Esclude node_modules e file non necessari  
✅ **Responsive Design** - Ottimizzato per tutti i dispositivi  

## Struttura del Progetto

```
comingsoon/
├── index.html      # Pagina principale
├── styles.css      # Stili CSS
├── server.js       # Server Express
├── package.json    # Dipendenze e configurazione
├── .gitignore      # File da ignorare
└── README.md       # Documentazione
```

## Personalizzazione

Per personalizzare la pagina:

1. **Testo**: Modifica il contenuto in `index.html`
2. **Colori**: Modifica i colori in `styles.css` (gradiente, colori social, etc.)
3. **Link Social**: Aggiorna gli href dei link social in `index.html`
4. **Copyright**: Modifica il testo nel footer

## Licenza

MIT
