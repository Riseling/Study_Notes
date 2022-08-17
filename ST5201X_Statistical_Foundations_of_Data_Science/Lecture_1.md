In this section, we would review some knowledge in probability and statistics.

# 1. Discrete Random Variables

First, the note will introduce some common discrete variables.

## 1.1 Bernoulli random variable

A Bernoulli random variable $X$ takes on only two values: $0$ and $1$, with probabilities $1 - p$ and
$p$, respectively. It is can be called two point distribution.

Then, it can be denoted $X\sim \text B(p)$.

The probability mass function (pmf) of $X$ is

$$
\begin{equation}
 P(X=x)= \begin{cases}
 p^{x}(1-p)^{1-x},\quad \text { if } x=0 \text { or } x=1 \\
0, \quad \text { otherwise }
 \end{cases}
\end{equation}
$$

And the expectation and variance are:

$$
\begin{align}
E(X) &=p \\
Var(X) &= p(1-p)
\end{align}
$$

## 1.2 Binomial random variable

Suppose that $n$ independent Bernoulli trials are performed, where $n$ is a fixed number, and that each trial results in a “success” with probability $p$ and a “failure” with probability $1-p$. The total number of successes, $X$, is a binomial random variable with parameters $n$ and $p$.

It can be denoted that $X \sim \text{Bin}(n,p) $

$$
\begin{equation}
P(X=k) = \binom{n}{k} p^k (1-p)^{n-k}
\end{equation}
$$

And the expectation and variance are:

$$
\begin{align}
E(X) &=np \\
Var(X) &= np(1-p)
\end{align}
$$

## 1.3 Geometric random variable

$X$ is the number of trials until the first success with probability $p$, denoted as $X \sim \text{Geo}(p)$
$$
\begin{equation}
P(X=k)= (1-p)^{k-1} p
\end{equation}
$$

And the expectation and variance are:

$$
\begin{align}
E(X) &=\frac{1}{p} \\
Var(X) &= \frac{1-p}{p^2} 
\end{align}
$$

## 1.4 Negative binomial random variable

$X$ denotes the total number of trials until $r$-th success  with probability $p$, denoted as $X\sim \text{NB}(k,r,p)$ and pmf is:

$$
P(X=k)= \binom{k-1}{r-1}(1-p)^{k-r} p^r, \quad k=r,r+1,...
$$

And the expectation and variance are:

$$
\begin{align}
E(X) &=\frac{r}{p} \\
Var(X) &= \frac{r(1-p)}{p^2}
\end{align}
$$

**Remark 1**: The reason why it is called negative binomial is that

$$
\begin{align*}
\binom{k-1}{r-1} &=  \frac{(k-1)!}{(r-1)!(k-r)!}  = \frac{(k-1)(k-2)\cdots r}{(k-r)!}\\&= (-1)^{k-r}\frac{(-k+1)(-k+2)\cdots (-r)}{(k-r)!}  \\
&= (-1)^{k-r}\frac{(-k+1)(-k+2)\cdots (-r)(-k)!}{(k-r)!(-k)!} \\
&= (-1)^{k-r} \binom{-r}{k-r}
\end{align*}
$$

**Remark 2** Negative binomial distribution also has other definition, but the meanings are identical.
For example, $X$ is the **failure number** until $r$-th success. Then it can be denoted as $X\sim \text{NB}(k, r, p)$ and

$$
\begin{align}
P(X=k)= \binom{k+r-1}{r-1}(1-p)^k p^r
\end{align}
$$

## 1.5 Hypergeometric random variable

Suppose that an urn contains $n$ balls, of which $r$ are black and $n-r$ are white. Let $X$ denote the number of black balls drawn when taking $m$ balls without replacement, denoted as $X\sim \text{HG}(k,m,n)$

$$
 \begin{equation}
P(X=k)= \frac{\binom{r}{k} \binom{n-r}{m-k}}{\binom{n}{m}}
 \end{equation}
$$

the pmf is positive if $\max(0,m-(n-r))\le k \le \min(r,m)$

And the expectation and variance are:

$$
\begin{align}
E(X) &=\frac{km}{n} \\
Var(X) &= \frac{km(n-m)(n-k)}{n^2(n-1)}
\end{align}
$$

## 1.6 Poisson random variable

The Poisson frenquency with parameter $\lambda(\lambda>0)$ is:

$$
\begin{equation}
P(X=k)= \frac{\lambda^k}{k!} e^{-\lambda}, \quad k=0,1,2,...
\end{equation}
$$

And $X$ is denoted as $X \sim \text{Pois}(\lambda)$.

What's more, the **expectation** and **variance** are

$$
\begin{align}
E(X) = Var(X) = \lambda
\end{align} 
$$

# 2. Continuous Random Variables

# 3. Functions of a Random Variable

# 4. Joint Distributions

# 5. Independent Random Variables

# 6. Conditional Distributions

## 6.1 The Discrete Case

**Definition**: If $X$ and $Y$ are jointly distributed discrete random variables, the conditional probability that $X=x_i$ given that $Y=y_i$ is, if  $p_Y(y_i)>0$,

$$
P_{X|Y}=P(X=x_i|Y=y_i)=\frac{P(X=x_i,Y=y_i)}{P(Y=y_i)}=\frac{p_{XY}(x_i,y_i)}{p_Y(y_i)}
$$

If $p_Y(y_i)=0$, then the probability is defined to be $0$

**Corollary**: **The Law of total probability**:

$$
p_X(x)=\sum_yp_{X|Y}(x|y)p_Y(y)
$$

## 6.2 The Continuous Case

**Definition**

If $X$ and $Y$ are jointly continuous random variables, the conditional density of $Y$ given $X$ is defined to be 

$$
f_{Y|X}(y|x) = \frac{f_{XY}(x,y)}{f_X(x)}
$$

if $0<f_X(x)<\infty$, and $0$ otherwise.



**The Law of Total Probability**

$$
f_Y(y)=\int_{-\infty}^\infty f_{Y|X}(y|x) f_X(x) \mathrm d x
$$





# 7. Functions of Jointly Distributed Random Variables

# 8. Extrema and Order Statistics

# 9. Expected Values

# 10. Limit Theorems




