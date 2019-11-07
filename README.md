# SCC-Graph-Exercise
## Description
Mahir earns money doing freelance jobs and keeps his money in piggy banks(kumbara). After some time he realizes that he has a considerable amount of money and becomes paranoid that someone might steal his money. He starts putting his keys to the piggy banks inside the piggy banks. One day his roommate tells him about cryptocurrencies and he decides to invest in Bitcoin. To do that he needs to open all piggy banks. Initially, Mahir doesn’t have any key which is not inside a piggy bank. Exercise's issue is to decide which piggy banks should be cracked so that Mahir can open all piggy banks and the number of cracked piggy banks is minimized.
#### Important Notes:
- Piggy banks are numbered from 1 to N.
- A piggy bank may have any number of keys to open it including 0.
- A piggy bank may contain any number of key inside it including 0.
- Mahir doesn’t need all the keys of a type to open a piggy bank(i.e he can open Xth piggy bank if he holds a key to the Xth piggy bank).

## Input/Output Format 
### Input Format
The first line of the input file holds an integer, N, showing the number of piggy banks.
In the following N lines, information about a piggy bank is given, one per line. Information includes a number K which indicates the number of keys inside the piggy bank followed by key types separated by space.
### Output Format
In a single line print the number of piggy banks he should crack followed by which ones he should crack.
#### Important Note: 
If there are more than 1 way to open all piggy banks it can print any of them.
## Examples 
**Sample Input**

5 

2 1 2 

0

2 2 5

0

1 4


**Sample Output**

2 1 3

**Explanation**
- The first piggy bank has 2 keys inside it, key 1 and key 2. 
- The second piggy bank doesn’t have any keys in it.
- The third piggy bank has 2 keys inside it, key 2 and key 5. 
- The fourth piggy bank doesn’t have any keys in it.
- The fifth piggy bank has one key inside it, key 4.

Mahir can open all piggy banks by cracking the first and the third piggy banks. When he cracks the first piggy bank he will have key to the second piggy bank(key to the first piggy bank is useless because we already cracked it). When he crakcs the third piggy bank he will have keys to the second and the fifth piggy bank. He can open the fifth piggy bank with the key and get the key to the fourth piggy bank.

**Sample Input**

5 

1 2

1 3 

1 4 

1 5 

1 1

**Sample Output**

1 4

**Explanation**

Every piggy bank contain the key to the next piggy bank. Mahir can crack any of them to open all the piggy banks. As stated in the output format any answer which satisfies the minimum number to open all piggy banks is accepted.

## Implementation Details
1. Variable limits are as follows: 
  - 1 ≤ N ≤ 105
  - 1≤numberof keysintotal≤106
2. Execution time limit is 1 seconds.
3. Program will be compiled with cmake CMakeLists.txt && make command.
4. Execute the program with ./project3 inputFile outputFile command.
