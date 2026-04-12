# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> This is a regression problem because our output is numeric (species richness, reserve size, budget). We are interested in inference because we want to understand a relationship between factors affecting species richness, rather than make predictions. n = 200, p = 4 (reserve size, years since establishment, enforcement budget, prox. to human settlements).

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> This is a classification problem because our response variable is categorical (unsuccessful vs successful). We are interested in prediction because we want to predict if a proposed corridor will support wildlife movement using data from 30 established corridors to make said prediction. n = 30, p = 11 (corridor length, width, land use type, + 8 more).

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> This is a regression problem because the response variable (ground-level ozone concentration) is a numeric continuous. We are interested in prediction because we want to predict weekly ozone concentration in a coastal city. n = 52 (weeks/year), p = 4 (wind speed, sea surface temp, solar radiation & atmospheric?).

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> A very flexible model can capture complex relationships in the data, leading to high accuracy and lower bias. However, its flexibility also makes it more prone to overfitting - capturing noise rather than the true pattern in the data. This can result in poor generalizability and high variance when applying it to new data. A less flexible model is less complex, more easily interpreted, and it reduces the risk of overfitting. In this case, generalizability is improved because the model not fit the data as tightly, and may perform better on new data. At the same time, less flexible models. At the same time, it can underfit the data and miss important patterns in it. 

When more flexible approach is preferred:
- When true relationship is complex and involves several factors that must be understood
- When sample size is large
- When high accuracy prediction is our main goal

When less flexible approach is preferred: 
- When sample size is small
- When interpretability is a primary goal 
- When the relationship is expected to be simple/ less complex.
---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> A parametric approach assumes a specific form for the relationship between predictors and response (linear regression, for example), and estimates a set number of parameters. It is simpler and easier to interpret, computationally more efficient, and requires less data. However, a parametric approach can be too restrictive. If the assumed form for the relationship is incorrect, the model will fail to capture the patterns in the data. A non-parametric does not assume a pre-defined form, instead it allows the data to determine the shape of the relationship. Thus, a non-parametric approach is more flexible and can capture complex relationships better. On the other hand, they require larger datasets and are more computationally intensive, as well as being more difficult to interpret. 