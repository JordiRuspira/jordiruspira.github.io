---
title: "Machine Learning With a Heart"
date: 2018-10-01
tags: [machine learning, data science, health]
header:
  image: "/images/mlheart/Morning-Dew.jpg"
excerpt: "Machine Learning, Health, Data Science"
mathjax: "true"
---
*(This post is under construction, and its content may have features from different sources. Once completed, I will update all the sources correctly.)*

# Introduction

Cardiovascular diseases (those diseases of the heart, blood vessels) are the **number 1 cause of death worldwide**, accounting for over 17 milion deaths per year (two times more than death caused by cancers), acording to the *World Heart Federation*. We can see a few more data in the following infographic:

<img src="{{ site.url }}{{ site.baseurl }}/images/mlheart/heart1.png" alt="heart1">

Thus, preventing heart diseases should be a global goal towards ending the major cause of death worldwide and its consequences.

## Adressing the problem

One of the best and most advanced methods towards prediction and therefore better understanding of heart diseases is a data-driven approach. For this project, we will work with the data from the following [DrivenData competition](https://drivendata.org/competitions/54/machine-learning-with-a-heart/). The study collects various measurements on patient health and cardiovascular statistics, making patient identities anonymous.

As stated in the competition, our goal is to predict the binary class heart_disease_present, which represents whether or not a patient has heart disease:
* *0* represents no heart disease present
* *1* represents heart disease present

There are 14 columns in the dataset, where the patient_id column is a unique and random identifier. The remaining 13 features are described in the section below.

* *slope_of_peak_exercise_st_segment* (type: int): the slope of the peak exercise ST segment, an electrocardiography read out indicating quality of blood flow to the heart
* *thal* (type: categorical): results of thallium stress test measuring blood flow to the heart, with possible values normal, fixed_defect, reversible_defect
*  *resting_blood_pressure* (type: int): resting blood pressure
* *chest_pain_type* (type: int): chest pain type (4 values)
* *num_major_vessels* (type: int): number of major vessels (0-3) colored by flourosopy
* *fasting_blood_sugar_gt_120_mg_per_dl* (type: binary): fasting blood sugar > 120 mg/dl
* *resting_ekg_results* (type: int): resting electrocardiographic results (values 0,1,2)
* *serum_cholesterol_mg_per_dl* (type: int): serum cholestoral in mg/dl
* *oldpeak_eq_st_depression* (type: float): oldpeak = ST depression induced by exercise relative to rest, a measure of abnormality in electrocardiograms
* *sex* (type: binary): 0: female, 1: male
* *age* (type: int): age in years
* *max_heart_rate_achieved* (type: int): maximum heart rate achieved (beats per minute)
* *exercise_induced_angina* (type: binary): exercise-induced chest pain (0: False, 1: True)


Python code block:
```python
    import numpy as np

    def test_function(x, y):
      z = np.sum(x,y)
      return z
```

Here's some inline code `x+y`.

Here's some math:

$$z=x+y$$

You can also put it inline $$z=x+y$$
