### 5 Generalized Permutations and Combinations.
(a) [5pts] How many strings can be formed by arranging the 8 letters of
 $$GIGGLING$$

(b) [5pts] How many solutions in nonnegative integers are there to the following equation
$$x1 +x2 +x3 +x4 =25$$

### SOLUTION
(a) 
Total number of letters in GIGGLING: 8
There are 4 $G$s and 2 $I$s
The number of distict strings can be formed is
$$
\frac{8!}{4!2!1!1!}=\frac{40320}{24\times2}=840
$$

(b)
For each $x_i$, the range is $[0, 25]$, so we will divide 25 into 4 variables
$$
k = 25, t=4\\
C(k+t-1,t-1)=C(28, 3)=19656
$$

---

### 4
 (a) [2pts] Basic Principles. How many ways can you award a gold medal, a silver medal, and a bronze medal to the top three nishers, respectively, in an event where 7 Olympians are competing, assuming there are no ties

 $P(7,3)=210$

 (b) [2pts] Basic Principles. How many bit strings have length at least 7 and at most 8

 $2^7+2^8=384$

 (c) [2pts] Basic Principles. How many 8-bit strings begin with 101 or end with 11 or both

 $2^5+2^6-2^3=32+64-8=88$

 (d) [2pts] Permutations and Combinations. How many different ways could you  rank the top 5 songs from a collection of 8 songs

 $P(8, 5) = 6720$

 (e) [2pts] Permutations and Combinations. How many 16-bit strings contain exactly 10 1s

 $C(16,10)=8008$

---

### 3
(a) [4pts] Let R be the relation $\lbrace(1,1), (2,2), (3,3), (1,3)\rbrace$ on the set $X = \lbrace1, 2,3\rbrace$ . 
Is R an equivalence relation on X? 
If R is, describe the partition F determined by R by listing the members of F. 
If R is not, state precisely which properties of an equivalence relation it is lacking and justify

(b) [6pts] Let X = ab c and let F = ab c . Describe the equivalence relation R on X determined by the partition F by listing the ordered pairs in R. Determine [b], the equivalence class of b.

### SOLUTION
(a) R is not an equivalence relation on X, because R is not symmetric, $(1,3) \in R$ but $(3,1) \not \in R$

(b) 
The equivalence relation R on X determined by the partition $\mathcal{F}$ is
$R=\lbrace(a,a), (b,b), (c,c), (a,b), (b,a)\rbrace$

The equivalence class $[b] = \lbrace a,b \rbrace$

---

### 2
(a) Sets. Let A = {2,3,5,6,8,9} ,B = (1,3,4,5,7,9} ,C = 123 ,andD= 56 . Find the following sets.

 i. [1pt] $A\cap B = {3,5,9}$

 ii. [1pt] $B \cup D = {1,3,4,5,6,7,9}$

 iii. [1pt] A-B = {2,6,8}

 iv. [1pt] $D \times C= {(5,1), (5,2), (5,3), (6,1), (6,2), (6,3)$

 v. [1pt] $\mathcal{P}(D)= \lbrace \emptyset, \rbrace$
