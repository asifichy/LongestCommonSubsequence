# LongestCommonSubsequence

LCS problem is a dynamic programming approach in which we find the longest subsequence which is common in between two given strings. A subsequence is a sequence which appears in the same order but not necessarily contiguous. For example ACF, AFG, AFGHD, FGH are some subsequences of string ACFGHD. So for a string of length n there can be total 2^n subsequences. The LCS algorithm is widely used in bioinformatics.

For string ACFGHD and ABFHD, the longest common subsequence is AFHD. The function that is used to find the longest common subsequence of two strings is given below.



![Screenshot 2021-12-07 193340](https://user-images.githubusercontent.com/68398397/145038503-938ba6e7-216a-43b7-b47c-734ec23fb9cd.png)



Using Dynamic Programming to find the LCS
Let us take two sequences: 



![Screenshot 2021-12-07 193541](https://user-images.githubusercontent.com/68398397/145038818-aeb82799-ef91-4f26-b679-834eafed3d3c.png)



In order to find the longest common subsequence, start from the last element and follow the direction of the arrow. The elements corresponding to () symbol form the longest common subsequence.



![Screenshot 2021-12-07 193652](https://user-images.githubusercontent.com/68398397/145039015-6f5d37b3-dc8f-4367-a489-7efec7797b6d.png)



How is a dynamic programming algorithm more efficient than the recursive algorithm while solving an LCS problem?

The method of dynamic programming reduces the number of function calls. It stores the result of each function call so that it can be used in future calls without the need for redundant calls.

In the above dynamic algorithm, the results obtained from each comparison between elements of X and the elements of Y are stored in a table so that they can be used in future computations.

So, the time taken by a dynamic approach is the time taken to fill the table (ie. O(mn)). Whereas, the recursion algorithm has the complexity of 2max(m, n).



![Screenshot 2021-12-07 193754](https://user-images.githubusercontent.com/68398397/145039138-87dded3f-4693-4976-bc7e-3ba63427b517.png)



Output - 



![Screenshot 2021-12-07 193425](https://user-images.githubusercontent.com/68398397/145039179-ca89b1ee-9950-460e-813d-ef607c19f987.png)

