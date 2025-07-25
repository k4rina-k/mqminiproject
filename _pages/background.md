---
permalink: /background/
title: "Background"
---

This project is a continuation of research I've conducted.

Rectal cancer is a major global health issue, as it’s the second leading cause of cancer-related deaths worldwide, with over 46,000 new cases occurring in the U.S. in 2024. Unlike colon cancer, treating rectal cancer is complicated due to the rectum’s proximity to other organs, making accurate staging critical for treatment planning. While MRI technology has enhanced staging accuracy, identifying the most predictive pre-treatment variables remains an ongoing challenge in clinical research.

In my previous project, [“Can We Predict Rectal Cancer Outcomes Using Clinical Data? A Comparative Analysis of Different Techniques”](https://partner.projectboard.world/oas/project/can-we-predict-rectal-cancer-outcomes-using-clinical-data-geedyp?rc=5a933f42-9776-4496-afcc-49d1c7fa9a30) (Krishnan, 2025), I analyzed a high-dimensional dataset of 55 patients from Case Western Reserve University. I applied a range of statistical regression techniques—including Tobit, Logit, LASSO, Ridge, and ElasticNet—to determine which pre-surgical and MRI features significantly predicted TNM stage and recurrence. Notably, lymph node involvement and initial clinical M-staging emerged as consistent predictors across methods. However, as the data was small and complex, classical techniques had limitations in capturing nonlinear relationships and interactions between features.

This motivated a deeper exploration into quantum machine learning (QML). This promising field leverages quantum phenomena like entanglement and superposition to detect patterns that classical models may miss, especially in low-sample, high-dimensional settings like clinical oncology. 

Check out this video to see how QML compares to classical ML:
<iframe width="560" height="315" src="https://www.youtube.com/embed/-xAlAcKY8KY?si=S0KNm9Sm1nt_Go79" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


In this continuation project, I aim to build a Variational Quantum Classifier (VQC) trained on a subset of features from the same patient dataset to explore whether QML offers deeper insight or better performance than classical statistical approaches.

A study by Mari et al. (2020), [Transfer learning in hybrid classical-quantum neural networks](https://quantum-journal.org/papers/q-2020-10-09-340/pdf/),  demonstrated the use of hybrid classical-quantum neural networks, including Variational Quantum Classifiers, on clinical data from the UCI Breast Cancer dataset. By training quantum circuits on a reduced feature set, it was shown that quantum models can achieve strong performance even with limited data, highlighting the potential of VQCs for small-scale biomedical prediction tasks like mine. This supports the feasibility of applying VQCs to my rectal cancer dataset for both outcome prediction and feature relevance analysis.
