---
title: "01.01 L'architettura di Segnali"
date: 2026-02-01
draft: false
---

# L'architettura di Segnali

Per trasmettere riflessioni e deduzioni logiche, serve un'infrastruttura che sia allo stesso tempo invisibile e resiliente. Ho scelto di mappare questo spazio digitale seguendo i principi della stabilità e del minimalismo.

## Lo Stack Tecnico

La "stazione radio" è costruita su tre pilastri fondamentali:

* **Motore:** [Hugo](https://gohugo.io/), un generatore di siti statici che trasforma il testo semplice in pagine HTML in millisecondi. Zero database, zero latenza.
* **Ambiente di Sviluppo:** VS Code, con font **IBM Plex Mono**. La scrittura avviene nello stesso ambiente in cui si scrive codice, mantenendo il legame tra forma e funzione.
* **Diffusione:** [Cloudflare Pages](https://pages.cloudflare.com/). Il sito non risiede su un unico server, ma è distribuito sulla rete Edge globale. 

## La logica del deploy

Ogni volta che salvo un pensiero su VS Code e lo invio al repository (GitHub), scatta un trigger. Cloudflare intercetta il segnale, compila i sorgenti e aggiorna i nodi della rete. 

Non c'è spazio per il rumore. Solo il segnale pulito, dal mio terminale al vostro schermo.

---
*Stato: Online*;
*Latenza: Minima*

