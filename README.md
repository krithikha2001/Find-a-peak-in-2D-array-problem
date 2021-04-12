# Find-a-peak-in-2D-array-problem
# Assignment - 05





1.1 Find a computational problem that you can solve using the divide and conquer approach. 

# PROBLEM STATEMENT: TO FIND A PEAK IN THE 2D ARRAY

![image](https://user-images.githubusercontent.com/59526292/114338996-e0cbe280-9b71-11eb-871d-aad8cb3c959b.png)

A peak element is defined as -

An element is greater than or equal to its four neighbors, left, right, top and bottom. For example neighbors for A[i][j] are A[i-1][j], A[i+1][j], A[i][j-1] and A[i][j+1],then the element is called a peak element.

The side elements are considered accordingly for their neighbours.
 

 
# 2 Write pseudocodes to design algorithms for the above mentioned computational problem using the brute-force approach (incremental approach) and the divide and conquer approach.

Brute force:
![image](https://user-images.githubusercontent.com/59526292/114339026-ef19fe80-9b71-11eb-9f31-7be3048bc55e.png)
![image](https://user-images.githubusercontent.com/59526292/114339038-f4774900-9b71-11eb-8059-b88bb3f41c99.png)

# Divide and conquer:

EFFICIENT ALGORITHM APPROACH EXPLAINED-

●	Pick middle column j = m/2

●	Find global maximum on column j at (i, j)

●	Compare (i, j − 1),(i, j),(i, j + 1)

●	Pick left columns of (i, j − 1) > (i, j)

●	Similarly for right

●	(i, j) is a 2D-peak if neither condition holds

●	Solve the new problem with half the number of columns.

●	When you have a single column, find global maximum and you‘re done.
 
 ![image](https://user-images.githubusercontent.com/59526292/114339091-0e189080-9b72-11eb-9c69-7cdc69c45afc.png)

# 3 Analyze the time complexity of above algorithms. Analyze the divide and conquer algorithm using different methods such as (1) Recursion Tree Method (2) Iterative Method (3) Master Method (4) Substitution Method. Try to analyze the algorithm using as many methods as discussed above.

ITERATIVE
![image](https://user-images.githubusercontent.com/59526292/114339107-153f9e80-9b72-11eb-8a6d-def5af81463e.png)
 
SUBSTITUTION
![image](https://user-images.githubusercontent.com/59526292/114339146-28eb0500-9b72-11eb-8a79-c6a9cef6f52a.png)
 
RECURSION TREE
![image](https://user-images.githubusercontent.com/59526292/114339153-2dafb900-9b72-11eb-81a3-0988d9b02166.png)
 
MASTER METHOD
![image](https://user-images.githubusercontent.com/59526292/114339165-330d0380-9b72-11eb-8871-e2d9853f25b1.png)

# 6 Analyze the performance of both the implemented algorithms (performance of algorithms on your computers). Plot a graph.

DIVIDE AND CONQUER


![image](https://user-images.githubusercontent.com/59526292/114339252-5e8fee00-9b72-11eb-907e-03b8ba225ff2.png)

ITERATION METHOD

	![image](https://user-images.githubusercontent.com/59526292/114339287-6f406400-9b72-11eb-9a1f-fb1786ece566.png)

# 7 Comparatively analyze the performance of above algorithms and plot a graph.


For simplicity we have taken only square matrices where n depicts the number of rows and columns.

![image](https://user-images.githubusercontent.com/59526292/114339300-79626280-9b72-11eb-82f4-aba9dd41a9ae.png)

# TIME COMPLEXITY

USING DIVIDE AND CONQUER: O(n*log(m))

USING ITERATION METHOD: O(n*m)

n → number of rows

m → number of columns

# APPLICATIONS

●	One of the common challenges in signal processing is to detect important points in time or in space like peaks. These points represent local maxima (or minima)

![image](https://user-images.githubusercontent.com/59526292/114339423-c80ffc80-9b72-11eb-8bf5-b5cd2e2c5d14.png)

●	The noise is a general term of unwanted modifications of the signal. Let’s consider the example of our infrared camera. If we happen to point it to a white wall, our image would be homogeneous but due to the noise, there could be many pixel positions labeled as a peak if we take only the definition above.
![image](https://user-images.githubusercontent.com/59526292/114339437-d1996480-9b72-11eb-8f16-3e86e7adb10e.png)

●	In special cases, more sophisticated algorithms are known and used like the Genetic algorithm or the famous optimization method Gradient Descent. They are appreciated mainly in scientific applications for instance
