---
layout: solution
title: Bubble Sort | Algorithm Solution
---

## Python Programming Language

~~~python
# Sorts data using bubble sort algorithm
def bubbleSort(items):
    while True:
        list_modified = False

        # FOR all items except the last
        #   swap adjacent items if out of order
        #   note if modification occur
        for i in range(len(items) - 1, 0, -1):
            if items[i] < items[i-1]:
                items[i], items[i-1] = items[i-1], items[i]
                list_modified = True

        # IF no modifications made to list THEN
        #   stop sorting
        if not list_modified:
            break

    return None

numbers = [10, 2, 3, 9, 4, 8, 6, 1, 7, 5]

print("Unsorted: \t %s" % numbers)
bubbleSort(numbers)
print("Sorted: \t %s" % numbers) 

~~~

~~~
$ python3 basic_bubble_sort.py
Unsorted: 	 [10, 2, 3, 9, 4, 8, 6, 1, 7, 5]
Sorted: 	 [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
~~~

## C Programming Language

~~~c
#include <stdio.h>  /* printf */

const int MAX_NUMBERS = 10000;

void bubbleSort(int[], int);
int swapAsc(int *, int *);
void printIntArray(int, int []);

int main(int argc, char* argv[]) {
	const int size = 10;	/* Number of items input by user */ 
	int numbers[size] = {2, 6, 3, 9, 8, 7, 1, 5, 4, 10};

    /* Output unsorted numbers */
	printf("Unsorted: \t");
	printIntArray(size, numbers);


    /* Sort numbers */
    bubbleSort(numbers, size);

    /* Output sorted numbers */
	printf("Sorted: \t");
	printIntArray(size, numbers); 

    return 0;
}

/* Bubble Sort
 * Sorts elements by comparing adjacent elements until 
 * they are sorted. */

void bubbleSort(int items[], int size) { 	
	int sorted;

    /* Sort items until sorted */
    do {
    	sorted = 1; /* Assume sorted */

        /* Swap items consecutively to end of array */
        for (int i = size - 1; i > 0; --i) {
            if ( swapAsc( &items[i], &items[i - 1] ) ) {
                sorted = 0; 
            }
        }  
    } while (!sorted);
}

/* Compares two elements, A and B,
 * and swaps them if they aren't ascending. */
int swapAsc(int *A, int *B) {
    if (*B > *A) {
        int temp = *A;
        *A = *B;
        *B = temp;

        return 1;
    }

    return 0;
}

void printIntArray(int size, int items[]) {	
	for (int i = 0; i < size; i++) {
		printf("%d ", items[i]);
	}
	printf("\n");
}
~~~

~~~
$ gcc -o basic_bubble_sort basic_bubble_sort.c 
$ ./basic_bubble_sort
Unsorted: 	2 6 3 9 8 7 1 5 4 10
Sorted: 	1 2 3 4 5 6 7 8 9 10
~~~

## Go Programming Language

~~~go
package main

import "fmt"

func bubbleSort(items []int) {
    for {
        list_modified := false

        for i := len(items) - 1; i > 0; i-- {
            if items[i] < items[i-1] {
                items[i], items[i-1] = items[i-1], items[i]
                 list_modified = true
            }
        }

        if !list_modified {
            break
        }
    }
}

func main() {
    items := []int{4, 4, 3, 4, 1}

    fmt.Println("Unsorted items: ", items)
    bubbleSort(items)
    fmt.Println("Sorted items: ", items)
}
~~~

~~~
$ go run basic_bubble_sort.go
Unsorted: 	 [10 9 8 7 6 5 4 3 2 1]
Sorted: 	 [1 2 3 4 5 6 7 8 9 10]
~~~

## Javascript (ES6) Programming Language

~~~js
function bubbleSort(items) {
    let swapped;

    do {
        swapped = false;
        for (var i = 0; i < items.length; i++) {
            if (items[i] > items[i+1]) {
                var temp = items[i];
                items[i] = items[i+1];
                items[i+1] = temp;
                swapped = true;
            }
        }
    } while (swapped);
  
  return items;
}

const unsorted_items = [4, 6, 2, 9, 8, 1, 7, 3, 10, 5];
let sorted_items = bubbleSort(unsorted_items.slice());

console.log("Unsorted:  " + unsorted_items);
console.log("Sorted:    " + sorted_items);
~~~

~~~
$ node basic_bubble_sort.js
Unsorted:  4,6,2,9,8,1,7,3,10,5
Sorted:    1,2,3,4,5,6,7,8,9,10
~~~