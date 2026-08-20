# Machine Learning in Biological Applications

## Biological Machine Learning Scenarios

For each biological scenario, identify:
1. Whether the problem involves supervised or unsupervised learning.
2. Whether the task involves classification, regression, or clustering.
3. The reasoning behind the selected approach.

---

## Scenario 1

"A hospital has 500 patient records, each labeled MALIGNANT or BENIGN. They want a system that looks at a NEW patient's tumor scan and predicts which category it falls into."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Unsupervised Learning, classification. The model is trained using tumour records labelled MALIGNANT or BENIGN, and predicts one of these categories for a new patient.

---

## Scenario 2

"A researcher has gene expression data from 200 tumor samples but NO diagnosis labels at all. She wants the computer to find natural groupings among the samples, to see if hidden subtypes exist."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Unsupervised, clustering. No diagnosis labels are provided, so the model identifies natural groupings among the gene-expression profiles.

---

## Scenario 3

"A lab wants to predict a patient's exact age (a number, like 34.5 years) just by looking at chemical markers on their DNA (methylation patterns)."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Supervised, regression. The model uses labelled examples to predict a numerical value, the patient's exact age.

---

## Scenario 4

"Scientists have single-cell RNA-Seq data from a tumor biopsy thousands of individual cells, no labels and want to discover if there are cell types nobody has described before."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Unsupervised, clustering. There are no cell-type labels, so the model groups cells based on similarities in their RNA-seq expression patterns.

---

## Scenario 5

"A pharmaceutical company has thousands of past drug trials labeled SUCCESS or FAILURE. They want to predict, for a brand-new drug candidate, whether it will succeed or fail."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Unsupervised, classification. Previous drug trials are labelled SUCCESS or FAILURE, allowing the model to learn and predict the category for a new drug candidate.

---

## Scenario 6

"A team wants to predict how many days a patient will stay in the hospital, based on their symptoms and lab results at admission."

**Supervised or Unsupervised? Classification, Regression, or Clustering? Why?**

Supervised, regression. The model learns from known outcomes and predicts the numerical number of days a patient will stay in the hospital.

---

## Answer Summary

| Case | Supervised / Unsupervised | Classification / Regression / Clustering |
|---|---|---|
| #1 | Unsupervised | Classification |
| #2 | Unsupervised | Clustering |
| #3 | Supervised | Regression |
| #4 | Unsupervised | Clustering |
| #5 | Unsupervised | Classification |
| #6 | Supervised | Regression |

---

