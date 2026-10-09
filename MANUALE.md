# Claude Code + GitHub con il metodo APPO

*Un piccolo manuale per chi parte da zero.*

---

## 1. Perché il metodo APPO

Il **metodo APPO** (di Marco Costanzo, presentato su
[miglioramento.com/appo](https://miglioramento.com/appo/)) aiuta a migliorare un
po' ogni giorno grazie a **domande intenzionali** da porsi **al mattino** e
**alla sera**. Il nome è un acronimo:

| Lettera | Parola          | Domanda guida (mattino)                          |
|---------|-----------------|--------------------------------------------------|
| **A**   | **Aspirazione** | Quale aspirazione (o bisogno) guiderà la mia giornata? |
| **P**   | **Problema**    | Quale problema dovrò affrontare?                 |
| **P**   | **Progetto**    | Quale progetto svilupperò oggi?                  |
| **O**   | **Opportunità** | Sarò attento a cogliere le opportunità che si presenteranno? |

La sera ci si ferma a riflettere ("ogni giorno più saggi"): cosa è successo,
cosa ho imparato, cosa ho provato. Si scrivono le risposte e si registrano i
progressi, perché sono i piccoli passi quotidiani a fare la differenza. Il
metodo consiglia di provarlo per almeno **66 giorni**, il tempo che serve a
trasformare una pratica in abitudine.

In questo manuale useremo la stessa struttura per imparare a lavorare con
**Claude Code** e **GitHub**: ogni sessione di lavoro inizia con le quattro
domande APPO e finisce con la riflessione serale.

---

## 2. Le parole da conoscere (in 2 minuti)

| Termine | Cosa significa, in parole semplici |
|---|---|
| **GitHub** | Un sito dove si conservano i progetti (codice, testi, documenti) e se ne tiene la storia. |
| **Repository (repo)** | La "cartella" di un progetto su GitHub, con tutta la sua storia. |
| **Branch** | Una "copia di lavoro" del progetto dove fare modifiche senza toccare la versione principale (`main`). |
| **Commit** | Un salvataggio con una breve descrizione ("Aggiunto il manuale"). |
| **Push** | L'invio dei commit dal computer (o dalla sessione di Claude) a GitHub. |
| **Pull Request (PR)** | La richiesta di unire le modifiche di un branch in `main`, dopo averle controllate. |
| **Merge** | L'unione effettiva delle modifiche in `main`. |
| **Claude Code** | Un assistente che legge il tuo progetto, scrive e modifica file, esegue comandi e lavora con git e GitHub, su tua richiesta. |

---

## 3. Preparazione (una volta sola)

1. **Crea un account GitHub** su [github.com](https://github.com) e un
   repository (pulsante **New**). Va benissimo anche vuoto.
2. **Scegli dove usare Claude Code**:
   - **Nel browser / app (consigliato per iniziare)**: vai su
     [claude.ai/code](https://claude.ai/code), collega il tuo account GitHub
     quando ti viene chiesto e scegli il repository. Claude lavora in un
     ambiente sicuro nel cloud: non devi installare nulla.
   - **Sul tuo computer (terminale)**: segui le istruzioni di installazione su
     [code.claude.com/docs](https://code.claude.com/docs), poi apri il
     terminale nella cartella del progetto e scrivi `claude`.
3. **Prima sessione**: chiedi a Claude
   *"Esegui /init e crea un file CLAUDE.md che descriva questo progetto"*.
   Il file `CLAUDE.md` è la "memoria" del progetto: Claude lo rilegge ogni
   volta. Scrivici anche le tue preferenze (es. *"Rispondi sempre in italiano"*).

---

## 4. La sessione di lavoro secondo APPO

### Mattino – le quattro domande (5 minuti, su carta o in un file)

Prima di scrivere a Claude, rispondi per iscritto:

- **A – Aspirazione**: *Che cosa voglio ottenere oggi, e perché?*
  Es.: "Voglio che il mio sito abbia una pagina contatti, così i clienti mi
  trovano più facilmente."
- **P – Problema**: *Che cosa mi blocca o cosa non funziona?*
  Es.: "Non so scrivere HTML e il modulo attuale non invia le email."
- **P – Progetto**: *Qual è il compito concreto e piccolo che porto a termine
  oggi?*
  Es.: "Creare `contatti.html` con nome, email e messaggio."
- **O – Opportunità**: *Cosa posso imparare o sfruttare oggi?*
  Es.: "Chiedo a Claude di spiegarmi ogni passaggio: imparo le basi di HTML
  e cos'è una Pull Request."

### Durante il giorno – trasforma l'APPO in una richiesta a Claude

Le quattro risposte diventano quasi da sole un'ottima richiesta (prompt):

```text
Aspirazione: voglio una pagina contatti per il mio sito.
Problema: non conosco l'HTML e il modulo attuale non funziona.
Progetto di oggi: crea contatti.html con i campi nome, email e messaggio,
collegata dal menu della home.
Opportunità: spiegami in parole semplici cosa fai a ogni passaggio.
Prima mostrami un piano, poi aspetta la mia conferma.
```

Poi segui questo ciclo:

1. **Piano** – Claude propone cosa farà. Leggi e correggi se serve.
   (Nel terminale puoi attivare la *modalità piano* con `Shift+Tab`.)
2. **Esecuzione** – Claude modifica i file. Quando ti chiede un permesso
   (es. eseguire un comando), leggi cosa sta per fare prima di accettare.
3. **Verifica** – Chiedi: *"Mostrami le modifiche"* oppure *"Come posso
   provarlo?"*. Non accettare ciò che non capisci: chiedi spiegazioni.
4. **Salvataggio su GitHub** – Chiedi: *"Fai commit e push sul branch"*.
   Quando sei soddisfatto: *"Apri una Pull Request"*.
5. **Revisione** – Su GitHub apri la PR, scheda **Files changed**, controlla
   e poi premi **Merge**. Le modifiche entrano in `main`.

### Sera – la riflessione ("ogni giorno più saggi")

Ripercorri la giornata e scrivi:

- *Ho raggiunto il Progetto di oggi?* (sì / in parte / no)
- *Il Problema si è risolto o è cambiato?*
- *Quale Opportunità ho colto? Cosa ho imparato di nuovo?*
- *Cosa ho provato?* (soddisfazione, frustrazione, curiosità…)
- *Cosa farò diversamente domani?* → se è una regola utile, aggiungila a
  `CLAUDE.md` così anche Claude se ne ricorderà.

---

## 5. Diario APPO (modello da copiare)

Crea nel repository un file `diario-appo.md` e aggiungi una voce al giorno.
In 66 giorni avrai la storia dei tuoi progressi (e GitHub conserverà tutto).

```markdown
## Giorno 1 – 2026-10-09

**Mattino**
- A – Aspirazione:
- P – Problema:
- P – Progetto:
- O – Opportunità:

**Sera**
- Progetto completato? sì / in parte / no
- Cosa ho imparato:
- Emozione principale:
- Domani farò diversamente:
- PR / commit del giorno:
```

Puoi anche chiedere a Claude: *"Aggiungi la voce di oggi a diario-appo.md con
queste risposte: …"*.

---

## 6. Frasi pronte per Claude

| Voglio… | Scrivi a Claude |
|---|---|
| capire un progetto | "Spiegami com'è organizzato questo repository, in parole semplici." |
| un piano prima di agire | "Proponi un piano e aspetta la mia conferma prima di modificare file." |
| vedere le modifiche | "Mostrami e spiegami le modifiche che hai fatto." |
| salvare il lavoro | "Fai commit con un messaggio chiaro e push sul branch." |
| far controllare il lavoro | "Apri una Pull Request con una descrizione delle modifiche." |
| annullare | "Annulla l'ultima modifica e torna com'era prima." |
| ricominciare pulito | `/clear` (nuova conversazione) |
| aiuto sui comandi | `/help` |

---

## 7. Regole d'oro per principianti

1. **Un Progetto piccolo al giorno.** Meglio una cosa finita che tre a metà.
2. **Prima il piano, poi le modifiche.**
3. **Leggi prima di approvare** comandi e merge.
4. **Mai password o chiavi segrete** nei file o nei messaggi: finirebbero su GitHub.
5. **Lavora su un branch** e unisci in `main` solo tramite Pull Request.
6. **Se non capisci, chiedi a Claude di spiegare**: è parte dell'Opportunità.
7. **Scrivi il diario ogni sera**: è lì che si vede il miglioramento.

---

*Fonti sul metodo APPO: [miglioramento.com/appo](https://miglioramento.com/appo/),
[metodoappo.com](https://metodoappo.com/), libro "Il metodo APPO" di Marco
Costanzo. Documentazione di Claude Code: [code.claude.com/docs](https://code.claude.com/docs).*
