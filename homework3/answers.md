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
The 110 number in (1) and (2) have possible values from 1 to 109. By the second form of the Pigeonhole Priciple, two of the numbers must coincide. We cannot have two of (1) or two of (2) identical; thus some number in (1) is equal to some number in (2). Therefore, $a_i-a_j=9$ for some $i$ and $j$, as desired.


---

### 5. Professor Euclid is paid every other week on Friday. Show that in some nomth, she is paid three times.

### SOLUTION

---

## Recurrence Relations

### 6. Fina a recurrence relation and initial conditions that begins with the given terms.
$$1,1,2,4,16,128,4096$$

### SOLUTION

---

### 7. Assume that a person invests $2000 at 14% interest compounded annually.
Let $A_n$ represent the amount at the end of $n$ years.

(a) Find a recurrence relation for the sequence $\lbrace A_n \rbrace ^{\infty}_{n=0}$  
(b) Find an initial condition for the sequence $\lbrace A_n \rbrace ^{\infty}_{n=0}$  
(c) Find $A_1, A_2,$ and $A_3$.  
(d) Find an explicit formula for $A_n$

### SOLUTION

---

### 8.
Let $S_n$ denote the number of n-bit strings that do not contain the parttern 00.

(a) Find a recurrence relation and initial conditions for the sequence $\lbrace S_n \rbrace$. Justify your answer.  
(b) Show that for all intergers $n \ge 1, S_n=f_{n+2}$, where $f$ denotes the Fibonacci sequence.

### SOLUTION

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