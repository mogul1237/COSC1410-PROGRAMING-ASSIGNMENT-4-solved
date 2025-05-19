# COSC1410-PROGRAMING-ASSIGNMENT-4-solved

Download Here: [COSC1410 PROGRAMING ASSIGNMENT 4 solved](https://jarviscodinghub.com/assignment/programing-assignment-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

 In this assignment, you will develop and implement a program that sorts an array using the index sort algorithm. The primary objective of this assignment is for you gain experience in using arrays. 2 Program The program should generate an array of 10 raandom integers in the range [0 … 99] and sort the array in the ascending order. The array elements should be displayed on the terminal screen both before and after the sorting. The assignment description contains a brief information about the index sort algorithm; however, students are encouraged to do research on the topic and watch videos demonstrating the sorting algorithm. The interesting point of the indexSort() function is that it will NOT re-arrange the values of the array. Instead, a second array (an array of indexes corresponding to the values of the first array) will be sorted instead. A sorted array can then be produced with the sorted indexes. 3 Program Structure We use functions to break a problem into smaller sub-problems. This reduces program complexity. The main function will be the driver of the program. 3.1 The main Function Please notice that you should include the predefined libraries. You are not supposed to modify the main function. If you think you need to chance anything in the main function, please contact your lab TA. The definition of the main function should be as follows: int main() { // Declare variables int numbers[10], indexes[10]; // Randomly initialize the array numbers initializeArray(numbers); // Initialize the array indexes for(int i=0; i<10; i++) indexes[i] = i; // Display the arrays before the sorting cout << “numbers:” ; for(int i=0; i<10; i++) cout << numbers[i] << ” “; cout << “\nindexes:” ; for(int i=0; i<10; i++) cout << indexes[i] << ” “; // Sort the array indexSort(numbers, indexes); // Display the arrays after the sorting cout << “\n*****************************\n” ; cout << “numbers:” ; for(int i=0; i<10; i++) cout << numbers[i] << ” “; cout << “\nindexes:” ; for(int i=0; i<10; i++) cout << indexes[i] << ” “; return 0; }

In addition to the main function, the program must define the following two functions:  initializeArray  indexSort
3.2 The initializeArray Function The initializeArray function must have the following prototype:
void initializeArray(int numbers[]);
The parameter int numbers[]is an empty array of size 10, and it should be initialized by the function. More specifically, this function generates 10 random integers in the range of [0…99] and assign them to the array. 3.3 The indexSort Function The indexSort function must have the following prototype:
void indexSort (int numbers[], int indexes[]);
int numbers[] is the input array and int indexes[] is the array containing the index values that will be sorted. This function must implement the index sort algorithm. An example of the sort is given below:
Let’s assume that we are given an array of 10 elements,
We need a second array that contains elements representing the indexes of the array numbers.
We call the function indexSort
indexSort(numbers, indexes);
The arrays will have the following values after the function execution.
The array numbers: (stays the same)
In this example, 2 is the smallest value in the array numbers. It has an index value of 9. Therefore, 9 should be the first element of the array indexes. 3 is the second smallest value in the array numbers. Accordingly, its index, which is 3, is the second element in the array indexes.
The array indexes:

4 Grading
Your file name must be as follows: FirstNameLastNameUHID.cpp
A correct solution: worth 100 points
Deductions:
ERROR DEDUCTED POINTSP rogram cannot be compiled OR terminated unexpectedly during runtime 40 The function main is modified. 30 Proper indentation is not used 10 Function prototype is different, for each 10 Code is not commented 10 .cpp files do not follow Naming Conventions for submissions, listed in Assignment 10 initializeArray function does not generate values randomly 20 indexSort function sorts the actual input array but not the array indexes 30
1. Feel free to discuss ideas and implementations with your classmates, however DO NOT share code.
2. If you have a question about the assignment, do not wait until the last minute to ask.
3. Normal deductions for late submissions will be in effect. Please see Assignment Guidelines.
4. ANY kind of cheating, will result in a grade of 0.
