---
title: "Probability Theory: Unlocking the World of Chance"
date: "May 31, 2023"
publishdate: "May 31, 2023"
draft: false
tags: 
  - Statistics
  - Probability
---


In the world of mathematics, probability theory has a significant presence due to its application in myriad disciplines, from computer science to quantum physics, finance, and beyond. By the end of this blog post, you will appreciate and understand several critical aspects of probability theory, including how it is represented, calculated, and interpreted.

### Probability: A Measure of Uncertainty

Let's first appreciate that a probability is a number between 0 and 1, inclusive. In essence, probability quantifies the likelihood of an event happening. A probability of 0 signifies impossibility, a probability of 1 means certainty, and any value in between represents varying degrees of uncertainty. 

### Estimating Probability: A Data-Driven Approach

Given data, you can estimate a probability. Let's say you've recorded the weather for the past 100 days, and it rained on 30 of those days. The estimated probability of rain, in this case, would be the number of days it rained divided by the total number of days, or 30/100 = 0.3.

### Symmetry and Probability

Assumptions about symmetry often simplify probability calculations. For example, a fair die has six faces, each with an equal likelihood (1/6) of landing up when rolled. This is due to the symmetry of the die: each face has the same chance because the die is a regular cube.

### The ‘Settling Down’ Phenomenon

As a statistical experiment is repeated many times, we often observe a 'settling down' phenomenon. This is the Law of Large Numbers in action, which states that the average result from repeating an experiment multiple times will converge to the expected value.

### Probability Mass Function (PMF)

Probabilities of outcomes for discrete data are encapsulated in the PMF. For a discrete random variable X, the PMF is a function that gives the probability that X is exactly equal to a certain value. For instance, in a die roll (a discrete random variable), the PMF would assign a probability of 1/6 to each outcome from 1 to 6.

### Probability Density Function (PDF) 

For continuous data, probabilities are calculated using the PDF. A PDF describes the likelihood of a random variable taking a value within a particular range. Remember that the total area under the graph of a PDF is equal to 1, representing the total probability for all possible outcomes.

### Validating PMFs and PDFs

To check if functions claiming to be PMFs or PDFs are valid, you should ensure two conditions: all probabilities they give should be non-negative, and the sum (in the case of a PMF) or integral (in the case of a PDF) over all possible outcomes should be 1.

### Cumulative Distribution Function (CDF)

The CDF for a random variable is defined as the probability that the variable takes a value less than or equal to a certain value. The CDF for a discrete random variable can be found by summing up the probabilities of outcomes less than or equal to the given value, while for a continuous random variable, you would integrate the PDF.

### Calculating Probabilities

In simple situations, you can write down the PMF and the CDF of a discrete random variable and use these to calculate probabilities. For example, the probability of rolling a 3 or less on a fair die is the sum of the PMF values for 1, 2, and 3. 

You can use the CDF of a continuous random variable to calculate the probability of the variable lying within certain intervals. For example, to find the probability that a normally-distributed variable falls within one standard deviation of the mean, you would subtract the C