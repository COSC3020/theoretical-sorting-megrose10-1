# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

In order to verify said claim, we must first look at the best case runtime. According to the slides/video, the best run time
for a comparison algorithm would be $O(nlogn)$, so, this run time would be incorrect. Speaking on the physical analysis, if I had a list of let's say [1, 3, 2, 4],
the best runtime we could get from this list since X is a comparison based alogorithm is $O(nlogn)$. However if we have a list that is [1, 2, 3, 4] we can get 
a $O(n)$, but this is only for a fully sorted list, most likely the list will not be sorted. Since we do not know how X is implemented, we can already assume that even with entering a unsorted list like above, the best case is $O(nlogn)$. Another way to test is by timing how much a differently sized list would take. I could load in a list of 1...1000...10000 elements, and see if it increases in time or if it is more linear of time. Comparing how much time this algorithm would take with differently sized lists can show if this is linear time or not. This could test sorted, unsorted, partially sorted lists and would find the average in these cases to see the average best time. We would see a logarithmatic graph, that goes up to a point and then slowly continues to go up, rather than a linear line that goes up with the amount of elements. 

I used the class slides/video on reviewing the material. I asked Ali Torabi for what parts I was not describing correctly, and then worked on my own describing these 
parts correctly.

I submitted this work Fall 2024.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
