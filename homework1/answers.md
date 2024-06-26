
## 1. **Math Induction.**
*Using Math Induction, prove that for every positive integer n,*
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

## 2. **Math Induction.**
*Using Math Induction, prove that for every positive integer $n \ge 3$,*
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
