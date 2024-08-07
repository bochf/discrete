## Relations
### 1. 
Let $R_1$ and $R_2$ be relations on $\lbrace 1, 2, 3, 4 \rbrace$ given by

$$
\begin{aligned}
&R_1= \lbrace (1, 1), (1, 2), (3, 4), (4, 2) \rbrace\\
&R_2= \lbrace (1, 1), (2, 1), (3, 1), (4, 4), (2, 2) \rbrace\\
\end{aligned}
$$

List the elements of $R_2 \circ R_1$ and $R_1 \circ R_2$.

### SOLUTION
$$
R_1 \circ R_2 = \lbrace (1,1), (1,2),(3,4), (4,1), (4,2) \rbrace
$$

$$
R_2 \circ R_1 = \lbrace (1,1), (1,2), (2,1), (2,2), (3,1), (3,2), (4,2) \rbrace
$$

## Equivalence Relations
### 2. 
Determine whether the given relation is an equivalence relation on $X= \lbrace 1, 2, 3, 4, 5 \rbrace$. If the relation is an equivalence relation, list the equivalence classes.

$$R= \lbrace (x,y) \in X \times X | 3\ divides\ (x-y) \rbrace$$

### SOLUTION
$R$ is an equivalence relation  on $X$ because $R$ is reflexive, symmetric, and transitive.  
**Proof**  
- $\forall x \in X, x-x=0$, 3 divides 0, $\therefore (x, x) \in R, R$ is **reflexive**
- $\forall x,y \in X$, if 3 divides $(x-y)$, then 3 divides $(y-x)$, $\therefore (y,x) \in R, R$ is **symmetric**
- $\forall xRy$ and $yRz$, we have $x=y+3m, y=z+3n \Rightarrow x=z+3(m+n) | m,n \in Z$, $\therefore (x,z) \in R, R$ is **transitive**

Equivalence classes are: $\lbrace 1, 4 \rbrace, \lbrace 2,5 \rbrace, \lbrace 3 \rbrace$

---

### 3. 
List the ordered pairs of the equivalence relation R on the set $X= \lbrace 1,2,3,4 \rbrace$ defined by the parition $\mathcal{F}= \lbrace\lbrace 1,4 \rbrace,\lbrace 2,3 \rbrace\rbrace$. Also, find the equivalence classes [1], [2], [3], and [4].

### SOLUTION
The equivalence relation $R$ on set $X$ defined by $\mathcal{F}$ is

$$\lbrace(1,1), (1,4), (4,1), (4,4), (2,2), (2,3), (3,2), (3,3) \rbrace$$

The equivalence classes are

$$
\begin{aligned}
&[1]=[4]=\lbrace 1,4 \rbrace\\
&[2]=[3]=\lbrace 2,3 \rbrace
\end{aligned}
$$

---

### 4. 
Let $f$ be a function from $X$ to $Y$. Define a relation $R$ on $X$ by
$xRy$ if and only if $f(x)=f(y)$
Prove that $R$ is an equivalence relation on $X$.

### SOLUTION
$R=\lbrace (x,y) \in X \times X | f(x)=f(y) \rbrace$

**Proof**
- obviously, $f(x)=f(x)\ \forall x \in X$, so $xRx$, R is **reflexive**
- if $xRy$, then $f(x)=f(y) \Rightarrow f(y)=f(x)$, therefore $yRx$, R is **symmetric**
- $\forall xRy$ and $yRz$, we have $f(x)=f(y)=f(z)$, therefore $xRz$, R is **transive**

## Matrices of Relations
### 5. 
Suppose $X=\lbrace 1,2,3 \rbrace$ and $Y=\lbrace x,y \rbrace$, and $Z=\lbrace a,b,c \rbrace$ are ordered sets. If $R_1$ is the relation from $X$ to $Y$ given by

$$R_1=\lbrace(1,x), (1,y), (2,x), (3,x) \rbrace$$

and $R_2$ is the relation from $Y$ to $Z$ given by

$$R_2=\lbrace (x,b), (y,b), (y,a), (y,c) \rbrace$$

(a) Find the matrix $A_1$ of the relation R1 (relative to the given orderings).  
(b) Find the matrix $A_2$ of the relation R2 (relative to the given orderings).  
(c) Find the matrix product $A_1A_2$.  
(d) Use the result of part ($c$) to find the matrix of the relation $R_2 \circ R_1$.  
(e) Use the result of part ($d$) to find the relation $R_2 \circ R_1$ (as a set of ordered pairs).

### SOLUTION
(a)

$$
A_1=
\begin{array}{rcl}
&\begin{array}{c}
x&y
\end{array}\\ 
\begin{matrix}
1\\
2\\
3
\end{matrix}
&\begin{pmatrix}
1&1\\
1&0\\
1&0
\end{pmatrix}
\end{array}
$$

(b)

$$
A_2=
\begin{array}{rcl}
  &\begin{array}{c}
    b&a&c
  \end{array}\\
  \begin{matrix}
    x\\
    y
  \end{matrix}
  &\begin{pmatrix}
    1&0&0\\
    1&1&1
  \end{pmatrix}
\end{array}
$$

(c)

$$
A_1A_2=
\begin{array}{rcl}
\begin{matrix}
1\\
2\\
3
\end{matrix}
&\begin{pmatrix}
1&1\\
1&0\\
1&0
\end{pmatrix}
\end{array}
\times
\begin{array}{rcl}
  &\begin{array}{c}
    b&a&c
  \end{array}\\
  &\begin{pmatrix}
    1&0&0\\
    1&1&1
  \end{pmatrix}
\end{array}=
\begin{array}{rcl}
  &\begin{array}{c}
    b&a&c
  \end{array}\\
  \begin{matrix}
    1\\
    2\\
    3
  \end{matrix}
  &\begin{pmatrix}
    2&1&1\\
    1&0&0\\
    1&0&0
  \end{pmatrix}
\end{array}
$$

(d)
Replace all non-zero elements in (c) to 1, we get the matrix

$$
R_2 \circ R_1=
\begin{array}{rcl}
  &\begin{array}{c}
    b&a&c
  \end{array}\\
  \begin{matrix}
    1\\
    2\\
    3
  \end{matrix}
  &\begin{pmatrix}
    1&1&1\\
    1&0&0\\
    1&0&0
  \end{pmatrix}
\end{array}
$$

(e)
Based on the matrix of (d), $R_2 \circ R_1 = \lbrace (1,b), (1,a), (1,c), (2,b), (2,c) \rbrace$

---

### 6.
Suppose the matrix $A$ of a relation $R$ on an ordered set $X=\lbrace w,x,y,z \rbrace$ is given by

$$
A=
\left(\begin{array}{cccc}
1&0&1&0\\
0&0&0&0\\
1&0&1&0\\
0&0&0&1\\
\end{array}
\right)
$$

(a) Use $A$ to determine if $R$ is reflexive.  
(b) Use $A$ to determine if $R$ is symmetric.  
(c) Use $A$ to determine if $R$ is anti-symmetric.  
(d) Use $A$ to determine if $R$ is transitive.  
(e) Find $R$ as a set of ordered pairs.  
(f) Find $R$ as a digraph.

### SOLUTION
(a) $R$ is not relfexive because $A_{1,1} = 0$

(b) $R$ is symmetric because $A_{ij} = A_{ji}$

(c) $R$ is not anti-symmetric because $A_{1,3} = A_{3,1}$

(d)

$$
A^2=
\begin{pmatrix}
  2&0&2&0\\
  0&0&0&0\\
  2&0&2&0\\
  0&0&0&1
\end{pmatrix}
$$

Whatever entry $i,j$ in $A^2$ is nonzero, entry $i,j$ in A is also nonzero, and vice versa. $R$ is transive. 

(e) $R=\lbrace (w,w), (w,y), (y,w), (y,y), (z,z)\rbrace$

(f)
```mermaid
stateDiagram
 w
 x
 y
 z
w-->w
w-->y
y-->y
y-->w
z-->z
```

## Basic Principles
### 7.
How many different car license plates can be constructed if the licenses contain three letters followed by two digits  
(a) if repetitions are allowed.  
(b) if repetitions are not allowed.

### SOLUTION
Assume there are total 26 **letters** in English alphabet, case insensitive.
Assume there are 10 digits (0-9).

(a) If repetitions are allowed, total number of different license plates is $26^3 \times 10^2=1,757,600$

(b) If repetitions are not allowe, total number of different license plates is $P(26,3) \times P(10,2)=1,404,000$

---

### 8. 
How many strings of length 5 formed using the letters ABCDEFG without repetitions  
(a) begin with AC or DB in that order?  
(b) contain letters B and D consecutively in either order (i.e., BD or DB)?

### SOLUTION
(a) A 5 character long string begins with AC or DB using letters ABCDEFG without repetitions is $\lbrace(A,C,x,y,z) | x,y,z\in \lbrace B,D,E,F,G \rbrace\rbrace + \lbrace(D,B,x,y,z) | x,y,z\in \lbrace A,C,E,F,G \rbrace\rbrace$  
Starts with AC: $P(5,3)=5*4*3=60$  
Starts with DB: $P(5,3)=5*4*3=60$
Total is 60+60=120

(b) Replace BD by X, the string of 5 letters using ABCDEFG is equivalent to a string of 4 letters using ACEFGX. The number of permutations of such string is $P(6,4)=6*5*4*3=360$. The same as contains DB.
Total number of strings contains consecutive letter B and D is $360+360=720$

---

### 9.
A **bit** is a binary digit (a digit that is 0 or 1). How many eigth-bit strings either start with a 1 or end with a 1 or both?

### SOLUTION
start with 1: $2^7=128$  
end with 1: $2^7=128$  
both start and end with 1: $2^6=64$

## Permutations and Combinations
### 10.
In how many ways can five distinct Martians and eight distinct Jovans wait in line if no two Martians stand together.

### SOLUTION
1. **Place the Jovans in line first** Since there are 8 Jovans, there will be 9 posible slots for Martians, like below:
   
   $$ mJmJmJmJmJmJmJmJm $$

Where $J$ represents one Jovan, $m$ represents a slot can place one Martian.  
There are $P_j=9!=40320$ ways to arrange the Jovans

2. **Place the 5 Martians in 5 slots** There are $P_m=P(9,5)=15120$ ways to place the Martians.
3. Total ways $T=P_j \times P_m = 40320 \times 15120 = 609,638,400$

---

### 11.
Let $X=\lbrace a,b,c,d \rbrace$.  
(a) Compute the number of 3-combinations of X.  
(b) List the 3-combinations of X.  
(c) Compute the number of 3-permutations of X.  
(d) List the 3-permutations of X.  

### SOLUTION
(a) $C(4,3)=\frac{4!}{3!}=4$

(b) $abc, abd, acc, bcd$

(c) $P(4,3)=\frac{4!}{(4-3)!}=24$

(d)
$$
abc,acb,bac,bca,cab,cba\\
bcd,bdc,cbd,cdb,dbc,dcb\\
acd,adc,cad,cda,dac,dca\\
abd,adb,bad,bda,dab,dba\\
$$

---

### 12.
Show that the number of $n$-bit strings having exactly $k$ 0’s with no two 0’s consecutive, is $C(n − k + 1, k)$.

### SOLUTION
A $n$-bit string with exactly $k$ 0's has $n-k$ 1's. We will insert $k$ 0's into $n-k+1$ slots in order to avoid consecutive 0, and $n-k+1 > k$. So we choose $k$ out of $n-k+1$ slots, there are $C(n-k+1, k)$ ways.

## Generalized Permutations and Combinations
### 13.
Determine the number of strings that can be formed by ordering the letters given.


$$MESSINESS$$

### SOLUTION
There are total 9 letters in the word $MESSINESS$, which has 2 $E$'s and 4 $S$'s. According to theorem 6.3.2, the number orderings is

$$\frac{9!}{1!2!4!1!1!}=\frac{362880}{2 \times 24}=7560$$

---

### 14.
Suppose there are piles of identical red, blue, and green balls where each pile contains at least 10 balls.  
(a) In how many ways can 10 balls be selected?  
(b) In how many ways can 10 balls be selected if at least one red ball must be selected?  
(c) In how many ways can 10 balls be selected if at most one red ball must be selected?  

### SOLUTION
(a) Select 10 balls from 3 colors, according to theorem 6.3.5, the number of different combinations is
$k=10,\ t=3 \quad C(k+t-1, t-1)=C(10+3-1, 3-1)=C(12,2)=66$

(b) If at least one red ball must be selected, the problem becomes select 9 balls from 3 colors. $k=9,\ t=3 \quad C(k+t-1, t-1)=C(9+3-1, 3-1)=C(11,2)=55$

(c) If at most one red ball must be selected, there are 2 cases:  
1. **0 red ball is selected** select 10 balls from 2 colors, $k=10,\ t=2 \quad C(k+t-1, t-1)=C(10+2-1, 2-1)=C(11,1)=11$
2. **1 red ball is selected** select 9 balls from 2 colors, $k=9,\ t=2 \quad C(k+t-1, t-1)=C(9+2-1, 2-1)=C(10,1)=10$  
Total number of of ways is $11+10=21$