---
title: "Bayesian Average Mean"
date: 2023-06-15T11:47:22+01:00
draft: false
tags:
  - Bayesian Average Mean
  - Statistics
---
---


## The Bayesian average is a type of weighted average that incorporates prior knowledge or belief, in addition to the given data. This method is used when the data set is small, or when there is a need to prevent extreme values from skewing the results significantly.

In the context of online ratings, for example, the Bayesian average is often used to calculate average ratings in a way that reduces the impact of ratings from users who rate extremely high or low, especially when the total number of ratings is low.

Considering the risks that come with the framework's flexibility is essential. Mistakes and vulnerabilities can quickly arise, so it's crucial to be diligent and cautious when using them.

A simple Bayesian average can be computed as:

$${
\text{{Bayesian Average}} = \frac{{C \times M + \sum_{{i=1}}^N x_i}}{{C + N}}
}
$$


_Where:_

_C_ is a chosen constant that represents a kind of "confidence" in the global average.

_M_ is the global average rating.

_Sum_ is the sum of all ratings for a particular item.


```python
# Example of a Bayesian Average Mean in Python

avg_num_votes = 1370 # Average number of votes

avg_rating = 2.7; #Average rating
new_num_votes = 7  # New number of votes
new_rating = 5 # Expected rating

bayesian_rating = ( (avg_num_votes * avg_rating) + (new_num_votes * new_rating) ) / (avg_num_votes + new_num_votes)

print(bayesian_rating)

```
_The output of the code above is:_

```python
2.711692084241104

```

By applying the Bayesian average, these extreme cases are adjusted towards the average rating of all items on the site. This approach gives a more accurate and fair representation of the product’s rating, especially when there are not enough reviews.

However, the Bayesian average will gradually converge to the actual average rating as the number of reviews for a specific item increases and provides more data. This balances the need for reliability in low-data situations with the desire to reflect actual user opinions as accurately as possible when sufficient data is available.

The Bayesian average is a favoured statistical tool for many recommendation systems: it provides a more reliable estimate when data is sparse or potentially skewed by outliers.


## References
- https://stackoverflow.com/questions/6653215/bayesian-rating
- Bayesian Average Ratings, Evan Miller, https://www.evanmiller.org/bayesian-average-ratings.html
