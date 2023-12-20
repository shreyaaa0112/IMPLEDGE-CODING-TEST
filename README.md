We mainly use Tries to perform the task given to us
I have chosen to perform this in C language as my proficiency is in that particular language

The flow of the program is as follows-
1. We create a trie and start inserting the words into it 
2. We keep record of the length of the words being formed
3.  We sort the words nd hence we are able to get the longest and second longest words
4.  Now we check for the words using the concept of suffixes and prefixes if they are compound words or not
5. We then print the longest and second longest compound word
6. I have uploaded the code for reading the second imput file here. We can change the code as per our requirements and read any file of our choice by replacing the names

Brief Explanation-

-The code starts with declaring a struct Trie of 100 pointers
-It then creates a new TrieNode object and sets the isEndOfWord variable to 0. After that it iterates through 100 times, creating a NULL for each iteration.
-After that we can see an Insert Function for the Trie 
 Curr is used to mark the root of the trie and helps in traversal
 for loop is used to read each character of the word and insert into the trie
 isendOfword set to 1 to mark the completion of insertion of a word.

Functions created and their uses-
**search:** A search function is then put into the code to read if there is an existing word in the trie 
It also states that we can use this function for the lowercase letters.

**Bsort:** Then we use bubble sort to put all the words in lengthwise order in descending order so as to easily find the longest and second longest word 

**findPrefix**: usedto search for words that can be split into two parts (prefix and suffix) such that both parts are present in a given Trie. This will help us in choosing only the Compound words and no other simple words.

**getCompoundWords:** used to find the concatenated words from the file. 

We then open the file and process it accordingly 

