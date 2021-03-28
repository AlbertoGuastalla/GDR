# Gestione delle reti

<p align="center">
  <img src="https://lh3.googleusercontent.com/proxy/dzHa9t_P_PGCzs6hEFhdIUNU3SxpKwii3idrvifF-qtWrRxCqj0YLu3xFVsG2rJrSCAgPiKDe0KAKdwQiTUfBvsQRJDk84G_41_4Ly-jO11TTpSWNXqwmQ"/>
</p>

# Descrizione del progetto
# GitHub

Il sito è principalmente utilizzato dagli sviluppatori, che caricano il codice sorgente dei loro programmi e lo rendono scaricabile dagli utenti. Questi ultimi possono interagire con lo sviluppatore tramite un sistema di issue tracking, pull request e commenti che permette di migliorare il codice del repository risolvendo bug o aggiungendo funzionalità. Inoltre Github elabora dettagliate pagine che riassumono come gli sviluppatori lavorano sulle varie versioni dei repository.

GitHub fornisce anche altri servizi come Gist, strumenti per creare repository individuali e per le pagine web che possono essere modificate tramite un repository di Git, un servizio di hosting ed una piattaforma di statistiche sui siti web.

E’ un software per il controllo di versione distribuito tramite Git.

E’ possibile, attraverso un abbonamento (Team, Enterprise, One), usufruire di ulteriori servizi offerti dalla piattaforma stessa.

## Fault Management

  Quando avviene un evento di fallimento, il componente deve notificare il guasto 
  al gestore della rete usando protocolli tipo SMNP.
  ### Problemi ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) :
  - outage elettricita a livello di paese,
  - componenti hardware si rompono,
  - attacchi esterni verso il sistema di gestione delle reti (es. DOS),
  - Malfunzionamento o rottura di un servizio esterno a GitHub.
  ### Operazioni ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) :
  - hardware monitoring -> hardware failure detection -> operator notification 
  - fornire più servizi con funzionalità simili.
  - disponibilita servizio 24/7


## Accounting Management
  Limitazione spazio dedicato e limitato numero di operazioni che si possono
  effettuare sul progetto software. 
 ### Problemi ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) :
  - un utente o un gruppo di utenti può abusare delle risorse messe a disposizione 
    e condivise
  - gli utenti possono fare un uso inefficiente delle risorse del sistema
  ### Operazioni ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) :
  Nel caso di Github la maggior parte degli utenti sono esterni.
  - [Rate Limiting](https://docs.github.com/en/rest/overview/resources-in-the-rest-api#rate-limiting) per gli utenti (nel caso di utilizzo delle API).
  - limitazione nelòlo spazio di storage.

## Configuration Management
  E un processo per mantenere la consistenza della performance del servizio. 
  Il sistema deve aiutare l'operatore della rete affinche possa scegliere 
  il software piu appropriato per gestire la rete.
### Problemi ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) :
  - non riesco a determinare il componente da cambiare nel caso in cui i requisiti
    del sistema cambino
  - outages nel caso in cui viene modificato erroneamente un componente di sistema 
### Operazioni ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) :
  - startup/shutdown schede di rete 
  - assegnazione ip alle macchine 

## Performance Management
  Monitorare le componenti affinche si abbia la massima efficienza in termini di prestazioni
  dei componenti stessi.
### Problemi ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) :
  - costi elevati in quanto viene effettuato un uso eccessivo delle risorse (poca efficienza
    nell'utilizzo delle componenti)
  - Elevata latenza nei tempi di download / upload del codice sorgente.
### Operazioni ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) :
  - monitorare componenti affinche non vi siano colli di bottiglia o sprechi di risorse

## Security Management
  Meccanismi di protezione e controllo degli accessi (generazione chiavi crittografiche,
  password). Possiamo considerare la parte inerente agli accessi dell'organizzazione che
  eroga il servizio. Tutti i membri del team di sviluppo dovrebbero avere dei dati di 
  accesso affinche possano accedere alla rete (organizzazione) interna al servizio.
  ### Problemi ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) :
  - accessi non autorizzati (al manager e/o agli agents)
  ### Operazioni ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) :
  - log di tutti gli accessi effettuati alla rete 
  - segnalazione accessi fraudolenti


| Authors | Andrea Audenino <br> (<a href="andrea.audenino@edu.unito.it">andrea.audenino@edu.unito.it</a>) | Alberto Guastalla <br> (<a href="alberto.guastalla@edu.unito.it">alberto.guastalla@edu.unito.it</a>) | Daniele Serafini <br> (<a href="daniele.serafini@edu.unito.it">daniele.serafini@edu.unito.it</a>) | Giacomo Costarelli <br> (<a href="giacomo.costarelli@edu.unito.it">giacomo.costarelli@edu.unito.it</a>) |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Github URLs | <a href="https://github.com/Gilgames000">https://github.com/Gilgames000</a> |  <a href="https://github.com/AlbertoGuastalla">https://github.com/AlbertoGuastalla</a> | <a href="https://github.com/DanSeraf">https://github.com/DanSeraf</a> | <a href="https://github.com/giacomocostarelli">https://github.com/giacomocostarelli</a>  |    
