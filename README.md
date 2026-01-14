# 📓 Diario delle Attività C++

Benvenuto nel repository del mio **Diario delle Attività**! Questo progetto è un'applicazione da riga di comando sviluppata in C++ per aiutare gli utenti a organizzare la propria giornata in modo semplice ed efficiente.

---

## 🎯 A cosa serve il programma
Il programma permette di gestire un registro digitale dei propri impegni. Per ogni attività, è possibile salvare:
* **Descrizione**: Cosa bisogna fare.
* **Ora di inizio**: Quando inizia l'attività.
* **Ora di fine**: Quando termina.
* **Data**: Il giorno specifico dell'impegno.

> 💾 **Persistenza dei dati**: Tutte le attività vengono salvate automaticamente in un file chiamato `attivita.txt`. Questo significa che i tuoi dati non andranno persi quando chiudi il programma!

---

## 🏗️ Com'è fatto il programma (Logica Tecnica)

Il codice è organizzato in modo modulare per essere facile da leggere e mantenere:

### 1. Classe `Attivita`
Rappresenta il modello dei dati. Ogni volta che crei una nuova attività, il **costruttore** della classe si occupa di inizializzare:
* La descrizione del compito.
* Gli orari di inizio e fine.
* La validazione della data.

### 2. Classe `DiarioAttivita`
È il "cervello" del progetto. Gestisce una collezione di oggetti `Attivita` usando:
* `std::vector`: Per memorizzare la lista dinamica degli impegni.
* `std::map`: Per organizzare le attività in base alla data, rendendo la ricerca molto veloce.

---

## 🚀 Funzionalità principali
1. **➕ Aggiungi**: Inserimento di nuove attività con salvataggio su file.
2. **👁️ Visualizza Giorno**: Filtra e mostra solo gli impegni di una data specifica.
3. **📋 Visualizza Tutto**: Mostra l'elenco completo di tutte le attività salvate.
4. **🗑️ Elimina**: Rimuove un'attività specifica dal diario.
5. **🧹 Pulizia Schermo**: Interfaccia pulita grazie alla funzione cross-platform (`cls` su Windows, `clear` su Linux).

---

## 🛠️ Requisiti e Compilazione
Per eseguire questo programma, hai bisogno di un compilatore C++ (come GCC o Clang).

**Comando per la compilazione:**
```bash
g++ main.cpp DiarioAttivita.cpp -o DiarioAttivita
