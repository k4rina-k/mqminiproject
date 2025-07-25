
---
permalink: /toolstech/
title: "Tools & Techniques"
---

A Tools/Techniques section that at minimum talks about the Mathematics areas/tools/techniques that are related to this topic. Optional: Section would discuss what tools you would use to undertake the project (think about the math concepts and hands-on techniques you’ve learned)

This project combines mathematical modeling, quantum computing, and biomedical data analysis to explore rectal cancer outcome prediction through quantum machine learning.

The foundation of this research rests on key mathematical and quantum mechanical principles, many of which I learned through the MathQuantum program:

**Linear Algebra:** for describing qubit states using vectors and matrices, and understanding quantum circuit operations like rotations and entanglement.

**Optimization:** to train the Variational Quantum Classifier (VQC) by minimizing a cost function over a high-dimensional parameter space using classical optimizers.

**Statistics & Variable Selection:** skills from my previous work using Ridge, LASSO, SCAD, and ElasticNet regression are applied here for preprocessing and comparison.


From MathQuantum, I developed a strong conceptual grounding in:

**Qubits and Superposition** – fundamental units of quantum and classical information

Superposition and the Bloch Sphere – visualizing quantum states as points on a sphere and encoding features as rotations

Entanglement and Interference – allowing qubits to represent relationships between clinical variables that classical models struggle with

Measurement and Error Correction – critical for extracting information from quantum circuits while addressing noise

Applying Quantum Gates – including the X-gate to flip qubit states and create complex superpositions

These concepts are directly applied in building, simulating, and training the quantum model.

⚙️ Software Tools & Implementation
To apply these mathematical concepts and quantum techniques, I will use:

Python – for preprocessing and interfacing with quantum backends

Qiskit – to design quantum circuits, encode features using rotation gates (e.g., RY), and simulate quantum measurements

Qiskit Machine Learning – to build and train a Variational Quantum Classifier

Scikit-learn & Pandas – to split data, normalize features, and benchmark against classical models

Matplotlib & Qiskit Visualizations – for rendering Bloch spheres, quantum circuits, and outcome comparisons

🛠️ Applied Experience
In my prior research, I applied statistical models to a real clinical dataset of 55 rectal cancer patients. I identified variables like lymph node involvement and clinical M-stage as significant predictors of outcomes. This experience taught me how to handle small, high-dimensional medical data—perfectly suited for quantum methods like VQC, which are optimized for low-data, high-complexity tasks.

This project applies both classical and quantum mathematical thinking to develop a working prototype of a cancer prediction model that explores whether quantum models can offer new insight or predictive power in a real-world clinical setting.
