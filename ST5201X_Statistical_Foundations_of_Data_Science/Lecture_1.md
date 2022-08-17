In this section, we would review some knowledge in probability and statistics.

# 1. Discrete Random Variables

First, the note will introduce some common discrete variables.

## 1.1 Bernoulli random variable

A Bernoulli random variable $X$ takes on only two values: $0$ and $1$, with probabilities $1 - p$ and
$p$, respectively. It is can be called two point distribution.

The probability mass function (pmf) of $X$ is

$$
\begin{equation}
 P(X=x)= \begin{cases}
 p^{x}(1-p)^{1-x},\quad \text { if } x=0 \text { or } x=1 \\
0, \quad \text { otherwise }
 \end{cases}
\end{equation}
$$





# 2. Continuous Random Variables

# 3. Functions of a Random Variable

# 4. Joint Distributions

# 5. Independent Random Variables

# 6. Conditional Distributions

## 6.1 The Discrete Case

**Definition**

If $X$ and $Y$ are jointly distributed discrete random variables, the conditional probability that $X=x_i$ given that $Y=y_i$ is, if  $p_Y(y_i)>0$, 

$$
P_{X|Y}=P(X=x_i|Y=y_i)=\frac{P(X=x_i,Y=y_i)}{P(Y=y_i)}=\frac{p_{XY}(x_i,y_i)}{p_Y(y_i)}
$$

If $p_Y(y_i)=0$, then the probability is defined to be $0$



**Corollary**

**The Law of total probability**:

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




