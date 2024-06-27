
## **Math Induction.**
### 1. *Using Math Induction, prove that for every positive integer n,*
$$1(1!) + 2(2!) + · · · + n(n!) = (n + 1)! − 1$$

### **SOLUTION**
* Basis Step (n = 1)
$$
\begin{align}
  1(1!) = 1 * 1 = 1\\
\begin{split}
  (1 + 1)! - 1 &= 2!-1\\
  &=2*1-1\\
  &=1
\end{split}
\end{align}
$$
$(1) = (2)$
* Inductive Step  
Assume *the equation is true for n*  
$$
1(1!)+2(2!)+...+n(n!) = (n+1)!-1
$$

* Now
$$
\begin{split}
\color{red}1(1!)+2(2!)+...+n(n!) + \color{blue}(n+1)((n+1)!)&=\color{red}(n+1)!-1 + \color{blue}(n+1)((n+1)!)\\
&=((n+1)!)(n+2)-1\\
&=(n+2)!-1\\
&=(\bold{(n+1)}+1)!-\bold{1}\\
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
  2(n+1)+1 &= 2n+2+1\\
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
11^(n+1) - 6 &= 11^n \times 11 - 6\\
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

### 4. Let the universe be the set $U = \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\}$. Let $A = \{1, 4, 7, 10\}, B = \{1, 2, 3, 4, 5\} and C = \{2, 4, 6, 8\}$. List the elements of each set.
(a) $B \cap C$

(b) $\bar{A}-B$

(c) $A \cup B − (C − B)$

### SOLUTION
(a) 
$$B \cap C = \{1, 2, 3, 4, 5\} \cap \{2, 4, 5, 8\} = \{2, 4\}\\$$

(b) 
$$
\begin{split}
&\bar{A}-B = (U - A) - B \\
&= \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\} - \{1, 4, 7, 10\} - \{1, 2, 3, 4, 5\} \\
&= \{6, 8, 9\}\\
\end{split}
$$

(c) 
$$
\begin{split}
&A \cup B − (C − B) \\
&= \{1, 4, 7, 10\} \cap \{1, 2, 3, 4\} - (\{2, 4, 6, 8\} - \{1, 2, 3, 4\}) \\
&= \{1, 2, 3, 4, 6, 8\} - \{6, 8\}\\
&= \{1, 2, 3, 4\}\\
\end{split}
$$

---

### 5. Let $A = \{x|x^2-4x+4=1\}$ and $B=\{1, 3\}$. Prove that $A = B$.
### SOLUTION
1. prove $\forall{x| x \in A},\ x \in B\\$
Solving the equation $x^2 -4x + 4 = 1$, we find that $x=1\ or\ x=3\\$
Therefore $\forall{x| x \in A},\ x \in B$
2. prove $\forall{x| x \in B},\ x \in A\\$
   if x = 1, 
   $1^2-4 \times 1 + 4 = 1-4+4=1$, therefore $x \in A\\$
   if x = 3,
   $3^2-4 \times 3 + 4 = 9-4 \times 3 + 4=1$, again $x \in A\\$

We conclude that $A=B$

---

### 6. Let $X=\{1, 2\}$ and $Y=\{a, b, c\}$. List the elements in each set.
(a) $X \times Y\\$
(b) $Y \times X\\$
(c) $X \times X \times X\\$

### SOLUTION
(a)
$$
\begin{split}
&X \times Y\\
&=\{1, 2\} \times \{a, b, c\}\\
&=\{\{1, a\}, \{1, b\}, \{1, c\}, \{2, a\}, \{2, b\}, \{2, c\}\}
\end{split}
$$

(b)
$$
\begin{split}
&Y \times X\\
&=\{a, b, c\} \times \{1, 2\}\\
&=\{\{a, 1\}, \{a, 2\}, \{b, 1\}, \{b, 2\}, \{c, 1\}, \{c, 2\}\}
\end{split}
$$

(c)
$$
\begin{split}
&X \times X \times X\\
&=\{1, 2\} \times \{1, 2\} \times \{1, 2\}\\
&=\{\{1,1\}, \{1,2\}, \{2,1\}, \{2,2\}\} \times \{1,2\}\\
&=\{\\
&\qquad\{\{1,1\},1\},\quad\{\{1,1\},2\},\\
&\qquad\{\{1,2\},1\},\quad\{\{1,2\},2\},\\
&\qquad\{\{2,1\},1\},\quad\{\{2,1\},2\},\\
&\qquad\{\{2,2\},1\},\quad\{\{2,2\},2\}\\
&\quad\}
\end{split}
$$