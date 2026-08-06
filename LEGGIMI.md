# Marchio datigrezzi

## Cosa c'è in questa cartella

**Il segno da solo**

| File | Uso |
|---|---|
| `marchio.svg` | Versione a colori, su fondo chiaro |
| `marchio-negativo.svg` | Su fondo scuro (l'ultima colonna diventa avorio) |
| `marchio-mono.svg` | Una sola tinta: fotocopie, circolari, timbri |
| `marchio-bianco.svg` | Tutto bianco, per fondi fotografici o pieni di colore |

**L'icona semplificata** — due colonne invece di quattro, perché sotto i 48 pixel le quattro si impastano.

| File | Uso |
|---|---|
| `favicon.svg` | Icona vettoriale del sito |
| `icona-fondo-scuro.svg` | Stessa icona con fondo inchiostro |
| `favicon-32.png`, `favicon-48.png` | Scheda del browser |
| `icona-180.png` | Schermata Home su iPhone e iPad |
| `icona-192.png`, `icona-512.png` | Manifest della PWA |
| `marchio-1024.png` | Anteprima ad alta risoluzione |

**Il marchio completo** — `marchio-completo.html`: segno più parola più sottotitolo, pronto da incollare.

## Colori

| Nome | Codice | Dove |
|---|---|---|
| Inchiostro | `#16303B` | Colonna allineata, testo del nome |
| Petrolio | `#17605C` | Colonna intermedia, puntino della i, sottotitolo |
| Rosso | `#B93A28` | Colonne sparse, la parola "grezzi" |
| Avorio | `#F4F0E6` | Fondo, e colonna finale sui fondi scuri |

## Regole d'uso

- **Lo spazio libero attorno al segno** è pari all'altezza di un elemento della griglia. Sotto quella misura il marchio soffoca.
- **Sotto i 48 pixel** si usa `favicon.svg`, mai il segno a quattro colonne.
- **Il nome resta sempre tutto minuscolo.** Le maiuscole riseparano visivamente le due parole, che sono state unite di proposito.
- **Il puntino verde sostituisce quello del carattere**, non ci si sovrappone.
- **Il sottotitolo è giustificato** sull'esatta larghezza della parola: la spaziatura fra le lettere si ricalcola, non si imposta a mano.

## Il carattere

Zilla Slab 700 per il nome, IBM Plex Mono 700 per il sottotitolo. Entrambi gratuiti su Google Fonts e con licenza libera, quindi utilizzabili anche nei documenti stampati.

## Se ti serve il marchio completo come immagine

Il file `marchio-completo.html` usa testo vivo, non tracciati: sul sito è la soluzione migliore, perché resta nitido a qualunque zoom e si modifica in un secondo. Ma un `.svg` con testo vivo si rompe sul computer di chi non ha i due caratteri installati.

Quindi, per una carta intestata o un PDF da mandare a terzi, servono i tracciati. Due strade:

1. **Aprire `marchio-completo.html` nel browser e stampare in PDF.** Il PDF incorpora i caratteri e non dipende più dalla loro presenza. È la via rapida.
2. **Installare Zilla Slab e IBM Plex Mono, ricomporre il blocco in Inkscape e convertire il testo in tracciati** (`Tracciato → Da oggetto a tracciato`). È la via giusta se il marchio deve finire in mano a un tipografo.

## Licenza

Il marchio segue la stessa licenza del progetto, GPL-3.0.
