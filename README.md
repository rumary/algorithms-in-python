# algorithms-in-python
In this respository, I implemented some famous alogritms using python. I arrange them according to the strategy they use. And for every algorithn, I will explain the problem they try to solve and some relevant resourses.
## 1.0 Divide and Conquer
### Interger Multiplication Problem [Link](https://en.wikipedia.org/wiki/Karatsuba_algorithm)
![Interger_MUL][Interger_MUL1]

[Interger_MUL1]: ./images/integer_mult.png
The standard procedure for multiplication of two n-digit numbers requires a number of elementary operations proportional to ${\displaystyle O(n^{2})}$. As for The Karatsuba algorithm, it reduces the running time to at most ${\displaystyle n^{\log _{2}3}\approx n^{1.585}}$ <br>

<strong>Key idea</strong> <br>
The basic step of Karatsuba's algorithm is a formula that allows one to compute the product of two large numbers ${\displaystyle x}$ and ${\displaystyle y}$ using three multiplications of smaller numbers, each with about half as many digits as ${\displaystyle x}$ or ${\displaystyle y}$, plus some additions and digit shifts. <br>
<strong>Propeties</strong> <br>
* Running Time: $T(n)=\Theta (n^{\log _{2}3})\,\!$
### Merge Sort [Link](https://en.wikipedia.org/wiki/Merge_sort)
Before we talk about merge sort. First take a look at another algorithm and its running time to fully appreciate how great merge sort is.
One intuitive idea for sorting is to imitate how we arrange cards according to their size, like the picture below. We immediately arrange the card when we receive it just based on what we have on our hands.
![insert][insert1]

[insert1]: ./images/insert.png
And the running time for this alogorithm is $T(n)= O(n^{2})\,\!$. <br>
Gif below shows how merge sort works:
![merge][merge1]

[merge1]: ./images/Merge-sort-example-300px.gif

<strong>Key idea</strong> <br>
Divide the unsorted list into n sublists, each containing 1 element (a list of 1 element is considered sorted) and repeatedly merge sublists to produce new sorted sublists until there is only 1 sublist remaining. This will be the sorted list.<br>
<strong>Propeties</strong> <br>
* Running Time: $T(n)= O(n{\log n})\,\!$
