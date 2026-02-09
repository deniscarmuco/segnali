---
title: "Guida completa alle caratteristiche dei post"
date: 2026-02-08
draft: true
weight: 10
tags: ["guide", "markdown", "formatting"]
summary: "Una guida completa che mostra tutte le possibilità di formattazione e strutturazione all'interno dei post. Titoli, liste, codice, blockquote e molto altro."
---

## Introduzione

Questo è un post di prova che dimostra tutte le possibili caratteristiche di formattazione e strutturazione disponibili nel sistema segnali_. Segui questa guida per comprendere come scrivere post ben strutturati e leggibili.

## Titoli e gerarchia

Puoi usare fino a 6 livelli di titoli:

### Titolo di livello 3
#### Titolo di livello 4
##### Titolo di livello 5
###### Titolo di livello 6

---

## Testo e formattazione

Il testo normale si scrive semplicemente. Puoi usare **testo in grassetto** per enfasi forte, *testo in corsivo* per enfasi leggera, e ***testo in grassetto e corsivo*** per enfasi massima.

Puoi usare anche ~~testo barrato~~ per indicare contenuto obsoleto.

Esiste anche il `codice inline` che puoi usare per riferimenti a funzioni, variabili, o comandi brevi.

---

## Liste

### Liste non ordinate

- Primo elemento
- Secondo elemento
  - Sub-elemento 1
  - Sub-elemento 2
- Terzo elemento

### Liste ordinate

1. Primo elemento
2. Secondo elemento
   1. Sub-elemento numerato
   2. Un altro sub-elemento
3. Terzo elemento

### Liste di definizione

Termine
: Definizione del termine

Concetto
: Spiegazione dettagliata del concetto in questione

---

## Blockquote e citazioni

> Questo è un blockquote. Perfetto per citazioni, messaggi importanti o estratti da altri testi.

> Un'altra citazione
> 
> Su più righe per maggiore leggibilità.

> Citazione nidificata
>> Con sotto-citazione
> 
> Ritorno alla citazione principale

---

## Codice

### Codice inline
Per inserire codice inline usa i backtick: `console.log('Hello')` o `npm install`.

### Blocchi di codice

```javascript
// JavaScript
function helloWorld() {
  console.log("Hello, World!");
  return true;
}
```

```python
# Python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)
```

```bash
# Bash/Shell
echo "Greeting from terminal"
ls -la
cd /path/to/directory
```

```html
<!-- HTML -->
<div class="container">
  <h1>Titolo principale</h1>
  <p>Paragrafo di testo.</p>
</div>
```

---

## Tabelle

| Feature | Descrizione | Disponibilità |
|---------|------------|---------------|
| Markdown | Formato testo semplice | ✓ Completa |
| Codice | Evidenziazione sintassi | ✓ Completa |
| Tabelle | Strutturazione dati | ✓ Completa |
| Immagini | Inserimento media | ✓ Sì |
| Link | Riferimenti interni/esterni | ✓ Completa |

---

## Link e riferimenti

[Link a Google](https://google.com)

[Link a pagina interna](/docs/infrastrutture/)

[Link con titolo](https://github.com "GitHub - Dove ospitare il codice")

Riferimento footnote[^1] che compila automaticamente.

[^1]: Questo è un footnote con spiegazione dettagliata

---

## Immagini

```markdown
![Testo alternativo](url-dell-immagine)
![Logo](/images/logo.png)
```

---

## Separatori orizzontali

Già usati sopra con `---`, ma puoi usare anche:

***

oppure

___

---

## Elementi speciali

### Enfasi

> **Lorem Ipsum** è il testo segnaposto per eccellenza.

### Elenchi di task

- [x] Task completato
- [ ] Task ancora da fare
- [ ] Altro da fare

---

## Sezione di Lorem Ipsum esteso

### Lorem Ipsum dolor sit amet

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### Variazione di Lorem

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.

Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.

---

## Front Matter (Metadati)

Ogni post ha un front matter YAML all'inizio che definisce:

```yaml
---
title: "Titolo del post"          # Titolo principale
date: 2026-02-08                  # Data di pubblicazione (YYYY-MM-DD)
draft: false                      # false=pubblicato, true=bozza
weight: 10                        # Ordine di visualizzazione (opzionale)
tags: ["tag1", "tag2"]           # Tag per categorizzazione
summary: "Breve descrizione..."   # Sommario da mostrare negli elenchi
---
```

---

## Note finali

Questo post dimostra:
- ✓ Titoli su più livelli
- ✓ Formattazione testo (grassetto, corsivo, barrato)
- ✓ Liste ordinate e non ordinate
- ✓ Blockquote
- ✓ Codice inline e blocchi
- ✓ Tabelle
- ✓ Link interni ed esterni
- ✓ Separatori
- ✓ Task list
- ✓ Footnote
- ✓ Front matter con metadati

Usa questi elementi per strutturare i tuoi post in modo chiaro e professionale!
