---
tags:
  - Fondamenti_di_Informatica
---

In C i <font color="#ffc000">File</font> sono gestiti tramite [[Puntatori]] e [[Funzioni per i File]] usando la libreria stdlio.h.

Li possiamo vedere come flussi di caratteri, parole o linee, e per interagirvi avremo bisogno di un [[Puntatori|puntatore]] a file, esso rappresenta la posizione all’ interno del <font color="#ffc000">File</font> in cui stanno avvenendo le modifiche, si <font color="#00b0f0">aggiorna automaticamente</font> quando andiamo a scrivere qualcosa o ad eliminarla.

Sono divisi in 2 tipi, <font color="#ffc000">Testo</font> e <font color="#ffc000">Binari</font>.

##### File di testo

Sono sequenze di <font color="#9bbb59">stringhe</font> organizzate in linee, che terminano con ‘\n’
Il file termina con un carattere speciale detto <font color="#f79646">EOF</font> (<font color="#4f81bd">End of File</font>).
Alcuni esempi di questi file sarebbero le estensioni:
- *.txt
- *.c
- *.cpp

##### File Binari

Sono sequenze di <font color="#9bbb59">bit</font>, sono memorizzati direttamente come sequenze di <font color="#e36c09">0</font>,<font color="#e36c09">1</font> alcuni esempi di estensioni di questi file sono:
- *.exe
- *.mp3
- *.jpg

