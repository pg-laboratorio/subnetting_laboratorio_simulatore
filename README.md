# Subnetting Simulatore

Strumento interattivo per vedere gli indirizzi IPv4 bit per bit ed esercitarsi su **analisi IPv4** e **subnetting** con indirizzi sempre diversi. Gira interamente nel browser: non serve installare nulla.

👉 **[Apri Subnetting Simulatore](https://pg-laboratorio.github.io/subnetting_laboratorio_simulatore/)**

È il compagno pratico del repository **[subnetting_laboratorio_esercizi](https://github.com/pg-laboratorio/subnetting_laboratorio_esercizi)**: lì trovi regole, formule ed esercizi svolti, qui puoi allenarti e verificare le tue risposte.

## Cosa contiene

### Visualizzatore
Inserisci un indirizzo IP e una subnet mask (in decimale puntato, es. `255.255.255.224`, oppure come prefisso, es. `/27`) e osserva:
* i 32 bit di IP, maschera, indirizzo di rete, broadcast e wildcard, con i **bit di rete** e i **bit di host** in colori diversi;
* l'operazione di **AND bit a bit** che produce l'indirizzo di rete;
* il riepilogo della sottorete: host utilizzabili, primo e ultimo host, classe storica e ambito dell'indirizzo.

### Esercizio: Analisi IPv4
Viene generato un indirizzo casuale con il suo prefisso. Rispondi ai 5 punti del metodo:
1. Identificare lo Scopo (classe storica e ambito di rete)
2. Identificare la Subnet Mask (in decimale e in binario)
3. Numero di Host Disponibili
4. Indirizzo di Rete
5. Indirizzo Broadcast

### Esercizio: Subnetting
Vengono dati un indirizzo IP, la maschera originale e la maschera nuova. Rispondi agli stessi passi degli esercizi svolti:
* Passo preliminare: la rete madre
1. Numero di bit della sottorete (Subnet Bits)
2. Numero di sottoreti create (Subnets Created)
3. Numero di bit dell'host (Host Bits)
4. Numero di host per sottorete (Hosts per Subnet)
5. Indirizzo di rete dell'IP corrente (Network Address)
6. Primo host (First Host)
7. Indirizzo di broadcast (Broadcast Address)
8. Ultimo host (Last Host)
* Domanda in più: in quale sottorete cade l'IP

## Come si usa

* **Livello**: *Base* usa solo maschere `/8`, `/16`, `/24`; *Avanzato* usa qualsiasi maschera.
* **Verifica**: ogni risposta diventa verde (corretta) o rossa (da rivedere). La soluzione non viene mostrata, così puoi correggere e riprovare. Per gli errori più comuni compare un suggerimento.
* **Mostra soluzione**: la risoluzione passo passo con entrambi i metodi, **AND bit a bit** e **salto** (*magic number*).
* **Apri nel visualizzatore**: mostra in binario l'indirizzo dell'esercizio.
* **Usa un indirizzo tuo**: inserisci l'IP e le maschere di un esercizio del libro o della verifica e correggi le tue risposte allo stesso modo.

Puoi aprire direttamente una sezione aggiungendo all'indirizzo `#analisi` oppure `#subnetting`, ad esempio:
`https://pg-laboratorio.github.io/subnetting_laboratorio_simulatore/#subnetting`

## Consiglio
**Regola d'oro:** prova sempre a risolvere l'esercizio su carta prima di premere *Verifica*. Il simulatore serve a controllare il ragionamento, non a sostituirlo.

## Struttura del repository

| File | Contenuto |
| :--- | :--- |
| `index.html` | L'intero simulatore (HTML, CSS e JavaScript in un unico file) |
| `README.md` | Questo documento |
| `LICENSE` | Licenza d'uso |

Per usarlo senza connessione basta scaricare `index.html` e aprirlo con un browser.

## Licenza
Distribuito con licenza [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Vedi il file [LICENSE](./LICENSE).
