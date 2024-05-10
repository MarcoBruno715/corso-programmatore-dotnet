## Lettura del codice

**Obiettivo:** 
Imparare a leggere il codice ed inserire commenti pertinenti

**Prerequisiti:**
Fondamenti della programmazione

Prima di iniziare a scrivere il codice bisogna saperlo leggere!
In questi esercizi si imparerà a leggere il codice e a descrivere cosa fa il codice scritto da altri.


**Leggere il seguente codice e descrivere cosa fa il metodo PrintEvenNumbers**

```c#
public void PrintEvenNumbers(int[] numbers)
{
    foreach (int number in numbers)
    {
        if (number % 2 == 0)
        {
            Console.WriteLine(number);
        }
    }
}
```

**Risposta**

il metodo prende in input un array di numeri interi e stampa a video solo i numeri pari contenuti nell'array.


**Leggere il seguente codice e descrivere cosa fa il metodo GetFactorial**

```c#
public int GetFactorial(int n)
{
    if (n == 0)
    {
        return 1;
    }
    else
    {
        return n * GetFactorial(n - 1);
    }
}
```

**Risposta**
il metodo calcola il fattoriale di un numero intero "n" passato come parametro,
utilizzando una chiamata ricorsiva alla stessa funzione fino a quando il valore di "n" non diventa 0.


 **Leggere il seguente codice e descrivere cosa fa il metodo ReverseString**

```c#
public string ReverseString(string str)
{
    char[] charArray = str.ToCharArray();
    Array.Reverse(charArray);
    return new string(charArray);
}
```

**Risposta**
il metodo prende in input una stringa e restituisce la stessa stringa ma con i caratteri in ordine inverso.


 **Leggere il seguente codice e descrivere cosa fa il metodo BubbleSort**

```c#
public int[] BubbleSort(int[] arr)
{
    for (int i = 0; i < arr.Length - 1; i++)
    {
        for (int j = 0; j < arr.Length - i - 1; j++)
        {
            if (arr[j] > arr[j + 1])
            {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    return arr;
}
```

**Risposta**

il metodo implementa l'algoritmo di ordinamento "Bubble Sort" per un array di numeri interi "arr".
L'algoritmo ordina l'array confrontando coppie di elementi adiacenti e scambiandoli se non sono in ordine crescente.

**Leggere il seguente codice e descrivere cosa fa il metodo IsPrime**

```c#
public bool IsPrime(int n)
{
    if (n <= 1)
    {
        return false;
    }

    for (int i = 2; i <= Math.Sqrt(n); i++)
    {
        if (n % i == 0)
        {
            return false;
        }
    }

    return true;
}
```

**Risposta**

il metodo verifica se un numero intero "n" passato come parametro è un numero primo,
utilizzando un ciclo "for" per controllare se "n" è divisibile per ogni numero compreso tra 2 e la radice quadrata di "n".


**Leggere il seguente codice e descrivere cosa fa il metodo SplitString**

```c#
public string[] SplitString(string str, char separator)
{
    string[] parts = str.Split(separator);
    return parts;
}
```

**Risposta**

il metodo prende in input una stringa "str" e un carattere separatore, e restituisce un array
di stringhe contenente le parti della stringa separate dal carattere separatore.


**Leggere il seguente codice e descrivere cosa fa il metodo MergeArrays**

```c#
public void MergeArrays(int[] arr1, int[] arr2)
{
    int[] mergedArr = new int[arr1.Length + arr2.Length];
    int i = 0;
    int j = 0;
    int k = 0;

    while (i < arr1.Length && j < arr2.Length)
    {
        if (arr1[i] < arr2[j])
        {
            mergedArr[k] = arr1[i];
            i++;
        }
        else
        {
            mergedArr[k] = arr2[j];
            j++;
        }
        k++;
    }

    while (i < arr1.Length)
    {
        mergedArr[k] = arr1[i];
        i++;
        k++;
    }

    while (j < arr2.Length)
    {
        mergedArr[k] = arr2[j];
        j++;
        k++;
    }

    Console.WriteLine("Array merged:");
    foreach (int num in mergedArr)
    {
        Console.Write(num + " ");
    }
}
```

**Risposta**

il metodo prende in input due array di numeri interi "arr1" e "arr2",
li unisce in un unico array ordinato "mergedArr" e stampa a video l'array risultante.
L'unione viene effettuata ordinando gli elementi degli array di partenza comparandoli tra loro per inserirli nell'array