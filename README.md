# merge-sort

## **Questions**
[16,21,11,8,12,22] -> Merge Sort

1. Write the stages of the above array according to the sort type.
2. Write the Big-O notation.

## **Answers**
one.
    * ### Since there are 6 elements in the array, it will be divided by 3-3
        * **[16,21,11]** - **[8,12,22]**
    * ### Then indexes with 3 elements will also be split until only one element remains.
        * **[16]** - **[21,11]** --------------------- **[8]** - **[12 ,22]**
        * **[16]** - **[21]** - **[11]** ----------------- **[8]** - * *[12]** - **[22]**
    * ### Then the left and right elements will be combined in ascending order.
        * **[16,21]** - **[11]** --------------------- **[8,12]** - * *[22]**
    * ### Starting from the left, we compare the first element with the element next to it and reorder them starting from the smallest.
        * **[11,16,21]** ------------------------- **[8,12,22]**
    * ### In the last step, we sort them from smallest to largest, starting from the first elements in the left and right indexes.
        * **[8,11,12,16,21,22]**
___
2. Elements are ordered by n each time. 2^x=n logn=x as this rank is halved each time hence

     Its Time Complexity is shown as **O(nlogn)**.
