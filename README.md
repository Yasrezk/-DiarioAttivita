#📘Spiegazione semplice del programma Diario Attività

##🎯 A cosa serve il programma

Il programma permette di registrare attività con:

descrizione

ora di inizio

ora di fine

data

Tutte le attività vengono salvate in un file chiamato attivita.txt, così non si perdono quando chiudi il programma.

##🧱 Come è fatto il programma

1. Classe Attivita
2. 
2.Rappresenta una singola attività.
Quando crei un’attività nuova, il costruttore salva:

descrizione

ora di inizio

ora di fine

data

Questi valori vengono passati dall’utente.

2. Classe DiarioAttivita
Gestisce l’intero diario.

Fa tre cose principali:

All’avvio: carica le attività dal file

Durante l’uso: permette di aggiungere attività

Alla chiusura: salva tutto nel file

Il costruttore imposta il nome del file e chiama la funzione che legge i dati.
Il distruttore salva automaticamente le attività quando il programma termina.

##💾 Come funziona il salvataggio

Il programma usa un file di testo chiamato attivita.txt.
Questo file contiene tutte le attività registrate.
Ogni volta che chiudi il programma, il diario riscrive il file aggiornato.

##⚙️ Funzionamento in breve

Il programma si avvia e legge il file.

L’utente aggiunge una o più attività.

Le attività vengono memorizzate in un vettore.

Alla fine, il programma salva tutto nel file.
