## KeyItaly
Realizzato per il corso di Tecnologie per lo Sviluppo Web (TSW) 2023/2024. 

Per una descrizione dettagliata delle funzionalità e della documentazione, consulta il file [Project proposal.pdf](https://github.com/g-cer/ProgettoTsw23-24/blob/main/Project%20proposal.pdf).

## Requisiti
- **Java JDK** (versione 11)
- **Tomcat** (versione 9.0)
## Installazione

1. Esegui gli script SQL presenti nella cartella `db` `keyItaly.sql` per la creazione e `insert.sql` per il popolamento del db.

2. Modifica il parametro `WEBCONTENT_PATH` nel file `WebContent\WEB-INF\web.xml` con il percorso completo della directory `\immaginiCatalogo` nel tuo ambiente locale.

3. Apri il file `WebContent\META-INF\context.xml` e inserisci la tua password per l'accesso al server MySQL su `localhost:3306`.

4. Accedi alla cartella `WebContent` tramite terminale e crea il file WAR con il comando:
	```bash
	jar -cvf keyItaly.war .
	```
	In alternativa, esporta il file WAR direttamente tramite Eclipse.

5. Copia il file WAR nella cartella `webapps` di Tomcat.

6. Avvia il server Tomcat per eseguire l'applicazione, il sito sarà accessibile tramite il browser all'indirizzo `http://localhost:8080/keyItaly`
