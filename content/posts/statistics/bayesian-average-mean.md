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

___ 
A simple Bayesian average can be computed as:
___ 

$${
\text{{Bayesian Average}} = \frac{{C \times M + \sum_{{i=1}}^N x_i}}{{C + N}}
}
$$


___ 
_Where:_

_C_ is a chosen constant that represents a kind of "confidence" in the global average.

_M_ is the global average rating.

_Sum_ is the sum of all ratings for a particular item.


___ 
```python
# Example of a Bayesian Average Mean in Python

avg_num_votes = 1370 # Average number of votes

avg_rating = 2.7; #Average rating
new_num_votes = 7  # New number of votes
new_rating = 5 # Expected rating

bayesian_rating = ( (avg_num_votes * avg_rating) + (new_num_votes * new_rating) ) / (avg_num_votes + new_num_votes)

print(bayesian_rating)
```

___ 
_The output of the code above is:_

```python
2.711692084241104

```
___

By applying the Bayesian average, these extreme cases are adjusted towards the average rating of all items on the site. This approach gives a more accurate and fair representation of the product’s rating, especially when there are not enough reviews.

However, the Bayesian average will gradually converge to the actual average rating as the number of reviews for a specific item increases and provides more data. This balances the need for reliability in low-data situations with the desire to reflect actual user opinions as accurately as possible when sufficient data is available.

The Bayesian average is a favoured statistical tool for many recommendation systems: it provides a more reliable estimate when data is sparse or potentially skewed by outliers.


## It's always important to understand your data's context and characteristics before choosing a statistical method.

### Pros of the Bayesian Average
* The Bayesian Average is excellent for situations with a wide disparity in the number of ratings per item. If an item has only a few ratings, a simple average might not be representative, and the Bayesian Average can provide a more balanced view.
* The Bayesian Average can reduce the impact of extreme ratings, especially when the total number of ratings is low.
* The Bayesian Average provides a broader context to an item's average by considering the average of all items in its calculation

### Cons of the Bayesian Average
* The Bayesian Average requires a global average to be calculated, which might not always be possible or meaningful, particularly in dynamic systems where new items are added frequently.
* The method requires you to choose a confidence level (represented by C in the formula), which can be somewhat subjective. This value represents the number of ratings you believe are needed before an item's own average becomes reliable. Different choices for this value can lead to different results.
* The Bayesian Average is more complex to calculate and understand than a simple average. This can make it more difficult to explain to users of a rating system how the average ratings are calculated.
* If the confidence level is set too high, items with a unique or niche appeal might be overshadowed because their Bayesian average will be heavily influenced by the global average.

## Please remember that the Bayesian Average may not be suitable for every situation. While it can be a valuable tool for dealing with sparse or skewed data, other solutions may work better in certain scenarios.

## References
- https://stackoverflow.com/questions/6653215/bayesian-rating
- Bayesian Average Ratings, Evan Miller, https://www.evanmiller.org/bayesian-average-ratings.html
