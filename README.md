The idea is to use Greedy Algorithm where at every step, such that the program settles all amounts of one person and recurs for the remaining n-1 persons.
Algorithm:
For every person Pi, from 0 to n – 1, do the following steps.
Compute the net amount for every person. The net amount for a person 'i' can be computed by subtracting the sum of all debts from the sum of all credits.
Find maximum creditor Pc and maximum debtor Pd. Suppose the maximum amount to be credited to a maximum creditor is maxCredit, and the maximum amount debited from a maximum debtor is called maxDebit.
Set x: = minimum of maxCredit and maxDebit. Then debit x from Pd, and credit x to Pc.
If x is the same as the maxCredit, then remove Pc from the set and recur for the next n-1 persons.
If x is the same as maxDebit, then remove Pd from a set of persons and recur for the next n-1 persons.
Complexity Analysis:
Time Complexity - O(N^2) where N is the number of persons
