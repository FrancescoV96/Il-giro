# Il Giro

**Il Giro** è una web app per organizzare il giro consegne giornaliero di un camion.

- **Giro di oggi**: inserisci i clienti da visitare (scelti dall'anagrafica o scritti a mano, uno per riga); l'app li riconosce automaticamente e calcola l'ordine migliore delle fermate partendo dal deposito.
- **Percorso per camion**: il calcolo usa [openrouteservice](https://openrouteservice.org) con profilo mezzi pesanti, tenendo conto di altezza, lunghezza, larghezza e peso del camion. Il percorso viene mostrato su mappa (Leaflet + OpenStreetMap) e si può aprire in Google Maps, anche a tratte, segnando le consegne fatte.
- **Clienti**: anagrafica con indirizzi, posizioni precise, alias e note di consegna.
- **Impostazioni**: deposito, dati del camion, chiave openrouteservice e copia di sicurezza (esporta/ripristina in JSON).

Tutti i dati restano salvati nel browser del dispositivo (localStorage). È un singolo file `index.html`, senza build: basta aprirlo o pubblicarlo con GitHub Pages.

Per usarla serve una chiave gratuita di openrouteservice, da inserire in *Impostazioni*.
