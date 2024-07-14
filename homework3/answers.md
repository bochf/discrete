## Binomial Coefficients and Combinatorial Identities

### 1. Expand $(2c-3d)^5$ using the Binomial Theorem.

### SOLUTION

$$
\begin{aligned}
&(2c-3d)^5\\
=&\sum^5_{k=0}C(5,k)(2c)^{5-k}(-3d)^k\\
=&C(5,0)(2c)^5+C(5,1)(2c)^4(-3d)+C(5,2)(2c)^3(-3d)^2+C(5,3)(2c)^2(-3d)^3+C(5,4)2c(-3d)^4+C(5,5)(-3d)^5\\
=&32c^5-240c^4d+720c^3d^2-1080c^2d^3+810cd^4-243d^5
\end{aligned}
$$

---

### 2. Find the coefficient of the term $x^4y^7$ when expanding the expression $(x+y)^{11}$.

### SOLUTION
$C(11,7) = 330$

---

### 3. Use the Binomial Theorem to show that

$$0=\sum^n_{k=0}(-1)^kC(n,k)$$

### SOLUTION
$$
\begin{aligned}
&(a+b)^n = \sum^n_{k=0}C(n,k)a^{n-k}b^k\\
&Let\ a=1, b=-1,\ we\ have\ coefficients\\
&a_n=(-1)^k, 0 \le k \le n\\
\therefore\quad& \sum^n_{k=0}(-1)^kC(n,k)=(1-1)^n=0
\end{aligned}
$$

---

## The Pigeonhole Principle

### 4. An inventory consists of a list of 100 items, each marked "available" or "unavailable". There are 55 available items. Show that there are at least two available items in the list exactly nine items apart.

### SOLUTION
Let $a_i$ denote the position of the $i$th available item. We must show that $\exists\ i \ne j, a_i-9=a_j$. Consider the numbers

$$a_1, a_2, \cdots, a_{55}\tag{1}$$  
$$a_1+9, a_2+9, \cdots, a_{55}+9\tag{2}$$  
The 110 number in (1) and (2) have possible values from 1 to 109. By the second form of the Pigeonhole Principle, two of the numbers must coincide. We cannot have two of (1) or two of (2) identical; thus some number in (1) is equal to some number in (2). Therefore, $a_i-a_j=9$ for some $i$ and $j$, as desired.


---

### 5. Professor Euclid is paid every other week on Friday. Show that in some month, she is paid three times.

### SOLUTION
There are $365/7=52$ weeks a year, if she is paid every other week on Friday, there are at least $52/2=26$ payments a year. If every month has less than 3 payments, she can't be paid more than 24 times a year. So she is paid 3 times in some months.

---

## Recurrence Relations

### 6. Find a recurrence relation and initial conditions that begins with the given terms.
$$1,1,2,4,16,128,4096$$

### SOLUTION

$$
\begin{aligned}
&a_0=0\\
&a_1=0\\
&a_n=2a_{n-1}a_{n-2}
\end{aligned}
$$

---

### 7. Assume that a person invests $2000 at 14% interest compounded annually.
Let $A_n$ represent the amount at the end of $n$ years.

(a) Find a recurrence relation for the sequence $\lbrace A_n \rbrace ^{\infty}_{n=0}$

(b) Find an initial condition for the sequence $\lbrace A_n \rbrace ^{\infty}_{n=0}$

(c) Find $A_1, A_2,$ and $A_3$.

(d) Find an explicit formula for $A_n$

### SOLUTION
(a) $A_n = A_{n-1} + 0.14 \times A_{n-1}$

(b) $A_0 = 2000$

(c) 

$$
\begin{aligned}
&A_1 = 2280\\
&A_2 = 2599.20\\
&A_3 = 2963.088
\end{aligned}
$$

(d) $A_n = (1.14)^n(2000)$

---

### 8.
Let $S_n$ denote the number of n-bit strings that do not contain the pattern 00.

(a) Find a recurrence relation and initial conditions for the sequence $\lbrace S_n \rbrace$. Justify your answer.  
(b) Show that for all intergers $n \ge 1, S_n=f_{n+2}$, where $f$ denotes the Fibonacci sequence.

### SOLUTION
(a) The 1-bit strings that do not contain the pattern 00 are $\lbrace 0,1 \rbrace$, the 2-bit strings that do not contain the pattern 00 are $\lbrace 01, 10, 11 \rbrace$. For $n \ge 3$, the $n$-bit strings are formed by a $(n-1)$-bit string concatenate a "1" or "0".
- If the string ends in "1", the preceding n-1 bits must be an $n-1$-bit string that does not contain "00". The number of such string is $S_{n-1}$.
- If the string ends in "0", the preceding n-1 bits must be an string ends in "1". The number of such string is $S_{n-2}$.

From above analysis, we obtain the recurrence relation:

$$
\begin{aligned}
S_1 &= 2\\
S_2 &= 3\\
S_n &= S_{n-1} + S_{n-2}\qquad if\ n \ge 3
\end{aligned}
$$

(b)
The Fibonacci sequence is $f_n = f_{n-1} + f_{n-2},\ if\ n \ge 3,\qquad\ f_1 = 1,\ f_2 = 1$  
Let $F_n = f_{n+2},\ n \ge 1$, then

$$
\begin{aligned}
F_1 &= f_3 = 2\\
F_2 &= f_4 = 3\\
F_n &= f_{n+2} = f_{n+1} + f_{n} \qquad (if\ n \ge 3)\\
&= F_{n-1} + F_{n-2}
\end{aligned}
$$

It is the same as $S_n$ we get from (a)

---

## Solving Recurrence Relations

### 9. Solve the given recurrence relation for the initial conditions geven.

$$
\begin{aligned}
&a_0=1\\
&a_n=2^n a_{n-1} \ if\ n \ge 1
\end{aligned}
$$

### SOLUTION

$$
\begin{aligned}
&a_1=2^1a_0\\
&a_2=2^2a_1=2^2*2^1a_0=2^{2+1}a_0\\
&a_3=2^3a_2=2^3*2^{2+1}a_0=2^{3+2+1}a_0\\
&\cdots\\
&a_n=2^{n+(n-1)+(n-2)+\cdots+1}a_0=2^{\sum^{n}_1}a_0
\end{aligned}
$$  
Since $a_0=1$, we obtain the explicit fomula $a_n=2^{\sum^{n}_1}$

---

### 10. Solve the given recurrence relation for the initial conditions given.

$$
\begin{aligned}
&a_0=4\\
&a_1=10\\
&a_n=2a_{n-1}+8a_{n-2}\ if\ n \ge 1
\end{aligned}
$$

### SOLUTION
Solve the quadratic equation $t^2-2t-8=0$, we get  $t_1=-2, \ t_2=4$  
The sequence $a$ is of the form $a_n = b*(-2)^n+d*4^n$  
To meet the initial conditions, we must have

$$
\begin{aligned}
4&=b+d\\
10&=-2b+4d
\end{aligned}
$$

Solving for b and d, we find that b=1 and d=3. Thus

$$a_n=(-2)^n+3\cdot 4^n$$

---

### 11. Solve the given recurrence relation for the initial conditions given.

$$
\begin{aligned}
&a_0=1\\
&a_1=1\\
&a_n=6a_{n-1}-9a_{n-2}\ if\ n \ge 2
\end{aligned}
$$

### SOLUTION
Solve the quadratic equation $t^2-6t+9=0$, we get  $t=3$  
Since there is only one root, the sequence $a$ is of the form $a_n=bt^n+dnt^n$  
To meet the initial conditions, we must have

$$
\begin{aligned}
1&=b\\
1&=b \cdot 3+d \cdot 3
\end{aligned}
$$

Solving for b and d, we find that $b=1$ and $d=-\frac{2}{3}$. Thus

$$a_n=3^n-\frac{2n}{3} \cdot 3^n$$