# Fondamenti della programmazione

Obiettivo: 
Familiarizzare con i concetti di base della programmazione

Imparare i concetti di base: prima di iniziare a scrivere codice, è importante acquisire una conoscenza di base dei concetti
fondamentali della programmazione, come le variabili, gli operatori, i cicli e le strutture dati

# Tipi di dati

Sono supportati una vasta gamma di tipi di dati, come stringhe, numeri interi, numeri a virgola mobile,
booleani e tipi di dati composti come array e strutture.

- Integer: rappresenta un numero intero positivo o negativo

- Float: rappresenta un numero decimale

- String: rappresenta una sequenza di caratteri

- Boolean: rappresenta un valore booleano, che può essere vero o falso

- Array: rappresenta una raccolta di valori dello stesso tipo

 **1. DICHIARARE UN ARRAY:**

   - Array numeri interi[10]
   - Array nomi stringhe[5]


 **2. INIZIALIZZARE UN ARRAY:**

   - numeri interi[0] = 1
   - numeri interi[1] = 2
   - numeri interi[2] = 3
   - nomi stringhe[0] = "Nome"
   - nomi stringhe[1] = "Luigi"
   - nomi stringhe[2] = "Bea"


 **3. ACCEDERE A UN ELEMENTO DI UN ARRAY:**

   - numeri interi[0]
   - nomi stringhe[1]

# Pila:

rappresenta una raccolta di valori dello stesso tipo

 **1. PUSH: INSERISCE UN ELEMENTO IN CIMA ALLA PILA.**

   - push(elemento)

In questo diagramma, la classe "Pila" rappresenta una pila e contiene un attributo "elementi"

La classe ha anche i metodi per eseguire le operazioni di inserimento, rimozione, accesso
all'elemento in cima alla pila, restituzione del numero di elementi presenti nella pila e verifica se la pila è vuota

# Variabili:

le variabili in C# vengono utilizzate per memorizzare i dati utilizzati dal programma.
Ogni variabile deve essere dichiarata con un tipo di dati specifico, come stringa,
intero o in virgola mobile, e deve essere assegnata un valore prima di essere utilizzata

 **1. DICHIARARE UNA VARIABILE:**

   - Integer x
   - String nome
   - Float y
   - Boolean z


 **2. INIZIALIZZARE UNA VARIABILE:**

   - x = 10
   - nome = "Mario"
   - y = 3.14
   - z = true


 **3. MODIFICARE IL VALORE DI UNA VARIABILE:**

   - x = x + 1
   - y = y * 2

# Operatori

C# supporta una vasta gamma di operatori, tra cui aritmetici (+, -, *, /),
di confronto (==, !=, <, >), di assegnazione (=), di logica (&&, ||, !) e di accesso ad un membro (.)

 **1. OPERATORI ARITMETICI:**

   - Somma (+): esegue la somma di due operandi.
   - Sottrazione (-): sottrae un operando da un altro.
   - Moltiplicazione (*): moltiplica due operandi.
   - Divisione (/): divide il primo operando per il secondo.

 **2. OPERATORI DI CONFRONTO:**

   - Uguale a (==): verifica se due operandi sono uguali.
   - Diverso da (!=): verifica se due operandi sono diversi.
   - Maggiore di (>): verifica se il primo operando è maggiore del secondo.
   - Minore di (<): verifica se il primo operando è minore del secondo.
   - Maggiore o uguale a (>=): verifica se il primo operando è maggiore o uguale al secondo.
   - Minore o uguale a (<=): verifica se il primo operando è minore o uguale al secondo.

 **3. OPERATORI LOGICI:**

   - And (&&): restituisce vero se entrambi gli operandi sono veri.
   - Or (||): restituisce vero se almeno uno degli operandi è vero.
   - Not (!): restituisce il contrario di un operando booleano

# Le condizioni:

 **1. IF-THEN:**

   - Se (condizione) allora (istruzioni)


 **2. IF-THEN-ELSE:**

   - Se (condizione) allora (istruzioni) altrimenti (istruzioni)


 **3. SWITCH-CASE:**

   - Scegli (espressione)
     caso (valore1): (istruzioni)
     caso (valore2): (istruzioni)
     caso (valore3): (istruzioni)
     ...
     caso (valoreN): (istruzioni)
     altrimenti: (istruzioni)

# Controlli di flusso

i controlli di flusso in C# permettono di controllare la logica del
programma e di eseguire determinate istruzioni solo in determinate condizioni.
I controlli di flusso comuni sono if-else, switch e cicli come for e while.

 **1. CICLO WHILE:**

   - Mentre (condizione) esegui (istruzioni)


 **2. CICLO DO-WHILE:**

   - Esegui (istruzioni) finché (condizione) è vera.


 **3. CICLO FOR:**

   - Per (variabile) da (valore iniziale) a (valore finale) esegui (istruzioni)


# Funzioni:

le funzioni in C# consentono di organizzare il codice in blocchi riutilizzabili e di creare un codice facile da leggere

 **1. DICHIARARE UNA FUNZIONE:**

   - funzione somma(x: Integer, y: Integer): Integer


 **2. DEFINIRE UNA FUNZIONE:**

   - funzione somma(x: Integer, y: Integer): Integer
     inizio
       risultato = x + y
       restituisci risultato
     fine


 **3. CHIAMARE UNA FUNZIONE**

   - z = somma(2, 3)

 **Espressioni**

le espressioni in C# sono utilizzate per valutare un valore,
come un'operazione matematica o una comparazione. Possono includere valori, variabili e operatori combinati insieme.

 **Istruzioni:**

le istruzioni in C# sono utilizzate per eseguire un'azione,
come assegnare un valore a una variabile o chiamare una funzione.
Le istruzioni più comuni sono assegnazioni, chiamate di funzione, controlli di flusso e cicli.

# Classi:

le classi in C# rappresentano gli oggetti che compongono un'applicazione.
Una classe può contenere dati e metodi, che rappresentano le azioni che l'oggetto può eseguire.

L'incapsulamento è rappresentato dal fatto che solo i metodi pubblici della classe possono essere utilizzati dagli oggetti esterni.
Gli attributi privati della classe possono essere accessibili solo attraverso i suoi metodi pubblici.

L'ereditarietà rappresenta il fatto che una classe può derivare da un'altra classe e utilizzare i suoi metodi e attributi.
Una classe derivata eredita tutti i metodi e gli attributi della classe base e può anche definire i suoi propri metodi e attributi.

Il polimorfismo rappresenta la capacità di una classe di utilizzare metodi di altre classi in modo diverso

In questo diagramma, una classe base ha diverse classi derivate che hanno i loro propri metodi e attributi.
 Un metodo polimorfico può essere utilizzato per eseguire operazioni su diverse classi derivate in modi diversi,
 in base alla sua implementazione specifica

 **1. DICHIARARE UNA CLASSE:**

   - classe Persona


 **2. DEFINIRE GLI ATTRIBUTI DI UNA CLASSE**

   - classe Persona
     - nome: String
     - età: Integer


 **3. DEFINIRE I METODI DI UNA CLASSE**

   - classe Persona
     - funzione saluta()
       inizio
         scrivi("Ciao, sono " + nome)
       fine


 **4. CREARE UN'ISTANZA DI UNA CLASSE**

   - persona1 = Persona()


 **5. ACCEDERE AGLI ATTRIBUTI DI UN'ISTANZA**

   - persona1.nome = "Mario"
   - persona1.età = 30


 **6. CHIAMARE I METODI DI UN'ISTANZA**

   - persona1.saluta()

In questo diagramma, la classe "Classe" rappresenta una classe generica e contiene un attributo "attributi" e un attributo "metodi"
che rappresentano gli attributi e i metodi della classe

# I metodi:
 
 I metodi rappresentano le azioni che l'oggetto può eseguire.


 **1. DICHIARARE UN METODO:**

   - funzione somma(x: Integer, y: Integer): Integer


 **2. DEFINIRE UN METODO:**

   - classe Calcolatrice
     - funzione somma(x: Integer, y: Integer): Integer
       inizio
         risultato = x + y
         restituisci risultato
       fine
     fine


 **3. CHIAMARE UN METODO:**

   - calcolatrice = Calcolatrice()
   - z = calcolatrice.somma(2, 3)

In questo diagramma, la classe "Classe" rappresenta una classe generica.
La classe "Calcolatrice" è una sottoclasse di "Classe" e rappresenta una classe specifica
che ha il metodo "somma". Le frecce che partono da "Calcolatrice" e puntano a "Classe" indicano che "Calcolatrice"
è una sottoclasse di "Classe" e ha accesso agli attributi e ai metodi ereditati dalla classe padre

# I costruttori:

I costruttori creano istanze delle classi e definiscono gli attributi

 **1. DEFINIRE UN COSTRUTTORE**

   - classe Persona
     - funzione costruttore(nome: String, età: Integer)
       inizio
         this.nome = nome
         this.età = età
       fine
     - <altre funzioni>

 **2. CREARE UN'ISTANZA DI UNA CLASSE UTILIZZANDO IL COSTRUTTORE**

   - persona1 = Persona("Mario", 30)

la classe "Classe" rappresenta una classe generica.
La classe "Persona" è una sottoclasse di "Classe" e rappresenta una classe specifica con gli
attributi "nome" e "età", il metodo "saluta" e un costruttore che accetta due parametri
("nome" e "età").
L'oggetto "persona1" è un'istanza della classe "Persona" che è stata creata utilizzando il costruttore e ha gli attributi
"nome" e "età" inizializzati in base ai valori passati al costruttore

# Gli oggetti:

In questo diagramma, la classe principale è "Tipi di oggetti", che ha cinque attributi rappresentati da una lista puntata.

 **1. CREARE UN'ISTANZA DI UNA CLASSE:**

   - persona1 = Persona()


 **2. INIZIALIZZARE GLI ATTRIBUTI DI UN'ISTANZA:**

   - persona1.nome = "Mario"
   - persona1.età = 30


 **3. CREARE UN'ALTRO OGGETTO A PARTIRE DALLA STESSA CLASSE:**

   - persona2 = Persona()


 **4. INIZIALIZZARE GLI ATTRIBUTI DELL'ALTRO OGGETTO**

   - persona2.nome = "Luigi"
   - persona2.età = 35

la classe "Classe" rappresenta una classe generica
La classe "Persona" è una sottoclasse di "Classe" e rappresenta una classe specifica con gli
attributi "nome" e "età" e il metodo "saluta".
Gli oggetti "persona1" e "persona2" sono istanze della classe "Persona" e hanno i loro attributi
specifici ("nome" e "età") inizializzati in modo diverso

# Namespace

i namespace in C# vengono utilizzati per organizzare le classi in modo gerarchico e per evitare conflitti di nomi.
Ciò consente di creare una struttura per il codice che lo rende più facile da navigare e mantenere

 **1. DICHIARARE UN NAMESPACE:**

   - namespace Nomi
   - namespace Numeri


 **2. DEFINIRE UN'ENTITÀ ALL'INTERNO DI UN NAMESPACE:**

   - namespace Nomi
     funzione stampaNome(nome: String)
       inizio
         scrivi(nome)
       fine
     fine


 **3. UTILIZZARE UN'ENTITÀ ALL'INTERNO DI UN NAMESPACE:**

   - Nomi.stampaNome("Mario")

# Le librerie di sistema

Sono parti di codice che aggiungono funzionalità


 **1. IMPORTARE UNA LIBRERIA DI SISTEMA**
 
   - import System


 **2. UTILIZZARE UNA FUNZIONE O UNA CLASSE DALLA LIBRERIA DI SISTEMA**

   - System.Console.WriteLine("Hello, World!")
   - x = System.Math.PI

In questo diagramma, la classe "Libreria di sistema" rappresenta una libreria di sistema
generica e contiene un attributo "funzioni" e un attributo "classi"
che rappresentano le funzioni e le classi fornite dalla libreria.
La classe "System" è una sottoclasse di "Libreria di sistema" e rappresenta una libreria di sistema specifica.
La classe ha diverse entità, come "Console", "Math", "File", ecc. che rappresentano le funzioni e le classi fornite dalla libreria.