# Come creare un bot telegram  
## Prima parte: chat bot  
Telegram ha due tipi di bot: chat bot e inline bot. I chat bot usano i comandi (come `/start`, `/help` ) per
interagire tra utenti. Gli inline bot possono invece essere chiamati da qualsiasi parte e aiutano gli utenti a
trovare e inviare contenuti dal vostro bot a qualsiasi chat che desiderano. In questa sede ci occupiamo dei chat bot.  
### Step 0.1: Scaricare Node.js e npm
Qui ci sono i link alla versione di [Node.js](https://hackerstribe.com/tag/node-js/) che useremo per questo workshop:  
Windows: <https://nodejs.org/dist/v6.6.o/node--v6.6.o--x64msi>  
MacOS: <http://nodejs.org/dist/v6.6.o/node--v6.6.o.pkg>  
Linux: dovreste già sapere come procurarvi Node.js  
### Step 0.2: Telegram  
Prima di fare un [Bot Telegram](https://hackerstribe.com/tag/bot-telegram/), avrete bisogno di un **account Telegram**. Andate su [telegram.org/dl](https://desktop.telegram.org/) e
create il vostro account.  
## Step 1: Creiamo la directory di progetto  
Ora che abbiamo Node.js e npm installati e il nostro account Telegram è pronto, possiamo partire col
nostro lavoro. Aprite il vostro terminale preferito a digitate questi comandi:  
```  
mkdir codeday-telegram-bot  
cd codeday-telegram-bot  
```
Adesso che abbiamo una directory per il nostro bot Telegram, abbiamo bisogno di un `package.json` , se
non siete neofiti di Node.js, non è necessario che vi spieghi a cosa serve. Altrimenti sappiate che molto
banalmente si può considerare come un descrittore del nostro progetto. Un file che indica nome,
descrizione e fra le altre cose anche le dipendenze (intese come pacchetti software) necessari al nostro
programma per funzionare.
Per crearlo molto semplicemente, dalla directory del nostro progetto lanciamo il comando:
```  
npm init   
```
Questo dirà al client **npm** di inizializzare la nostra project directory con un `package.json` predefinito.
Cliccate Invio a tutti i prompts, possiamo occuparci di “compilaro” più tardi.
