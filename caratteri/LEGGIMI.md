# Caratteri del sito

Due caratteri, entrambi con **SIL Open Font License 1.1**: si possono ospitare,
modificare e ridistribuire, anche in un progetto commerciale. L'unico vincolo è
non venderli da soli e mantenere la licenza.

| File | Uso | Peso |
|---|---|---|
| `ZillaSlab-Bold.woff2` | Il nome "datigrezzi" | 700 |
| `IBMPlexMono-Bold.woff2` | Sottotitolo del marchio | 700 |
| `IBMPlexMono-Medium.woff2` | Testo di servizio | 500 |

Sono **ridotti al solo insieme di caratteri utilizzato** (lettere, cifre,
punteggiatura, vocali accentate italiane): da circa 270 KB ciascuno a 9-23 KB.

## Come usarli in una pagina

Metti i tre file in una cartella `caratteri/` accanto alla pagina e aggiungi
questo in cima al foglio di stile, al posto del collegamento a Google Fonts:

```css
@font-face{
  font-family:'Zilla Slab'; font-style:normal; font-weight:700; font-display:block;
  src:url('caratteri/ZillaSlab-Bold.woff2') format('woff2');
}
@font-face{
  font-family:'IBM Plex Mono'; font-style:normal; font-weight:700; font-display:block;
  src:url('caratteri/IBMPlexMono-Bold.woff2') format('woff2');
}
@font-face{
  font-family:'IBM Plex Mono'; font-style:normal; font-weight:500; font-display:block;
  src:url('caratteri/IBMPlexMono-Medium.woff2') format('woff2');
}
```

`font-display:block` fa attendere un istante prima di disegnare il testo, invece
di mostrarlo col carattere di ripiego e poi sostituirlo. Su file così piccoli
l'attesa è impercettibile ed elimina lo sfarfallio.

## Perché non usare più Google Fonts

1. **Resa identica ovunque.** Nessuna dipendenza dalla rete: il carattere o c'è
   o non c'è, e c'è sempre.
2. **Più veloce.** Tre file da pochi KB serviti dallo stesso dominio battono una
   connessione supplementare verso un dominio esterno.
3. **Nessun dato verso terzi.** Il collegamento a Google Fonts trasmette
   l'indirizzo IP di chi visita la pagina ai server di Google. Per un sito
   scolastico è una complicazione evitabile: ospitando i file, il problema non
   si pone.

## Se aggiungi testo con caratteri nuovi

I file contengono solo i segni presenti nell'insieme scelto. Se in futuro
servissero simboli non compresi (per esempio lettere greche o matematiche),
vanno rigenerati dai file completi, scaricabili da
`github.com/google/fonts/tree/main/ofl/zillaslab` e
`github.com/google/fonts/tree/main/ofl/ibmplexmono`.
