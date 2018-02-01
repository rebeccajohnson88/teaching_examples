Teaching examples

Here is an outline to some code I have created as part of teaching and TA-related lectures and assignments.

1. **Activity to practice writing functions**: the example uses reports of potentially vaccine-linked adverse events to move students from using inefficient code to more efficient functions. Students have to recode a categorical age variable to the midpoint of each category -- for instance, "1-2 years" becomes 1.5, "30-39" years becomes 34.5, etc. They first do this using an if, else if, else chain within a for loop that involves a fairly manual coding of the midpoint. The rest of the code takes them step by step to create a function "agemidfunc" that takes in a vector of age coded categorically and returns a vector with the midpoint of age. The inside of the function uses regular expressions to parse a category like "1-2 years" into the useful digits (1 and 2) and non-useful characters (- and "years"), and then calculate the midpoint.

2. **Activity to practice E-M algorithm**: the example has students practice coding and applying the E-M algorithm to estimate a multivariate normal model on wine-data defined by three clusters, defined by two dimensions (e.g., phenol content and acidity). The E-M algorithm is used to estimate the mean of, and covariance between, the two dimensions, for each of the clusters.


3. **Activity to practice k-fold validation and programming a likelihood function**: the example combines two activities. First, students practice writing a function to apply cross-validation on a dataset related to views about the Iraq war with a binary outcome variable. Then, students switch from the binary outcome variable to a Likert-type scale variable in the same data. Because either ordered logit or ordered probit models are most applicable to Likert-type scale variables where we are unsure about the relative spacing between categories, the students practice programming a function for the log-likelihood for this model (loglik.probit) and then maximize the likelihood using optim.

