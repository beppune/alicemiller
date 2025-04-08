Gestione Accessi Datacenter, o gadc, è un'applicazione web che consente di gestire i dati e lo svolgimento della procedura di accessi fisici nei datacenter di Poste, nelle sue varianti.

- Gestire la configurazione dei siti
- Registrare i dati di una [[richiesta]]
- Gestire lo stato di una richiesta dalla creazione alla risoluzione
- Mantenere un'anagrafica di visitatori
- Mantenere un'anagrafica di richiedenti
- Permenttere l'accesso tramite credenziali di Poste agli operatori
- Mantenere i log delle operazioni effettuate
- Riservare alcune operazioni di alto livello a un ristretto numero di operatori
- Comunicare via mail automatiche il verificarsi di alcuni eventi
- Generare reportistica
- Configurare regole di validazione, generiche o temporanee, per le richieste
- Configurare operazioni ricorrenti in maniera semi-automatica

### Tecnologie utilizzate

- Database MySql
- Spring Boot
	- Vaadin Flow (interfaccia grafica)
	- Spring Security (autenticazione e aurizzazione)
	- Spring JDBC (connessione alla base di dati)
	- BIRT (reportistica)
- Git (controllo versione)
- Obsidian (note di sviluppo)