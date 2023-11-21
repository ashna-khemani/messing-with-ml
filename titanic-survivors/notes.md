# Notes
## Attempt 1: K-Nearest Neighbors
* **Why I tried it:** perhaps similar passengers would face similar fates. Ex: the lower-class passengers were likely to be trapped in the lower parts of the ship
* **Score:** 0.58133 
* **Reaction:** 😬 yikes. probably picked up on other patterns that were not as relevant to passenger class (for example, sex, number of siblings, parents...). I think we'd want something based more on probability/solid decisions instead of "proximity."
<br><br>
## Attempt 2: Naive Bayes (Gaussian)
* **Why I tried it:** more probability based. Pick up on and analyze the probability that someone with some set of features was likely to survive. Why Gaussian? There is discrete data (the fare) which would be not as suited to other forms of Naive Bayes
* **Score:** 0.75598 
* **Reaction:** 🤔 hmm... not terrible but definitely can be better. Maybe some of the loss comes from a general fact that probability can be influenced – perhaps we picked up on irrelevant features or misguiding patterns. We said after Attempt 1 we try something with more "solid decisions." Maybe we try a decision tree/random forest.