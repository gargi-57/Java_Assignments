# Assignment_2

Part 1: W.a.p that declares two arrays named ‘even’ and ‘odd’. Accept numbers from the user and move them to respective arrays depending on whether they are even or odd. 
Part 2: Implement a java function that finds 2 neighboring numbers in an array with the smallest distance to each. The function should return the index of the 1st number.
Part 3: Write a Java program to convert an array into ArrayList and vice versa.
Algorithm: segregateEvenOdd()
1) Initialize two index variables left and right:  
            left = 0,  right = size -1 
2) Keep incrementing left index until we see an even number.
3) Keep decrementing right index until we see an odd number.
4) If left < right then swap arr[left] and arr[right]

 Making an array in a Java program involves three distinct steps:
Declare the array name.
Create the array.
Initialize the array values.
We refer to an array element by putting its index in square brackets after the array name: the code a[i] refers to element i of array a[]. For example, the following code makes an array of n numbers of type double, all initialized to 0:
double[] a;                    // declare the array
a = new double[n];             // create the array
for (int i = 0; i < n; i++)    // elements are indexed from 0 to n-1
   a[i] = 0.0;                 // initialize all elements to 0.0
Typical array-processing code.
ArrayExamples.java contains typical examples of using arrays in Java.

examples of array processing
Programming with arrays. Before considering more examples, we consider a number of important characteristics of programming with arrays.
Zero-based indexing. We always refer to the first element of an array a[] as a[0], the second as a[1], and so forth. It might seem more natural to you to refer to the first element as a[1], the second value as a[2], and so forth, but starting the indexing with 0 has some advantages and has emerged as the convention used in most modern programming languages.
Array length. Once we create an array, its length is fixed. You can refer to the length of an a[] in your program with the code a.length.
Default array initialization. For economy in code, we often take advantage of Java's default array initialization convention. For example, the following statement is equivalent to the four lines of code at the top of this page:
double[] a = new double[n]; 
The default initial value is 0 for all numeric primitive types and false for type boolean.
Memory representation. When you use new to create an array, Java reserves space in memory for it (and initializes the values). This process is called memory allocation.
Bounds checking. When programming with arrays, you must be careful. It is your responsibility to use legal indices when accessing an array element.
Setting array values at compile time. When we have a small number of literal values that we want to keep in array, we can initialize it by listing the values between curly braces, separated by a comma. For example, we might use the following code in a program that processes playing cards.
String[] SUITS = {
    "Clubs", "Diamonds", "Hearts", "Spades"
}; 

String[] RANKS = {
    "2", "3", "4", "5", "6", "7", "8", "9", "10",
    "Jack", "Queen", "King", "Ace"
};
After creating the two arrays, we might use them to print a random card name such as Queen of Clubs, as follows.
int i = (int) (Math.random() * RANKS.length); 
int j = (int) (Math.random() * SUITS.length); 
System.out.println(RANKS[i] + " of " + SUITS[j]); 



 
