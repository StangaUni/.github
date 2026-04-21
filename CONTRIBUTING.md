# Guida alla contribuzione

Grazie per l'interesse nel migliorare questi materiali. Le contribuzioni sono benvenute tramite **pull request**: ogni PR viene revisionata e approvata esclusivamente dal maintainer, che è l'unico ad avere accesso in scrittura alle repository e al sito.

> A meno che non sia diversamente specificato nella PR stessa, il tuo **nome utente GitHub** e un **link al tuo profilo** saranno aggiunti sul sito: nella pagina delle informazioni e nelle sezioni dove il contributo è stato apportato. Non si guadagna nulla lavorando gratuitamente per gli altri, ma è giusto riconoscere l'impegno di ognuno, per quanto grande o piccolo.

---

## Cosa si può contribuire

- Correzioni di errori (concettuali, formali, tipografici)
- Aggiunte o miglioramenti agli appunti esistenti
- Nuovi esercizi o soluzioni
- Miglioramenti alla struttura dei file o alle risorse grafiche

Non verranno accettate PR che includono materiale didattico originale (slide, registrazioni, testi di esame): questi rimangono di proprietà dei rispettivi docenti e dell'Università di Padova.

---

## Struttura delle repository

Ogni repository segue la convenzione di denominazione `AASS_materia`:
- `AA` = ultime due cifre dell'anno di inizio dell'a.a. (es. `25` per 2025)
- `SS` = ultime due cifre dell'anno di fine (es. `26` per 2026)
- `materia` = nome della materia in minuscolo con underscore

Esempio: `2526_algebra_e_matematica_discreta`

### Cartelle tracciate

Non tutte le cartelle presenti localmente sono incluse nel repository: ogni repository ha un proprio `.gitignore` che esclude cartelle non ancora pubblicate. Le cartelle attualmente tracciate e aperte a contribuzioni sono:

```
repository/
├── Riassunti/        # Riassunti sintetici degli argomenti
├── Utils/            # Materiale di supporto (schemi, schede riassuntive)
└── assets/           # Immagini e diagrammi SVG
```

La cartella `Esercizi/` è al momento esclusa temporaneamente: il sito è ancora in fase di avvio e la sua pubblicazione è stata posticipata per non sovraccaricare il lavoro iniziale. Verrà resa disponibile — e aperta a contribuzioni — non appena il contenuto sarà allineato.

Prima di aprire una PR, verifica sempre il `.gitignore` della repository specifica per capire quali percorsi sono tracciati. Non proporre modifiche a cartelle che non compaiono nel repository remoto.

### Convenzioni sui nomi dei file

| Tipo | Posizione | Formato | Esempio |
|------|-----------|---------|---------|
| Riassunti | `Riassunti/` | `NN. Titolo Descrittivo.md` | `03. Algebra Lineare.md` |
| Diagrammi SVG | `assets/` | `nome.svg` / `nome_scuro.svg` | `grafo.svg` |

Regole generali:
- I nomi dei file Markdown iniziano sempre con un numero a due cifre seguito da punto e spazio (`NN. `).
- I diagrammi SVG vengono forniti in due varianti: chiara (`nome.svg`) e scura (`nome_scuro.svg`).
- Non includere spazi nei nomi di file che contengono asset; usare `_` o `-`.

---

## Formato dei file Markdown

Gli appunti usano **Markdown** con estensione MDX-compatibile. Alcune indicazioni:

- Usa intestazioni a partire da `##` (il titolo `#` è riservato al frontmatter o al titolo principale del file).
- Le formule matematiche usano la sintassi LaTeX inline (`$...$`) o a blocco (`$$...$$`).
- I blocchi di codice specificano sempre il linguaggio (`` ```c ``, `` ```python ``, ecc.).
- Evita HTML grezzo ove possibile; preferisci Markdown puro.

---

## Come aprire una pull request

1. Fai un **fork** della repository che vuoi modificare.
2. Crea un branch con un nome descrittivo (es. `fix/errore-teorema-cinese`, `add/esercizio-puntatori`).
3. Applica le modifiche rispettando la struttura e le convenzioni descritte sopra.
4. Apri la PR verso il branch `main` della repository originale, compilando il template fornito.
5. Attendi la revisione: il maintainer è l'unico che può approvare e unire le PR.

### Cosa scrivere nella PR

- **Titolo** chiaro e conciso (es. `Correggi dimostrazione teorema di Lagrange`).
- **Descrizione** con: cosa hai modificato, perché, e eventuali riferimenti (numero di lezione, pagina del libro, ecc.).
- Se non vuoi che nome utente e link al profilo vengano aggiunti al sito, indicalo esplicitamente nella descrizione.

---

## Canali alternativi

Se non vuoi aprire una PR ma vuoi comunque contribuire:

| Situazione | Cosa fare |
|---|---|
| Hai trovato un errore | Apri una issue → template **Errore nei contenuti** |
| Manca un argomento | Apri una issue → template **Richiesta argomento** |
| Hai una domanda | Usa le **Discussions** della repository o dell'organizzazione |
| Problema con il sito | Apri una issue in [`stangauni.github.io`](https://github.com/StangaUni/stangauni.github.io) → template **Problema con il sito** |

---

> Il materiale didattico originale (slide, registrazioni, testi di esame) rimane di proprietà dei rispettivi docenti e dell'Università di Padova: **non verrà mai incluso in queste repository**.
