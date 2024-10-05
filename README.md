# keyItaly

Progetto per il corso di TSW 23-24, sito di e-commerce per la vendita di tastiere per PC e accessori come switch e keycaps.

Le funzionalità sono elencante nel pdf insieme alla documentazione completa [Project proposal.pdf](https://github.com/g-cer/prova/blob/main/Project%20proposal.pdf)

## Installazione

1. Creare e popolare il database tramite gli script SQL "db\keyItaly.sql" e "db\insert.sql"

2. Modificare in "WebContent\WEB-INF\web.xml" il parametro "WEBCONTENT_PATH" con l'indirizzo completo della directory "\immaginiCatalogo"

3. Modificare in "WebContent\META-INF\context.xml" la propria password di accesso al server Mysql@localhost:3306

4. Tramite la shell dei comandi:
- Accedere alla cartella WebContent
- Creare il file WAR:
	- jar –cvf keyItaly.war .
 
 oppure esportare il file WAR tramite Eclipse

5. Copiare il file WAR nella cartella “webapps” di Tomcat

6. Lanciare il server Tomcat
