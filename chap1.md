## 1.1
The sum of any three single-digit numbers is less than $3*(b-1)$, while $b^{2}-3*(b-1)=b^2 - 3b + 3 > 0$, so it is is at
most two digits long.

## 1.2
Assume that $n$ is written as a binary integer of length $b$, then $2^{b-1} \leq n \leq 2^{b}-1$, 

we get $b = 1 + \lfloor log_{2}n \rfloor$, similarily, if $n$ is wirrten as a demical integer of length $d$, 

then $d = 1 + \lfloor log_{10}n \rfloor$. 

$4*d = 4 + 4 * \lfloor log_{10}n \rfloor$. 

## 1.3
  In order to minimize the depth, the number of nodes per layer must be as high as possible, 
  so $(d^{h-1}-1)/(d-1) < n \leq (d^{h} -1)/(d-1)$, then
     $h = \lfloor log_{d}((d-1)n + 1) \rfloor$


## 1.4
 - First, $n! = n*(n-1)*\cdots1 \leq n*n*\cdots n = n^{n}$, so $log(n!) = O(nlogn)$

 - Second, $n!^{2} = (n*1)*((n-1)*2)*\cdots (1*n) \geq (n/2)*(n/2)*\cdots(n/2) = (n/2)^{n}$

   &emsp;&emsp;&emsp; $log(n!) \geq (n/2)*log(n/2) = n/2*(logn) - n/2$,  

   &emsp;&emsp;&emsp;When $n \geq 4$ , $log(n)*n/4 \geq 2*n/4 = n/2$,

   &emsp;&emsp;&emsp;So $log(n!) \geq n/2*(logn) - n/2 \geq n/4*(logn)$
         
   &emsp;&emsp;&emsp;We get $log(n!) = \Omega(nlogn)$ 

## 1.5
<br/>


## 1.6
<br/>


## 1.7
   O(n*m)


## 1.8
We can prove $x*y = multiply(x, y)$ by induction on $n$, 
  
- Base case: when $y = 0$,  $x * 0 = multiply(x, 0)$, it's correct.

- Inductive Case:  
 &emsp;&emsp; if $y$ is odd, then
  $$
   \begin{aligned}
   x*y &= x*1 + x * (2* \lfloor y/2 \rfloor)   \\
       &= x*1 + 2 * (x * \lfloor y/2 \rfloor)  \\
       &= x*1 + 2* (mutiply(x, \lfloor y/2 \rfloor)) \: (by \: inductive \: hypothesis ) 
   \end{aligned}
 $$

  &emsp;&emsp; if $y$ is even, then
  $$
   \begin{aligned}
   x*y &= x * (2* \lfloor y/2 \rfloor)   \\
       &= 2 * (x * \lfloor y/2 \rfloor)  \\
       &= 2* (mutiply(x, \lfloor y/2 \rfloor)) \: (by \: inductive \: hypothesis ) 
   \end{aligned}
 $$


 
## 1.9



