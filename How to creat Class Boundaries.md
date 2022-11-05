```mermaid 

graph TD 

A[Select Two Consecutive Classes]-->|Class 1| B[3.0-3.9]
A[Select Two Consecutive Classes]-->|Class 2| C[4.0-4.9]
B[3.0-3.9]-->D[3.0]
B[3.0-3.9]-->E[3.9]
C[4.0-4.9]-->F[4.0]
C[4.0-4.9]-->G[4.9]
D[3.0]-->H(Lower Limit)
E[3.9]-->I(Upper Limit)
F[4.0]-->J(Lower Limit)
G[4.9]-->K(Upper Limit)


```

####  Now deduct Upper limit of class 1 from Lower limit of class 2
##### (4.0 - 3.9) = 0.1 
#### Now devide the answer i.e. 0.1 by 2 
##### 0.1/2 = 0.05
#### Deduct 0.05 from all the lower limits classes
#### Add 0.05 to all the upper limits of classes
