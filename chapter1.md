# Questions and Answers

## 1.1 Question:
Suppose you have a sorted list of 128 names, and you’re searching through it using binary search. What’s the maximum number of steps it would take?

**Answer:**
The maximum number of steps required to search through a list of 128 names using binary search is log2(128) = 7

---

## 1.2 Question:
Suppose you double the size of the list. What’s the maximum number of steps now? Give the run time for each of these scenarios in terms of Big O.

**Answer:**
The maximum number of steps required to search through a list of double the last list is 256 names using binary search is log2(256) = 8

---

## 1.3 Question:
You have a name, and you want to find the person’s phone number in the phone book.

**Answer:**
the runtime in Big O notation depends on whether the phone book is sorted:
For a sorted phone book :O(log n)
For an unsorted phone book : O(n)

---

## 1.4 Question:

You have a phone number, and you want to find the person’s name in the phone book.. (Hint: You’ll have to search through the whole 
book!)

**Answer:**

 the runtime in Big O notation for searching a phone number in a 
phone book to find the person’s name is: O(n)

---

## 1.5 Question:

You want to read the numbers of every person in the phone book.

**Answer:**

as same as the 1.4 ,to read the numbers of every person in the phone book: O(n)

---

## 1.6 Question:

You want to read the numbers of just the As. (Ths is a tricky one!
It involves concepts that are covered more in chapter 4. Read the
answer—you may be surprised!)

**Answer:**

 We will divide it into two parts : 
Find the start of the "A" section: Using binary search, find the first entry that 
starts with "A."
Read through the "A" section: Once the start of the "A" section is found, iterate 
through the entries until you reach an entry that no longer starts with "A".
So the first part we can use o(log n ) and second part we can use o(m) "m is 
smaller than n" the answer will be o(log n + m)

---