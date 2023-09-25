# Progetto Express App

Questo progetto è un'applicazione web di base realizzata con Express.js. L'app implementa un semplice sistema di autorizzazione basato su password.

## Installazione e Setup

Prima di eseguire l'applicazione, è necessario installare le dipendenze. Aprire un terminale nella directory del progetto e eseguire il seguente comando:

```bash
npm install
```

## Struttura del Progetto

Il progetto contiene diversi file e directory:

- `index.js`: Il file principale dell'applicazione.
- `public/`: Contiene i file HTML che saranno serviti dall'applicazione.
  - `index.html`: La pagina principale dell'app.
  - `secret.html`: Una pagina segreta accessibile solo dopo l'autorizzazione.

## Esecuzione dell'Applicazione

Dopo aver installato le dipendenze, è possibile avviare l'applicazione con il seguente comando:

```bash
npm start
```

L'applicazione sarà in esecuzione all'indirizzo [http://localhost:3000](http://localhost:3000).

## Funzionalità

L'applicazione ha due route principali:

- `GET /`: Serve la pagina principale `index.html`.
- `POST /check`: Verifica se l'utente è autorizzato e, in caso affermativo, serve la pagina `secret.html`. Altrimenti, reindirizza l'utente alla pagina principale.

L'autorizzazione dell'utente è determinata dalla funzione middleware `passwordCheck`, che controlla se la password fornita è corretta.

## Contribuire

Se desiderate contribuire al progetto, create una Pull Request con le vostre modifiche.

## Licenza

Questo progetto è rilasciato sotto la licenza MIT. Consultare il file `LICENSE` per ulteriori dettagli.

---

Questo `README` fornisce una descrizione di base del progetto e delle sue funzionalità. È possibile aggiungere ulteriori dettagli o sezioni a seconda delle esigenze del progetto.
