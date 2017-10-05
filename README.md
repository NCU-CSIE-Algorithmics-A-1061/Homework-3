# Homework 3

1. Problem 4-1: Recurrence examples<br>
Give asymptotic upper and lower bounds for T(n) in each of the following recurrences. Assume that T(n) is constant for n≤2. Make your bounds as tight as possible, and justify your answers.
    - ![T(n)=T(9n/10)+n](http://latex.codecogs.com/gif.latex?T%28n%29%3DT%28%5Cfrac%7B9n%7D%7B10%7D%29%2Bn)
    - ![T(n)=7T(n/3)+n^2](http://latex.codecogs.com/gif.latex?T%28n%29%3D7T%28%5Cfrac%7Bn%7D%7B3%7D%29%2Bn%5E2)
    - ![T(n)=7T(n/2)+n^2](http://latex.codecogs.com/gif.latex?T%28n%29%3D7T%28%5Cfrac%7Bn%7D%7B2%7D%29%2Bn%5E2)
    - ![T(n)=2T(n/4)+sqrt(n)](http://latex.codecogs.com/gif.latex?T%28n%29%3D2T%28%5Cfrac%7Bn%7D%7B4%7D%29%2B%5Csqrt%7Bn%7D)
    - 第十七組

2. Problem 4-3: More recurrence examples<br>
Give asymptotic upper and lower bounds for T(n) in each of the following recurrences. Assume that T(n) is constant for sufficiently small n. Make your bounds as tight as possible, and justify your answers.
    - ![T(n)=4T(n/3)+nlogn](http://latex.codecogs.com/gif.latex?T%28n%29%3D4T%28%5Cfrac%7Bn%7D%7B3%7D%29%2Bnlogn)
    - ![T(n)=3T(n/3)+n/logn](http://latex.codecogs.com/gif.latex?T%28n%29%3D3T%28%5Cfrac%7Bn%7D%7B3%7D%29%2B%5Cfrac%7Bn%7D%7Blogn%7D)
    - ![T(n)=4T(n/2)+n^2\*sqrt(n)](http://latex.codecogs.com/gif.latex?T%28n%29%3D4T%28%5Cfrac%7Bn%7D%7B2%7D%29%2Bn%5E2%5Csqrt%7Bn%7D)
    - ![T(n)=3T(n/3-2)+n/2](http://latex.codecogs.com/gif.latex?T%28n%29%3D3T%28%5Cfrac%7Bn%7D%7B3%7D-2%29%2B%5Cfrac%7Bn%7D%7B2%7D)
    - ![T(n)=T(n-1)+logn](http://latex.codecogs.com/gif.latex?T%28n%29%3DT%28n-1%29%2Blogn)
    - 第十組

3. Exercise 4.5-4:<br>
Can the master method be applied to the recurrence ![T(n)=4T(n/2)+n^2\*logn](http://latex.codecogs.com/gif.latex?T%28n%29%3D4T%28%5Cfrac%7Bn%7D%7B2%7D%29%2Bn%5E2logn)? Why or why not? Give an asymptotic upper bound for this recurrence.
    - 第六組

4. In chapter 4.1 (p.68), the author converts the stock buying problem into the maximum-subarray problem, then solves the problem with a divide-and-conque algorithm which takes Θ(nlogn) time. Design a O(n)-time algorithm that solves the stock buying problem without transformation.
    - 第二組

5. Analyze best-case, average-case, and worst-case performance of the following pseudocode which describes a sorting algorithm and determine whether it is in place and whether it is stable. Append your analyzing process or reasons.
    - 第十八組

```ruby
sort(first, last) # pass by address
    swap first and last if last.value < first.value
    size = last - first + 1
    if size >= 3
        offset = size / 3
        sort(first, last - offset)
        sort(first + offset, last)
        sort(first, last - offset)
```
