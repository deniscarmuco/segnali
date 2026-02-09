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

## Front Matter - Opzioni Complete

Il front matter è la sezione YAML all'inizio di ogni post che definisce i metadati. Ecco tutte le opzioni disponibili:

### Struttura base

```yaml
---
title: "Titolo del post"
date: 2026-02-08
draft: false
---
```

### Opzioni complete del Front Matter

| Campo | Tipo | Obbligatorio | Descrizione |
|-------|------|--------------|-------------|
| `title` | string | ✓ Sì | Titolo principale del post |
| `date` | YYYY-MM-DD | ✓ Sì | Data di pubblicazione |
| `draft` | boolean | No | `true` = bozza (nascosto), `false` = pubblicato |
| `weight` | numero | No | Ordine di visualizzazione nella sezione (numeri più bassi = prima) |
| `tags` | array | No | Tag per categorizzazione: `["tag1", "tag2"]` |
| `summary` | string | No | Sommario di 1-2 righe mostrato negli elenchi |
| `description` | string | No | Descrizione alternativa (SEO) |
| `keywords` | array | No | Parole chiave per ricerca: `["chiave1", "chiave2"]` |
| `aliases` | array | No | URL alternativi per il post |
| `slug` | string | No | URL personalizzato del post |
| `layout` | string | No | Template layout personalizzato |
| `toc` | boolean | No | Mostra/nascondi table of contents |
| `math` | boolean | No | Abilita rendering KaTeX per formule matematiche |
| `diagram` | boolean | No | Abilita rendering Mermaid per diagrammi |

### Esempio completo con tutte le opzioni

```yaml
---
# Informazioni base (obbligatori)
title: "L'architettura tecnica del progetto"
date: 2026-02-09

# Visibilità e ordine
draft: false                    # Pubblica il post
weight: 1                       # Primo nella sezione

# Organizzazione e categorizzazione
tags: ["architettura", "backend", "infrastructure"]
summary: "Una analisi profonda dell'architettura tecnica, dalle fondamenta ai sistemi distribuiti."

# SEO e Discovery
description: "Scopri come è costruita l'infrastruttura tecnologica di questo progetto"
keywords: ["architettura", "backend", "infrastructure", "design", "sistema"]

# URL personalizzato
slug: architettura-tecnica

# Funzionalità speciali
toc: true                       # Mostra indice automatico dei titoli
math: true                      # Se il post contiene formule matematiche
diagram: true                   # Se il post contiene diagrammi Mermaid

# URL alternativi (redirect)
aliases:
  - /architettura/
  - /architettura-progetto/
---
```

### Note sui campi

**`title`**
- Obbligatorio
- Usato per il titolo h1 della pagina
- Mostrato negli elenchi e nelle card

**`date`**
- Obbligatorio, formato: YYYY-MM-DD
- Determina l'ordine nei listing
- Mostrata accanto al titolo

**`draft`**
- `true` = post non pubblicato (visibile solo con `hugo server --buildDrafts`)
- `false` = post pubblico (default)
- Utile per bozze in sviluppo

**`weight`**
- Numeri bassi vendono prima (weight: 1 prima di weight: 10)
- Default è ordine alfabetico se non specificato
- Usabile per pinning di post importanti

**`tags`**
- Array di stringhe: `["tag1", "tag2", "tag3"]`
- Crea pagine filtrate per tag
- Mostrate nella pagina del post

**`summary`**
- Testo di 1-2 righe (massimo 140 caratteri)
- Mostrato negli elenchi (home, archivio, categorie)
- Se non presente, Hugo estrae automaticamente dal contenuto

**`toc` (Table of Contents)**
- `true` = mostra indice automatico sulla destra
- `false` = nasconde indice
- Default dipende dalle impostazioni globali

**`math` e `diagram`**
- Abilita KaTeX per formule: `$$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$`
- Abilita Mermaid per diagrammi (flowchart, sequence, etc.)

### Esempio minimo (solo obbligatori)

```yaml
---
title: "Primo post"
date: 2026-02-09
---
```

### Esempio con tutte le feature

```yaml
---
title: "Guida al machine learning"
date: 2026-02-10
draft: false
weight: 5
tags: ["machine-learning", "ia", "python"]
summary: "Introduzione ai concetti base del machine learning con esempi pratici"
description: "Una guida completa ai principi fondamentali del machine learning"
keywords: ["ML", "AI", "deep-learning", "neural-networks"]
toc: true
math: true
slug: guida-machine-learning
aliases:
  - /ml-guide/
  - /machine-learning-101/
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
