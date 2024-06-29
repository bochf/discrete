
## **Math Induction.**
### 1. *Using Math Induction, prove that for every positive integer n,*
$$1(1!) + 2(2!) + · · · + n(n!) = (n + 1)! − 1$$

### **SOLUTION**
* Basis Step (n = 1)

$$1(1!) = 1 * 1 = 1 \tag{1}$$

$$
\begin{aligned}
  (1 + 1)! - 1 &= 2!-1\\
  &=2*1-1\\
  &=1 
\end{aligned}
\tag{2}
$$

$$(1) = (2)$$
* Inductive Step  
Assume *the equation is true for n*

$$
1(1!)+2(2!)+...+n(n!) = (n+1)!-1
$$

* Now

$$
\begin{split}
&\color{red}1(1!)+2(2!)+...+n(n!) + \color{blue}(n+1)((n+1)!)\\
&=\color{red}(n+1)!-1 + \color{blue}(n+1)((n+1)!)\\
&=((n+1)!)(n+2)-1\\
&=(n+2)!-1\\
&=((n+1)+1)!-1\\
\end{split}
$$

Since the Basis Step and the Inductive Step have been verified, the Principle of Mathematical Induction tells us that $1(1!) + 2(2!) + · · · + n(n!) = (n + 1)! − 1$ is true for all the positive integers $n$.  

---

### 2. *Using Math Induction, prove that for every positive integer $n \ge 3$,*
$$2n + 1 \le 2^n$$

### **SOLUTION**
* Basis Step (n = 3)
$$2*3 + 1=7\tag{1}$$
$$2^3 = 8\tag{2}$$
$$(1) < (2)$$

* Inductive Step  
Assume *the inequation is true for n*
$$2n + 1 \le 2^n$$

* Now  

$$
\begin{split}
  &2(n+1)+1 \\
  &= 2n+2+1\\
  &=2n+1+2\\
  &\le 2^n+2\\
  &\lt 2^n + 2^n  \ (\forall n\ge3)\\
  &=2^{n+1}\\
\end{split}\\
$$

Since the Basis Step and the Inductive Step have been verified, the Principle of Mathematical Induction tells us that $2n + 1 \le 2^n$ is true for every positive integer $n \ge 3$

---

### 3. Using Math Induction, prove that
$11^n − 6$ is divisible by 5, for all n ≥1

### SOLUTION

* Basis Step (n = 1)
$$11 ^ 1 - 6 = 5$$
$$5 \bmod 5 = 0$$

* Inductive Step
Assume $11^n - 6$ is divisible by 5 for n, i.e. 
$$(11^n - 6) \bmod 5 = 0$$

* Now

$$
\begin{split}
&11^{n+1} - 6\\
&= 11^n \times 11 - 6\\
&=(10 + 1) \times 11^n -6\\
&=10 \times 11^n + (11^n - 6)\\
\end{split}
$$
$$
\because
10 \times 11^n \bmod 5 = 0 \And 11^n-6 \bmod 5 = 0
\therefore 11^(n+1)-6 \bmod 5 = 0
$$

Since the Basis Step and the Inductive Step have been verified, the Principle of Mathematical Induction tells us that 
$$(11^n - 6) \bmod 5 = 0$$

---

## **Set**

### 4. Let the universe be the set $U = \lbrace 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 \rbrace $. Let $A = \lbrace 1, 4, 7, 10 \rbrace , B = \lbrace 1, 2, 3, 4, 5 \rbrace \ and \ C = \lbrace 2, 4, 6, 8 \rbrace $. List the elements of each set.
(a) $B \cap C$

(b) $\bar{A}-B$

(c) $A \cup B − (C − B)$

### SOLUTION
(a) $$B \cap C = \lbrace 1, 2, 3, 4, 5 \rbrace  \cap \lbrace 2, 4, 5, 8 \rbrace  = \lbrace 2, 4 \rbrace $$

(b) 

$$
\begin{split}
&\bar{A}-B = (U - A) - B \\
&= \lbrace 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 \rbrace  - \lbrace 1, 4, 7, 10 \rbrace  - \lbrace 1, 2, 3, 4, 5 \rbrace  \\
&= \lbrace 6, 8, 9 \rbrace \\
\end{split}
$$

(c) 

$$
\begin{split}
&A \cup B − (C − B) \\
&= \lbrace 1, 4, 7, 10 \rbrace  \cap \lbrace 1, 2, 3, 4 \rbrace  - (\lbrace 2, 4, 6, 8 \rbrace  - \lbrace 1, 2, 3, 4 \rbrace ) \\
&= \lbrace 1, 2, 3, 4, 6, 8 \rbrace  - \lbrace 6, 8 \rbrace \\
&= \lbrace 1, 2, 3, 4 \rbrace \\
\end{split}
$$

---

### 5. Let $A = \lbrace x|x^2-4x+4=1 \rbrace $ and $B=\lbrace 1, 3 \rbrace $. Prove that $A = B$.
### SOLUTION
1. prove $\forall{x| x \in A},\ x \in B$

  Solving the equation $x^2 -4x + 4 = 1$, we find that $x=1\ or\ x=3$  
  Therefore $\forall{x| x \in A},\ x \in B$

2. prove $\forall{x| x \in B},\ x \in A$

   if x = 1,  
   $1^2-4 \times 1 + 4 = 1-4+4=1$, therefore $x \in A$  
   if x = 3,  
   $3^2-4 \times 3 + 4 = 9-4 \times 3 + 4=1$, again $x \in A$

We conclude that $A=B$

---

### 6. Let $X=\lbrace 1, 2 \rbrace $ and $Y=\lbrace a, b, c \rbrace $. List the elements in each set.
(a) $X \times Y\\$
(b) $Y \times X\\$
(c) $X \times X \times X\\$

### SOLUTION
(a)

$$
\begin{aligned}
&X \times Y\\
&=\lbrace 1, 2 \rbrace  \times \lbrace a, b, c \rbrace \\
&=\lbrace \lbrace 1, a \rbrace , \lbrace 1, b \rbrace , \lbrace 1, c \rbrace , \lbrace 2, a \rbrace , \lbrace 2, b \rbrace , \lbrace 2, c \rbrace  \rbrace 
\end{aligned}
$$

(b)

$$
\begin{aligned}
&Y \times X\\
&=\lbrace a, b, c \rbrace  \times \lbrace 1, 2 \rbrace \\
&=\lbrace \lbrace a, 1 \rbrace , \lbrace a, 2 \rbrace , \lbrace b, 1 \rbrace , \lbrace b, 2 \rbrace , \lbrace c, 1 \rbrace , \lbrace c, 2 \rbrace  \rbrace 
\end{aligned}
$$

(c)

$$
\begin{aligned}
&X \times X \times X\\
&=\lbrace 1, 2 \rbrace  \times \lbrace 1, 2 \rbrace  \times \lbrace 1, 2 \rbrace \\
&=\lbrace \lbrace 1,1 \rbrace , \lbrace 1,2 \rbrace , \lbrace 2,1 \rbrace , \lbrace 2,2 \rbrace  \rbrace  \times \lbrace 1,2 \rbrace \\
&=\lbrace \\
&\qquad\lbrace \lbrace 1,1 \rbrace ,1 \rbrace ,\quad\lbrace \lbrace 1,1 \rbrace ,2 \rbrace ,\\
&\qquad\lbrace \lbrace 1,2 \rbrace ,1 \rbrace ,\quad\lbrace \lbrace 1,2 \rbrace ,2 \rbrace ,\\
&\qquad\lbrace \lbrace 2,1 \rbrace ,1 \rbrace ,\quad\lbrace \lbrace 2,1 \rbrace ,2 \rbrace ,\\
&\qquad\lbrace \lbrace 2,2 \rbrace ,1 \rbrace ,\quad\lbrace \lbrace 2,2 \rbrace ,2 \rbrace \\
&\quad \rbrace 
\end{aligned}
$$

---

### 7. Suppose there is a group of 191 students, of which 10 are taking French, business, and music; 36 are taking French and business; 20 are taking French and music; 18 are taking business and music; 65 are taking French; 76 are taking business; and 63 are taking music.
(a) How many are taking none of the three subjects?  
(b) Draw a Venn Diagram to illustrate the universal set U of students, set F those students taking
French, set B for those students taking business, and set M for those students taking music.
Write the number of students belonging each region depicted in the diagram.

### SOLUTION
(a) Let 
- U = all the students
- F = all the students taking French
- B = all the students taking business
- M = all the students taking music
$$
\begin{split}\tag{Given}
&|U| = 191\\
&|F| = 65\\
&|B| = 76\\
&|M| = 63\\
&|F \cap B \cap M| = 10\\
&|F \cap B| = 36\\
&|F \cap M| = 20\\
&|B \cap M| = 18
\end{split}
$$
Therefor
$$
\begin{split}\tag{Inclusion-Exclusion Principle}
&\quad|\bar{F} \cap \bar{B} \cap \bar{M}|\\
&= |U| - (|F| + |B| + |M|) + (|F \cap B| + |F \cap M| + |B \cap M|) - |F \cap B \cap M|\\
&= 191 - (65 + 76 + 63) + (36 + 20 + 18) - 10\\
&= 51
\end{split}
$$

(b)