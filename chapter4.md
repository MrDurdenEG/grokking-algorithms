# Questions and Answers

## 4.1 Question:

 Write out the code for the earlier sum function.

**Answer:**

#include <stdio.h>

int sum(int a, int b) {
    return a + b;
}

int main() {
    int result = sum(3, 5);
    printf("The sum is: %d\n", result);
    return 0;
}

---

## 4.2 Question:

 Write a recursive function to count the number of items in a list

**Answer:**

#include <stdio.h>


int count_items(int arr[], int size) {
    if (size == 0) {
        return 0;
    }
    else {
        return 1 + count_items(arr + 1, size - 1);
    }
}
int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int size = sizeof(arr) / sizeof(arr[0]);
    
    int count = count_items(arr, size);
    
    printf("Number of items in the list: %d\n", count);  // Output will be 5
    
    return 0;
}

---

## 4.3 Question:

 Find the maximum number in a list.

**Answer:**

#include <stdio.h>

int find_max(int arr[], int size) {
    int max = arr[0];
    for (int i = 1; i < size; ++i) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }
    return max;
}
int main() {
    int arr[] = {23, 45, 17, 52, 38};
    int size = sizeof(arr) / sizeof(arr[0]);
    int max_number = find_max(arr, size); 
    printf("The maximum number in the list is: %d\n", max_number);  // Output will be 52
    return 0;
}
---

## 4.4 Question:

Remember binary search from chapter 1? It’s a divide-and
conquer algorithm, too. Can you come up with the base case
and recursive case for binary search?

**Answer:**

The base case for binary search is an array with one
item. If the item you’re looking for matches the item in the
array, you found it! Otherwise, it isn’t in the array. In the
recursive case for binary search, you split the array in half,
throw away one half, and call binary search on the other half.

---
How long would each of these operations take in Big O notation?
---

## 4.5 Question:

Printing the value of each element in an array

**Answer:**

O (n)

---

## 4.6 Question:

 Doubling the value of each element in an array

**Answer:**

O (n)

---

## 4.7 Question:

Doubling the value of just the first element in an array

**Answer:**

O (1)

---

## 4.8 Question:

Creating a multiplication table with all the elements in the array. So 
if your array is [2, 3, 7, 8, 10], you first multiply every element by 2, 
then multiply every element by 3, then by 7, and so on.

**Answer:**

O (n2)

---
