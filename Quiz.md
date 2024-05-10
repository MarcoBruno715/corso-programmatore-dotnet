/***********************************************************************************************************************
 * Esercizi                                                                                                            *
 ***********************************************************************************************************************/

FACILI

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una variabile intera e stampa il valore della variabile nella console.             *
 ***********************************************************************************************************************/

    int num = 5; // dichiarazione di una variabile intera di nome num e inizializzazione a 5
    Console.WriteLine(num); // Console è una classe che rappresenta la console e WriteLine è un metodo che stampa una stringa nella console

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una variabile a virgola mobile e stampa il valore della variabile nella console.   *
 ***********************************************************************************************************************/

    double myDouble = 3.14; // dichiarazione di una variabile a virgola mobile di nome myDouble e inizializzazione a 3.14
    Console.WriteLine(myDouble);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una variabile booleana e stampa il valore della variabile nella console.           *
 ***********************************************************************************************************************/

    bool myBoolean = true; // dichiarazione di una variabile booleana di nome myBoolean e inizializzazione a true
    Console.WriteLine(myBoolean);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una variabile di tipo stringa e stampa il valore della variabile nella console.    *
 ***********************************************************************************************************************/

    string myString = "Hello, world!"; // dichiarazione di una variabile di tipo stringa di nome myString e inizializzazione a "Hello, world!"
    Console.WriteLine(myString);

/***********************************************************************************************************************
 * Scrivi un programma che chiede all'utente di inserire il proprio nome e l'età e poi stampa una frase che li contiene. *
 ***********************************************************************************************************************/

    Console.Write("Inserisci il tuo nome: ");
    // legge una stringa dalla console con Console.ReadLine
    string name = Console.ReadLine(); // ReadLine è un metodo che legge una stringa dalla console
    Console.Write("Inserisci la tua eta': ");
    // legge un intero dalla console con Console.ReadLine
    int age = int.Parse(Console.ReadLine()); // Parse è un metodo che converte una stringa in un intero
    Console.WriteLine("Ciao, " + name + "! Hai " + age + " anni."); // stampa una frase che contiene il nome e l'età

/***********************************************************************************************************************
 * Scrivi un programma che chiede all'utente di inserire la propria età, quindi stampa "Sei maggiorenne" se l'età      *
 * è maggiore o uguale a 18, altrimenti stampa "Sei minorenne".                                                        *
 ***********************************************************************************************************************/

    Console.Write("Inserisci la tua eta': ");
    int age = int.Parse(Console.ReadLine()); // legge l'età inserita dall'utente

    if (age >= 18) { // controlla se l'età è maggiore o uguale a 18
        Console.WriteLine("Sei maggiorenne.");
    } else {
        Console.WriteLine("Sei minorenne.");
    }


MEDI

/***********************************************************************************************************************
 * Scrivi un programma che chiede all'utente di inserire un numero intero, quindi stampa "Il numero è positivo" se il numero > di zero, *
 * "Il numero è negativo" se il numero è < zero e "Il numero è zero" se il numero è uguale a zero.                     *
 ***********************************************************************************************************************/

    Console.Write("Inserisci un numero: "); // chiede all'utente di inserire un numero
    int num = int.Parse(Console.ReadLine()); // legge il numero inserito dall'utente
    // controlla se il numero è positivo, negativo o zero
    if (num > 0) {
        // se il numero è positivo, stampa "Il numero è positivo"
        Console.WriteLine("Il numero e' positivo.");
    } else if (num < 0) {
        // se il numero è negativo, stampa "Il numero è negativo"
        Console.WriteLine("Il numero e' negativo.");
    } else {
        // se il numero è zero, stampa "Il numero è zero"
        Console.WriteLine("Il numero e' zero.");
    }

/***********************************************************************************************************************
 * Scrivi un programma che dichiara un array di stringhe contenente i nomi di tre persone e stampa il secondo nome dell'array . *
 ***********************************************************************************************************************/
    
    // dichiara un array di stringhe contenente i nomi di tre persone
    string[] names = { "Alice", "Bob", "Charlie" };
    // stampa il secondo nome dell'array
    Console.WriteLine(names[1]);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara due variabili intere, una contenente il valore 10 e l'altra contenente il valore 20, *
 * quindi le somma e stampa il risultato.                                                                              *
 ***********************************************************************************************************************/

    int num1 = 10; // dichiara una variabile intera contenente il valore 10
    int num2 = 20; // dichiara una variabile intera contenente il valore 20
    int sum = num1 + num2; // somma le due variabili
    Console.WriteLine(sum); // stampa il risultato

/***********************************************************************************************************************
 * Scrivi un programma che dichiara un array di stringhe contenente i nomi di tre città, e poi stampa tutti            *
 * i nomi delle città con la parola "città" aggiunta alla fine di ciascun nome.                                        *
 ***********************************************************************************************************************/

    // dichiara un array di stringhe contenente i nomi di tre città
    string[] cities = { "Roma", "Milano", "Firenze" };
    // stampa tutti i nomi delle città con la parola "città" aggiunta alla fine di ciascun nome
    foreach (string city in cities) { // per ogni città nell'array
        Console.WriteLine(city + " città"); // stampa il nome della città con la parola "città" aggiunta alla fine
    }

/***********************************************************************************************************************
 * Scrivi un programma che stampa i numeri da 1 a 10 utilizzando un ciclo while.                                       *
 ***********************************************************************************************************************/

    // dichiara una variabile intera contenente il valore 1
    int i = 1;
    // esegue il codice all'interno del ciclo finché la variabile i è minore o uguale a 10
    while (i <= 10) { // finché i è minore o uguale a 10
        Console.WriteLine(i);
        // incrementa la variabile i di 1
        i++;
    }

/***********************************************************************************************************************
 * Scrivi un programma che stampa i numeri da 1 a 10 utilizzando un ciclo for.                                          *
 ***********************************************************************************************************************/

    // esegue il codice all'interno del ciclo 10 volte
    for (int i = 1; i <= 10; i++) { // per ogni numero da 1 a 10 (inclusi) esegui
        Console.WriteLine(i);
    }

/***********************************************************************************************************************
 * Scrivi un programma che chiede all'utente di inserire due numeri interi, quindi stampa la loro somma utilizzando l'operatore +. *
 ***********************************************************************************************************************/

    Console.Write("Inserisci il primo numero: ");
    // legge il primo numero inserito dall'utente e lo converte in un numero intero
    int num1 = int.Parse(Console.ReadLine());
    Console.Write("Inserisci il secondo numero: ");
    // legge il secondo numero inserito dall'utente e lo converte in un numero intero
    int num2 = int.Parse(Console.ReadLine());

    // somma i due numeri
    int sum = num1 + num2;
    Console.WriteLine("La somma dei numeri e': " + sum);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara un array di interi vuoto, quindi stampa il numero di elementi dell'array nella console. *
 ***********************************************************************************************************************/

    // dichiara un array di interi vuoto
    int[] numbers = new int[0];
    // stampa il numero di elementi dell'array
    Console.WriteLine(numbers.Length);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una lista di interi contenente i numeri 1, 2 e 3,                                  *
 * quindi stampa il primo elemento della lista nella console.                                                          *
 ***********************************************************************************************************************/

    // dichiara una lista di interi contenente i numeri 1, 2 e 3
    List<int> numbers = new List<int> { 1, 2, 3 };
    // stampa il primo elemento della lista
    Console.WriteLine(numbers[0]);

In C#, gli array e le liste sono entrambi utilizzati per contenere una raccolta di elementi:

Dimensioni:
gli array hanno una dimensione fissa, mentre le liste possono espandersi o contrarsi dinamicamente.

Dichiarazione:
gli array vengono dichiarati utilizzando una sintassi fissa e con una dimensione specificata mentre le liste vengono dichiarate come oggetti utilizzando il costruttore List<T>.

Accesso agli elementi:
gli array consentono l'accesso diretto agli elementi utilizzando l'indice di posizione,
mentre le liste consentono l'accesso agli elementi utilizzando i metodi di accesso come ElementAt o Find.

Prestazioni:
gli array sono generalmente più efficienti delle liste in termini di prestazioni
perché hanno una dimensione fissa e sono memorizzati in modo continuo in memoria mentre le liste devono allocare memoria dinamicamente e dividere gli elementi in nodi.

Manipolazione degli elementi:
le liste forniscono molti metodi utili per manipolare gli elementi, come l'aggiunta, la rimozione e l'inserimento degli
elementi, mentre gli array richiedono che gli elementi siano copiati manualmente in una nuova posizione quando l'array viene modificato.

In generale, gli array sono più adatti per situazioni in cui la dimensione della raccolta di elementi è
nota in anticipo e non cambierà molto spesso, mentre le liste sono più adatte per situazioni in cui la dimensione della
raccolta potrebbe cambiare dinamicamente nel tempo.

Tuttavia, la scelta tra array e liste dipende dalle specifiche esigenze di un progetto e dalle considerazioni di prestazioni e gestione della memoria

DIFFICILI

/***********************************************************************************************************************
 * Scrivi un programma che dichiara un array di interi contenente i numeri 3, 5, 7, 9 e 11,                            *
 * quindi calcola e stampa la somma di tutti i numeri dell'array nella console.                                        *
 ***********************************************************************************************************************/

    // dichiara un array di interi contenente i numeri 3, 5, 7, 9 e 11
    int[] numbers = { 3, 5, 7, 9, 11 }; // oppure int[] numbers = new int[] { 3, 5, 7, 9, 11 };
    int sum = 0; // dichiara una variabile intera contenente il valore 0
    foreach (int number in numbers) { // per ogni numero nell'array
        sum += number; // aggiungi il numero alla variabile sum
    }
    Console.WriteLine("La somma dei numeri e': " + sum);

/***********************************************************************************************************************
 * Scrivi un programma che chiede all'utente di inserire un carattere e stampa "Il carattere è una vocale"             *
 * se il carattere è una vocale (a, e, i, o, u), altrimenti stampa "Il carattere non è una vocale".                    *
 ***********************************************************************************************************************/

    Console.Write("Inserisci un carattere: ");
    // legge il carattere inserito dall'utente e lo converte in un carattere
    // dichiara una variabile carattere contenente il carattere inserito dall'utente
    char ch = char.Parse(Console.ReadLine()); 
    // controlla se il carattere è una vocale
    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') { // condizione composta
        Console.WriteLine("Il carattere e' una vocale.");
    } else {
        Console.WriteLine("Il carattere non e' una vocale.");
    }

/***********************************************************************************************************************
 * Scrivi un programma che:                                                                                            *
 * dichiara un array di stringhe contenente i nomi di tre persone,                                                     *
 * quindi chiede all'utente di inserire il proprio nome e lo confronta con i nomi nell'array per vedere se c'è una corrispondenza. *
 * Se c'è una corrispondenza, il programma stampa un messaggio di saluto personalizzato per l'utente.                  *
 ***********************************************************************************************************************/

    // dichiara un array di stringhe contenente i nomi di tre persone
    string[] names = { "Alice", "Bob", "Charlie" };
    // chiede all'utente di inserire il proprio nome
    Console.Write("Inserisci il tuo nome: ");
    // dichiara una variabile stringa contenente il nome inserito dall'utente
    string user = Console.ReadLine();

    // confronta il nome inserito dall'utente con i nomi nell'array
    foreach (string name in names) { // per ogni nome nell'array
        if (name == user) { // se il nome corrisponde al nome inserito dall'utente
            // stampa un messaggio di saluto personalizzato per l'utente
            Console.WriteLine("Ciao, " + user + "!");
        }
    }

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una lista di interi vuota e aggiunge il numero 5 alla lista.                       *
 ***********************************************************************************************************************/

    // dichiara una lista di interi vuota
    List<int> numbers = new List<int>(); // metodi e oggetti sono inizializzati con il costruttore
    // oppure in maniera equivalente
    // List<int> numbers = new List<int> { };

    // aggiunge il numero 5 alla lista
    numbers.Add(5);

/***********************************************************************************************************************
 * Scrivi un programma che dichiara una lista di stringhe contenente i nomi di tre città italiane, quindi rimuove la seconda città dalla lista. *
***********************************************************************************************************************/

    // dichiara una lista di stringhe contenente i nomi di tre città italiane
    List<string> cities = new List<string> { "Roma", "Milano", "Napoli" };
    // rimuove la seconda città dalla lista
    cities.RemoveAt(1);