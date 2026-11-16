# MieOre – release

Qui ci sono solo gli APK pubblicati e il file `annunci.json`. Il codice è privato.

## annunci.json

L'app legge questo file all'apertura e mostra gli avvisi attivi nella schermata Settimana.

| Campo | Significato |
|---|---|
| `id` | univoco; se il tecnico chiude l'avviso non lo rivede più. Per riproporlo usa un id nuovo |
| `titolo`, `testo` | testo semplice (niente HTML) |
| `bottone`, `url` | facoltativi. L'url deve essere `https://github.com/FamiliaCuba/...` o `https://fmcuba.com/...`: gli altri vengono ignorati |
| `dal`, `al` | facoltativi, formato `AAAA-MM-GG` |

Massimo 3 avvisi visibili insieme.
