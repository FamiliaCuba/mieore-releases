# MieOre – release

Qui ci sono solo gli APK pubblicati e il file `annunci.json`. Il codice è privato.

## annunci.json

L'app legge questo file all'apertura e mostra gli avvisi attivi nella schermata Settimana.

| Campo | Significato |
|---|---|
| `id` | univoco. Da MieOre 1.0.6: se il tecnico lo chiude con la X sparisce solo per quel giorno e torna il giorno dopo (fino ad `al`). Versioni precedenti: chiuso = non torna più (per riproporlo usa un id nuovo) |
| `una_volta` | facoltativo, `true`: chiuso con la X non torna più (comportamento vecchio) |
| `titolo`, `testo` | testo semplice (niente HTML) |
| `bottone`, `url` | facoltativi. L'url deve essere `https://github.com/FamiliaCuba/...` o `https://fmcuba.com/...`: gli altri vengono ignorati |
| `dal`, `al` | facoltativi, formato `AAAA-MM-GG` |

Massimo 3 avvisi visibili insieme. **Gli avvisi sono solo per cose importanti** (novità, scadenze, problemi).

## app (Impostazioni → Altre app utili)

Le altre app di FMcuba NON si pubblicizzano negli avvisi: vanno nella lista `app`, che MieOre (dalla 1.0.11) mostra in
Impostazioni → Altre app utili con il pulsante "Scarica" (apre la pagina, MieOre non installa nulla).

| Campo | Significato |
|---|---|
| `nome`, `testo` | testo semplice |
| `url` | pagina di download: `https://github.com/FamiliaCuba/...` o `https://fmcuba.com/...` |

Se la lista manca o non si scarica, l'app usa quella interna (GPS Cam).
