# StangaUni

Raccolta open source di **appunti, riassunti, esercizi e materiale di supporto** redatti durante il percorso di laurea in **Informatica** presso l’[Università degli Studi di Padova](https://www.unipd.it).

Il materiale è scritto a scopo personale e didattico.  
**Non è garantita la completezza né l’assenza di errori**: usatelo come riferimento, non come sostituto allo studio dai libri di testo o alle lezioni.

> [!NOTE]
> Il maintainer segue prioritariamente i materiali ufficiali caricati dai docenti sulle piattaforme istituzionali.  
> Eventuali appunti basati solo sulla frequentazione delle lezioni (quando le slide non sono disponibili) sono segnalati esplicitamente nelle rispettive repository.

Le repository accettano contribuzioni esterne tramite **pull request**.  
Ogni PR viene revisionata e approvata esclusivamente dal maintainer (unico con accesso in scrittura).  
Consulta [CONTRIBUTING.md](../CONTRIBUTING.md) per le linee guida.

---

## Sito web

Tutti gli appunti sono consultabili in forma ottimizzata su:

**[stangauni.github.io](https://stangauni.github.io)**

Il sito offre:
- navigazione per materia
- supporto completo a formule matematiche (KaTeX / LaTeX)
- tema chiaro/scuro
- ricerca e struttura leggibile su desktop e mobile

Stack del sito: React · TypeScript · Vite · MDX · Tailwind CSS · KaTeX · Framer Motion · GitHub Pages.

---

## Repository

Le repository seguono la convenzione `AASS_materia`:
- `AA` = ultime due cifre dell’anno di inizio dell’a.a.
- `SS` = ultime due cifre dell’anno di fine
- `materia` = nome della materia in minuscolo con underscore

Esempio: `2526_algebra_e_matematica_discreta` = a.a. 2025/2026.

### Anno accademico 2025/2026 (I anno)

| Repository | Semestre | Materia |
|---|---|---|
| [2526_logica](https://github.com/StangaUni/2526_logica) | I | Logica |
| [2526_analisi_matematica](https://github.com/StangaUni/2526_analisi_matematica) | I | Analisi Matematica |
| [2526_architettura_degli_elaboratori](https://github.com/StangaUni/2526_architettura_degli_elaboratori) | I | Architettura degli Elaboratori |
| [2526_algebra_e_matematica_discreta](https://github.com/StangaUni/2526_algebra_e_matematica_discreta) | II | Algebra e Matematica Discreta |
| [2526_programmazione](https://github.com/StangaUni/2526_programmazione) | II | Programmazione |
| [2526_sistemi_operativi](https://github.com/StangaUni/2526_sistemi_operativi) | II | Sistemi Operativi |

### Anno accademico 2026/2027 (II anno)

| Repository | Semestre | Materia |
|---|---|---|
| [2627_programmazione_ad_oggetti](https://github.com/StangaUni/2627_programmazione_ad_oggetti) | I | Programmazione ad Oggetti |

> [!IMPORTANT]
> I riferimenti ai docenti (quando presenti sul sito) sono puramente indicativi: identificano i docenti responsabili dell’insegnamento su cui si basano i materiali.  
> **Non implicano alcuna attribuzione, approvazione o responsabilità** da parte dei docenti o dell’Università di Padova.  
> Tutto il contenuto è redatto interamente dagli studenti contributori.

---

## Struttura tipica di una repository

```
repository/
├── Riassunti/     # Riassunti sintetici delle lezioni
├── Utils/         # Schede, pattern, guide ai compitini, esempi di codice
├── Esercizi/      # Esercizi svolti (quando pubblicati)
└── assets/        # Diagrammi SVG (variante chiara + scura)
```

Le cartelle non ancora pronte per la pubblicazione sono escluse tramite `.gitignore` di ogni repository.

---

## Contribuire

1. Fai un **fork** della repository che vuoi modificare.
2. Crea un branch descrittivo (`fix/...`, `add/...`, `improve/...`).
3. Apri una **pull request** verso `main`.
4. Compila il template della PR.

A meno che non sia diversamente specificato nella PR, il tuo **nome utente GitHub** e un link al profilo verranno aggiunti sul sito (pagina informazioni + sezioni interessate).

Consulta [CONTRIBUTING.md](../CONTRIBUTING.md) per:
- convenzioni sui nomi dei file
- struttura delle cartelle
- formato Markdown/MDX
- cosa è accettato e cosa no

**Non vengono mai accettate** PR che includono materiale didattico originale (slide, registrazioni, testi d’esame).

---

## Licenza

Salvo diversa indicazione, tutto il materiale è distribuito sotto licenza  
**[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)**  
(Attribution-NonCommercial 4.0 International).

È consentito condividere e adattare per fini non commerciali, citando sempre la fonte.

Il materiale didattico originale (slide, testi di esame, dispense ufficiali, ecc.) rimane di proprietà dei rispettivi docenti e dell’Università di Padova e **non è incluso** in queste repository.
