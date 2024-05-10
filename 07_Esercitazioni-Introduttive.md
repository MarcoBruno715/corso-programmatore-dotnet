
**Esempio di utilizzo di try-parse per convertire una stringa**
```c#
Console.Write("Inserisci un numero intero: "); // chiede all'utente di inserire un numero intero
string input = Console.ReadLine(); // legge la stringa inserita dall'utente
int num; // dichiara una variabile di tipo intero
bool success = int.TryParse(input, out num); // converte la stringa in un numero intero e lo assegna alla variabile "num"
if (success) // se la conversione è andata a buon fine "true"
{
    Console.WriteLine("Il doppio del numero inserito è: " + (num * 2)); //  stampa il doppio del numero
}
else // altrimenti avrà il valore "false"
{
    Console.WriteLine("Input non valido!"); // stampa un messaggio di errore
}
```

**Esempio di utilizzo di variabili per il calcolo matematico**
```c#
Console.Write("Inserisci la lunghezza del lato del quadrato: ");
string input = Console.ReadLine();
int lato; // dichiara una variabile di tipo intero
bool success = int.TryParse(input, out lato); //input ed lato sono le variabili che verranno utilizzate per la conversione

if (success) // se la conversione è andata a buon fine, esegue il codice all'interno delle parentesi graffe
{
    int area = lato * lato; // calcola l'area del quadrato
    int perimetro = lato * 4;// calcola il perimetro del quadrato

    Console.WriteLine("L'area del quadrato è: " + area);
    Console.WriteLine("Il perimetro del quadrato è: " + perimetro);
}
else // se la conversione non è andata a buon fine, esegue il codice all'interno delle parentesi graffe
{
    Console.WriteLine("Input non valido!");
}
```
**Esempio di conversione di dati in questo caso da Celsius a Farenheit**
```c#
Console.Write("Inserisci la temperatura in gradi Celsius: ");
string input = Console.ReadLine();
double celsius; // dichiara una variabile di tipo double cioè con la virgola
// converte la stringa in un numero double e lo assegna alla variabile "celsius" e restituisce un valore booleano che indica se la conversione è andata a buon fine
bool success = double.TryParse(input, out celsius); 

if (success)
{
    // calcola la temperatura in gradi Fahrenheit
    double fahrenheit = (celsius * 9 / 5) + 32; // la formula per convertire da gradi Celsius a gradi Fahrenheit è: (gradi Celsius * 9 / 5) + 32
    Console.WriteLine("La temperatura in gradi Fahrenheit è: " + fahrenheit);
}
else
{
    Console.WriteLine("Input non valido!");
}
```
**Esempio di utilizzo di una fuziona ausiliaria**

la funzione ausiliaria "ReverseString" prende una stringa come parametro e restituisce la stringa invertita
 ```c#
static void Main(string[] args) // obsoleto da C# 7.0 in poi pero occhio che spesso si trova ancora
{
    Console.Write("Inserisci una stringa: ");
    string input = Console.ReadLine();

    // chiama la funzione ausiliaria "ReverseString" e passa la stringa inserita dall'utente come parametro
    string reversed = ReverseString(input);

    Console.WriteLine("La stringa invertita è: " + reversed);
}

static string ReverseString(string str) // string str è il parametro della funzione
{
    char[] charArray = str.ToCharArray(); // converte la stringa in un array di caratteri e lo assegna alla variabile "charArray"
    Array.Reverse(charArray); // inverte l'ordine degli elementi dell'array
    return new string(charArray); // converte l'array di caratteri in una stringa e la restituisce alla funzione chiamante (Main)
}
```
**Esempio di funzione ausialiaria che interagisce con un array calcolando la somma degli elementi**

la funzione ausiliaria "SommaArray" prende un array di numeri interi come parametro e restituisce la somma degli elementi dell'array
```c#
static void Main(string[] args)
{
    int[] numeri = { 5, 7, 10, 3, 4 }; // dichiara e inizializza un array di numeri interi

    Console.WriteLine("La somma degli elementi dell'array è: " + SommaArray(numeri));
}

static int SommaArray(int[] array) // int[] array è il parametro della funzione
{
    int somma = 0; // dichiara e inizializza una variabile di tipo intero a 0
    foreach (int numero in array) // scorre tutti gli elementi dell'array
    {
        somma += numero; // aggiunge il valore dell'elemento corrente all'accumulatore "somma"
    }
    return somma; // restituisce la somma degli elementi dell'array alla funzione chiamante (Main)
}
```
**Esempio di programma FizzBuzz**
```c#
static void Main(string[] args)
{
int numero; // dichiara una variabile di tipo intero

do // esegue il ciclo almeno una volta
{
    Console.Write("Inserisci un numero tra 1 e 100: "); // si ripete finché non si inserisce un numero compreso tra 1 e 100
    string input = Console.ReadLine();
    bool success = int.TryParse(input, out numero);

    if (!success || numero < 1 || numero > 100) // verifica che l'input sia un numero intero compreso tra 1 e 100
    {
        Console.WriteLine("Input non valido!");
    }
} while (numero < 1 || numero > 100); // ripete il ciclo finché l'input non è un numero intero compreso tra 1 e 100

if (numero % 3 == 0 && numero % 5 == 0) // verifica se il numero è divisibile sia per 3 che per 5
{
    Console.WriteLine("FizzBuzz"); // stampa "FizzBuzz" se il numero è divisibile sia per 3 che per 5
}
else if (numero % 3 == 0) // verifica se il numero è divisibile per 3
{
    Console.WriteLine("Fizz"); // stampa "Fizz" se il numero è divisibile per 3
}
else if (numero % 5 == 0) // 
{
    Console.WriteLine("Buzz"); 
}
else
{
    Console.WriteLine(numero);
}
}
```
**Esempio di programma che chiede all'utente di indovinare un numero dando dei suggerimenti**
```c#
Random random = new Random();   // crea un oggetto "Random" per generare numeri casuali
int numeroCasuale = random.Next(1, 101);    // genera un numero casuale compreso tra 1 e 100
int tentativi = 0;  // dichiara e inizializza una variabile di tipo intero a 0 per contare il numero di tentativi

Console.WriteLine("Indovina il numero segreto compreso tra 1 e 100!");

while (true)   // esegue il ciclo finché non si inserisce un numero compreso tra 1 e 100
{
    Console.Write("Tentativo #" + (tentativi + 1) + ": "); // stampa il numero del tentativo corrente
    string input = Console.ReadLine();
    int guess; // dichiara una variabile di tipo intero per memorizzare il numero inserito dall'utente
    bool success = int.TryParse(input, out guess);

    if (!success || guess < 1 || guess > 100) // verifica che l'input sia un numero intero compreso tra 1 e 100 i simboli  || significano "oppure"
    {
        Console.WriteLine("Input non valido! Inserisci un numero compreso tra 1 e 100.");
        // se l'input non è un numero intero compreso tra 1 e 100, stampa un messaggio di errore e ripete il ciclo
        continue;
    }

    tentativi++; // incrementa il numero di tentativi

    if (guess == numeroCasuale) // verifica se il numero inserito dall'utente è uguale al numero segreto
    {
        Console.WriteLine("Complimenti! Hai indovinato il numero segreto in " + tentativi + " tentativi.");
        break; // esce dal ciclo
    }
    else if (guess < numeroCasuale) // verifica se il numero inserito dall'utente è più piccolo del numero segreto
    {
        Console.WriteLine("Il numero segreto è più grande di " + guess + ".");
    }
    else
    {
        Console.WriteLine("Il numero segreto è più piccolo di " + guess + ".");
    }
}

```
**Esempio di semplice calcolatrice**
```c#
Console.WriteLine("Calcolatrice");

while (true)    // esegue il ciclo finché non si inseriscono due numeri e si sceglie un'operazione
{
    Console.Write("Inserisci il primo numero: ");
    string input1 = Console.ReadLine();
    double num1;    // dichiara una variabile di tipo double per memorizzare il primo numero inserito dall'utente
    bool success1 = double.TryParse(input1, out num1); // tenta di convertire la stringa in un numero decimale

    if (!success1)  // verifica che la conversione sia andata a buon fine
    {
        Console.WriteLine("Input non valido! Inserisci un numero.");
        continue;   // se la conversione non è andata a buon fine, ripete il ciclo
    }

    Console.Write("Inserisci il secondo numero: ");
    string input2 = Console.ReadLine();
    double num2;    // dichiara una variabile di tipo double per memorizzare il secondo numero inserito dall'utente
    bool success2 = double.TryParse(input2, out num2);

    if (!success2)
    {
        Console.WriteLine("Input non valido! Inserisci un numero.");
        continue;  // se la conversione non è andata a buon fine, ripete il ciclo
    }

    Console.WriteLine("Scegli un'operazione:");
    Console.WriteLine("1. Addizione");
    Console.WriteLine("2. Sottrazione");
    Console.WriteLine("3. Moltiplicazione");
    Console.WriteLine("4. Divisione");

    Console.Write("Operazione scelta: ");   // chiede all'utente di scegliere un'operazione 
    string scelta = Console.ReadLine();    // memorizza la scelta dell'utente in una variabile di tipo string

    double risultato;   // dichiara una variabile di tipo double per memorizzare il risultato dell'operazione

    switch (scelta) // esegue un'operazione diversa a seconda della scelta dell'utente
    {
        case "1":   // se l'utente ha scelto l'addizione
            risultato = num1 + num2;    // esegue l'addizione
            Console.WriteLine("Il risultato dell'addizione è: " + risultato);
            break;  // esce dal ciclo
        case "2":   // se l'utente ha scelto la sottrazione
            risultato = num1 - num2;    // esegue la sottrazione
            Console.WriteLine("Il risultato della sottrazione è: " + risultato);
            break;  // esce dal ciclo
        case "3":   // se l'utente ha scelto la moltiplicazione
            risultato = num1 * num2;    // esegue la moltiplicazione
            Console.WriteLine("Il risultato della moltiplicazione è: " + risultato);
            break;  // esce dal ciclo
        case "4":   // se l'utente ha scelto la divisione
            if (num2 == 0)  // verifica che il secondo numero non sia zero
            {
                Console.WriteLine("Impossibile dividere per zero!");
            }
            else
            {
                risultato = num1 / num2;    // esegue la divisione
                Console.WriteLine("Il risultato della divisione è: " + risultato);
            }
            break;  // esce dal ciclo
        default:    // se l'utente non ha inserito un'operazione valida (1, 2, 3 o 4)
        // default è una parola chiave che indica il codice da eseguire se nessuna delle altre condizioni è soddisfatta
            Console.WriteLine("Operazione non valida! Riprova.");
            break; // esce dal ciclo
    }
}
```
**Esempio di programma che manipola le parole**
```c#
static void Main(string[] args)
{
    Console.WriteLine("Giochi di parole");  // stampa un messaggio di benvenuto

    Console.Write("Inserisci una parola: ");    // chiede all'utente di inserire una parola
    string parola = Console.ReadLine(); // memorizza la parola inserita dall'utente in una variabile di tipo string

    Console.WriteLine("La parola invertita è: " + InvertiParola(parola));   // stampa la parola invertita
    Console.WriteLine("La parola in maiuscolo è: " + parola.ToUpper());   // stampa la parola in maiuscolo
    Console.WriteLine("La parola in minuscolo è: " + parola.ToLower());  // stampa la parola in minuscolo
    Console.WriteLine("La parola ha " + ContaVocali(parola) + " vocali.");  // stampa il numero di vocali

    if (Palindroma(parola)) // verifica se la parola è palindroma
    {
        Console.WriteLine("La parola è palindroma.");
    }
    else
    {
        Console.WriteLine("La parola non è palindroma.");
    }
}

static string InvertiParola(string parola)  // funzione ausiliaria per invertire la parola
{
    char[] chars = parola.ToCharArray();    // converte la stringa in un array di caratteri
    Array.Reverse(chars);   // inverte l'ordine degli elementi dell'array di caratteri tramite la funzione "Reverse"
    // Array è una classe che contiene metodi per gestire gli array
    // Reverse è un metodo della classe Array che inverte l'ordine degli elementi di un array
    // un metodo è una funzione che appartiene ad un oggetto
    return new string(chars);   // converte l'array di caratteri in una stringa
}

static int ContaVocali(string parola)
{
    int count = 0;  // dichiara una variabile di tipo int per memorizzare il numero di vocali
    foreach (char c in parola)  // scorre tutti i caratteri della parola e verifica se è una vocale
    // char c in parola è un'espressione che indica che c è un carattere della stringa parola
    {
        if ("AEIOUaeiou".IndexOf(c) >= 0)   // IndexOf(c) restituisce l'indice del carattere c all'interno della stringa "AEIOUaeiou"
        {
            count++;    // incrementa il contatore delle vocali
        }
    }
    return count;   // restituisce il numero di vocali
}

static bool Palindroma(string parola)
{
    string invertita = InvertiParola(parola);   // memorizza la parola invertita in una variabile di tipo string
    return parola.Equals(invertita, StringComparison.OrdinalIgnoreCase);    // verifica se la parola è uguale alla parola invertita (ignorando la differenza tra maiuscole e minuscole)
}
```