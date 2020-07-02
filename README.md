# progtechweb

------------------- Il player --------------

Gira su smartphone {e PC}. Viene usato dai ragazzi, che ricevono attraverso di esso
le istruzioni per i vari task e forniscono attraverso di esso le risposte cercate. Viene
attivata sullo smartphone tramite QRCode.

------------------ L'ambiente autore -------------------

Gira solo su PC. Viene usato dai curatori del museo (o dagli insegnanti) per creare
attività diverse, e raccogliere queste attività in tante storie diverse. Applicazione
web tradizionale da PC con parte client di raccolta foto, descrizioni, percorsi,
metadati, ecc. e parte server dove memorizzare i dati per i visitatori.

----------------- Le storie -------------------

Ogni gioco è una storia immersiva con un ambientazione
precisa e un obiettivo preciso, in cui hanno un ruolo chiave
alcuni oggetti reali (missioni diegetiche confidenziali).
• I giochi sono di tre tipi:
– individuale,
– piccolo gruppo (2-5 ragazzi) o
– classe (15-25 ragazzi organizzati in piccoli gruppi paralleli,
indipendenti ed in competizione)
• Gli studenti sono di tre fasce d'età:
– 7-10 anni: molte attività realizzative e iconiche, poche simboliche
– 11-14 anni: molte attività iconiche e simboliche, poche realizzative
– 15-18 anni: molte attività simboliche

Le storie sono organizzate in missioni composte da attività, di tipo
spiegazione o sfida.
– Le attività di tipo spiegazione sono testi, immagini, video, ecc. che l'utente
percepisce passivamente e che servono per dare contesto, background e
scopi.
– Le attività di tipo sfida (quest) sono richieste che spingono l'utente a fare
qualcosa, cercare qualcosa, usare qualcosa, o riflettere su qualcosa.
Ogni attività si conclude con un'azione dell'utente per proseguire a
quella successiva.
– La conclusione di una spiegazione è il click di un pulsante o una cosa del
genere per passare alla successiva
– la conclusione di una sfida è l'input di un dato che corrisponde alla soluzione
di un enigma o la dimostrazione del completamento
di un'azione: dati, testi, fotografie, ecc

Per passare alla attività successiva, l'input dell'utente va vagliato da
un'apposita procedura (che può e deve essere diversa caso per
caso), e dà parere positivo o negativo alla prosecuzione, o, con
storie parallele, indica in quale sottosequenza di attività si è andato
a cacciare l'utente.
Esistono tre tipi di risposte corrette:
– E' stata sottomessa una risposta purchessia (presenza/assenza)
– E' stata sottomessa una risposta accettabile (valore esatto, valore
presente in una lista di valori, valore in un range di valori, ecc.)
– E' stata sottomessa una risposta che ha generato una risposta positiva in
un servizio server-side black-box (solo 9CFU)
Ad ogni classe di risposta corrisponde la selezione di un'attività successiva, che
può essere obbligata oppure a scelta tra più attività o
missioni parallele. Accettabile anche la selezione random.

A seconda della natura della storia, la reazione ad una input
"sbagliato" può essere:
– niente (ad es., il codice della cassaforte è sbagliato),
– un errore (ad es. per il laboratorio delle analisi scientifiche il
campione spedito non è sangue ma pomodoro)
– una transizione verso una nuova attività più complessa e
pericolosa (ad es. la parola d'ordine era sbagliata e la sentinella
si è insospettita).
In nessun caso il messaggio risultante è fuori contesto (ad es. un
messaggio d'errore standard) ma rimane nella storia.
In nessun caso un input sbagliato fa precipitare la storia verso una
conclusione negativa. Questo non è un quiz, ma
un modo per apprendere dei concetti. 

Ci sono attività speciali all'inizio e alla fine, tutte spiegazioni:
– Attività iniziali: servono per fornire l'introduzione alla storia,
il background e il contesto e spiegano come giocare, chi è il
giocatore nella storia e come interagire con il device.
– Attività conclusive: servono per congratularsi con il
giocatore/la giocatrice per la conclusione del gioco e
dargli/le un premio: una promozione, un messaggio speciale,
la mano della principessa/del principe, ecc.
• In nessun caso c'è un messaggio di sconfitta. Il gioco non viene
MAI perso, ma solo rallentato o non concluso. 

{Ogni consegna deve fornire almeno tre giochi diversi, per tre
pubblici diversi (su nove combinazioni possibili). Almeno una per
ogni tipo di gioco e una per ogni fascia d'età.
Ogni gioco deve contenere almeno 10 attività diverse.
Ogni gioco deve avere un obiettivo didattico chiaro e preciso (ad
esempio, Napoleone Bonaparte, le equivalenze tra unità di misura,
la struttura della cellula, l'analisi logica, ecc.
La storia e le attività non debbono essere relative all'obiettivo
didattico relativo (ad esempio, il gioco su Napoleone può essere
basata su una storia contemporanea su un ladro
di cimeli napoleonici, ecc. }

Criteri di valutazione delle storie
{Le storie vengono valutate:
• per l'adeguatezza della storia al fine didattico
• per la sofisticazione narrativa
• per la sofisticazione delle attività richieste al giocatore
• per l'adeguatezza delle attività al pubblico a cui sono destinate}

-------------------- Il player ------------------------

• Il meccanismo principale attraverso cui il giocatore interagisce con le storie.
• Gira su smartphone {e, per esigenze di correzione, su PC}.
• La storia si attiva fotografando un QRcode specifico (ad esempio da un
cartellone appeso ecc.)
• Non c'è login: ad ogni attivazione di un gioco viene assegnato
automaticamente al device un nome in codice che verrà usato per tutto la
partita per identificare il device. L'associazione giocatore/nome in codice
non è compito del player.
• Ogni attività è composta da testi, immagini, video, oggetti interattivi, e un
meccanismo di gestione dell'input dell'utente.
– Le spiegazioni sono attività il cui unico input è "Prosegui" sempre vero.
– Le sfide richiedono input più complessi e gestione
della prosecuzione sulla base dell'input. 

• All'avvio, il player carica una risorsa (e.g., un file JSON) che
contiene i dati per gestire il gioco e le transizioni.
• L'interfaccia complessiva si adatta al singolo gioco sia per stile
(skin) che per struttura (layout).
• Il device stesso è contestualizzato nella storia: un taccuino nelle
mani di un investigatore, una radio ad onde corte nelle mani di
un agente del servizio segreto, un cellulare con whatsapp e
facebook nelle mani di un attivista politico che denuncia un
governo corrotto, ecc.
• Anche i widget di input sono contestualizzati nella
storia. Ad esempio, se debbo inserire il codice di
una cassaforte non vedrò il campo di input
numerico di default del browser, ma la manopola
di una cassaforte.
• Stili, widget e immagini vengono caricati
dinamicamente a partire dalla risorsa JSON. 

Criteri di valutazione del player
1. {Flessibilità e adattabilità a storie diverse
2. Sofisticazione grafica
3. Facilità d'uso
4. Robustezza e parametricità del codice}

------------- L'ambiente autore --------------

• Il meccanismo principale attraverso cui agisce il creatore di storie.
• Gira su browser tradizionale su PC.
• Contiene una sezione per gestire le storie (creazione, pubblicazione, ritiro,
ecc.) e una sezione per editare le attività di una o più storie.
• Attività di gestione:
– Creazione di una nuova storia
– Salvataggio temporaneo di una storia
– Duplicazione di una storia salvata
– Caricamento di una storia salvata
– Pubblicazione di una storia salvata
– Generazione del QRCode di una storia pubblicata
– Ritiro di una storia salvata
– Eliminazione/archiviazione di una storia salvata

• Attività di editazione:
– Creazione e modifica di attività
• Inserimento di testi, immagini, video, ecc.
• Specifica di widget di input per l'utente
• Specifica di risposte accettabili, non accettabili, sbagliate e
• Specifica di corrispondenti transizioni ad altre attività e
• Attribuzione di punteggi (anche negativi) a ciascuna risposta
– Organizzazione delle attività in missioni
• Missioni in sequenza o in parallelo
• Spostamenti di attività in ordine diverso o in missioni diverse
• Copia ed incolla di attività e missioni tra storie diverse.
• Attivazione/disattivazione di singole attività o missioni
• Visualizzazione del grafo delle transizioni da un'attività all'altra e da una missione
all'altra nella storia.
– Creazione e modifica del look & feel del player
• Opzione minima: caricamente foglio di stile CSS e librerie
javascript di widget precedentemente predisposti
• Opzione ottima: editor per stili e oggetti. 

Criteri di valutazione dell'ambiente autore
1. {Facilità d'uso complessiva
2. Flessibilità nella creazione di attività, missioni, storie
3. Presenza/assenza di editor di stili e componenti
4. Facilità d'uso dell'editor di stili e componenti
5. Robustezza e parametricità del codice}

----------------- Criteri di valutazione ----------------

Criteri di valutazione saranno:
1. la generalità dei tool:
– quanto le soluzioni per la compatibilità sono forzate e
quanto sono frutto di scelte ottimali per framework,
organizzazione del codice e uso corretto delle tecnologie
disponibili
2. la flessibilità:
– quanto le soluzioni tecniche adottate sono solide,
strutturate, facilmente comprensibili, facilmente
estendibili, facilmente adattabili a nuovi device / browser /
sistemi operativi / modelli di dati / modelli di annotazione
3. l'usabilità:
– Quanta attenzione è data alle esigenze di utenti (sia
lettori, sia annotatori) che non conoscono i dettagli né
del semantic web, né delle sintassi utilizzate, né del
modello concettuali prescelto
4. la sofisticazione grafica
– Quanta attenzione viene data alla presentazione delle
informazioni, al rapporto tra dimensioni delle maschere e
dimensioni dei dati da rappresentare, al rapporto tra
label comprensibili e dati formalizzati, alla corretta
differenziazione nei tipi di dati e di annotazioni.
