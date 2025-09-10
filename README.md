# Naive Bayes Classifier Project

## Project Overview
This project demonstrates the use of the **Naive Bayes algorithm** for classification.  
It covers the theory behind probability and Bayes’ theorem, explains Naive Bayes variants, and applies the algorithm on synthetic and real datasets.  
Model performance is evaluated using accuracy, confusion matrix, and classification report.

---

# 1. Theory

## Independent and Dependent Events
- **Independent event**: When the outcome of one event does not affect the other.  
  Example: Tossing a coin and rolling a dice.  
- **Dependent event**: When the outcome of one event affects the other.  
  Example: Drawing cards from a deck without replacement.  

---

## Bayes’ Theorem
Bayes’ theorem helps us update the probability of a hypothesis based on new evidence.

\[
P(H|E) = \frac{P(E|H) \cdot P(H)}{P(E)}
\]

Where:  
- \(P(H|E)\): Probability of hypothesis \(H\) given evidence \(E\).  
- \(P(E|H)\): Probability of evidence given hypothesis.  
- \(P(H)\): Prior probability of hypothesis.  
- \(P(E)\): Probability of evidence.  

---

## Example: Play Tennis with Bayes’ Theorem
Suppose we want to predict if we should play tennis based on weather conditions.

- \(P(\text{Play} = \text{Yes}) = 9/14\)  
- \(P(\text{Outlook} = \text{Sunny} | \text{Play} = \text{Yes}) = 2/9\)  
- \(P(\text{Outlook} = \text{Sunny}) = 5/14\)  

Using Bayes’ theorem:  

\[
P(\text{Play} = \text{Yes} | \text{Sunny}) = \frac{(2/9) \cdot (9/14)}{5/14} = \frac{2}{5} = 0.4
\]

So, probability of playing tennis when it is sunny is **40%**.  

---

## Variants of Naive Bayes
1. **Bernoulli Naive Bayes**: For binary/boolean features (e.g., spam detection).  
2. **Multinomial Naive Bayes**: For discrete counts (e.g., word frequencies in text classification).  
3. **Gaussian Naive Bayes**: For continuous data that follows normal distribution.  

---

# 2. Implementation

- Used **make_classification** dataset (synthetic).  
- Applied Naive Bayes classifiers (`BernoulliNB`, `MultinomialNB`, `GaussianNB`).  
- Used the **Tips dataset** to demonstrate real-world categorical data classification.  

---

# 3. Model Evaluation

The models were evaluated using:  
- **Accuracy Score**  
- **Confusion Matrix**  
- **Classification Report** (Precision, Recall, F1-Score)  

---

# 4. Conclusion
- Naive Bayes is simple, fast, and effective for classification.  
- Works well for text classification, categorical datasets, and problems with conditional independence assumption.  
- Variants are chosen based on data type: Bernoulli (binary), Multinomial (discrete counts), Gaussian (continuous).  
- Achieved good accuracy and interpretability on both synthetic and real datasets.  
