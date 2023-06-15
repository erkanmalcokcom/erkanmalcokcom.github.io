---
title: "Preview Latex"
date: "May 31, 2023"
publishdate: "May 31, 2023"
katex: true
markup: 'mmark'
draft: true
tags: 
  - Statistics
  - Probability
---


Sure, here is the conversion from LaTeX to KaTeX. KaTeX is a subset of LaTeX, so most LaTeX commands will work in KaTeX without any changes. Here's the conversion of the above LaTeX to KaTeX:

The function \(B(5, 0.8)\) refers to a binomial distribution with 5 trials and a probability of success of 0.8. Here are some of its statistical properties:

- Mean: 4
- Standard Deviation: 0.894427
- Variance: 0.8
- Skewness: -0.67082
- Kurtosis: 3.05

$$\int x^3 dx$$
$$\ P (X = x) = $$


The probability density function (PDF) is given by:

```katex
P (X = x) = 
\begin{cases} 
0.2^{(5 - x)} \cdot 0.8^x \cdot \text{binomial}(5, x) & \text{for } 0 \leq x \leq 5 \\
0 & \text{otherwise}
\end{cases}
```

The cumulative distribution function (CDF) is given by:

```katex
P (X \leq x) = 
\begin{cases} 
I_{0.2}(5 - \lfloor x \rfloor, \lfloor x \rfloor + 1) & \text{for } 0 \leq x < 5 \\
1 & \text{for } x \geq 5
\end{cases}
```

Here are some probability results:

- Probability of all successes: 32.77%
- Probability of all failures: 0.032%
- Probability of at least one success: 99.97%
- Probability of at least one failure: 67.23%

Please note that the rendering of KaTeX will depend on the platform you are using to view it.