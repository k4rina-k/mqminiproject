---
permalink: /toolstech/
title: "Tools & Techniques"
---

This project combines mathematical modeling, quantum computing, and biomedical data analysis to explore rectal cancer outcome prediction through quantum machine learning.

## The foundation of this research rests on key mathematical and quantum mechanical principles, many of which I learned through the MathQuantum program:

**Linear Algebra:** for describing qubit states using vectors and matrices, and understanding quantum circuit operations like rotations and entanglement.

**Optimization:** to train the Variational Quantum Classifier (VQC) by minimizing a cost function over a high-dimensional parameter space using classical optimizers.

**Statistics & Variable Selection:** skills from my previous work using Ridge, LASSO, SCAD, and ElasticNet regression are applied here for preprocessing and comparison.


## From MathQuantum, I developed a strong conceptual grounding in:

### **Qubits and Superposition:** 

The qubit, or quantum bit, is the basic unit of quantum information. Unlike classical bits (0 or 1), a qubit can exist in a superposition:
$$
|\psi\rangle = \alpha|0\rangle + \beta|1\rangle \quad \text{where} \quad |\alpha|^2 + |\beta|^2 = 1
$$

In this project, each input clinical feature is mapped onto a qubit via rotation gates, creating superpositions that encode probabilistic behavior and uncertainty in medical variables.

### **Bloch Sphere:**
![bloch sphere](https://miro.medium.com/v2/resize:fit:500/1*ZtLUJ7OJJ-mtn5VvBJvUuA.png)

I learned how qubit states can be represented as points on the Bloch sphere, a geometric visualization of pure states. This is particularly important when performing angle encoding, where a normalized clinical variable $$x \in [0, 1]$$ is mapped onto a rotation:
$$
|\psi(x)\rangle = RY(\theta = x \cdot \pi) \, |0\rangle
$$

This encoding translates data into **quantum amplitudes**, which are then manipulated and entangled in the circuit. The Bloch sphere helps visualize how patient data "moves" through quantum space and evolves.

### **Entanglement:**

Entanglement allows two or more qubits to share information in a non-classical way. For example, after applying a **CNOT gate** to two qubits, their states become correlated:

$$
|\psi\rangle = \frac{1}{\sqrt{2}} (|00\rangle + |11\rangle)
$$

In a VQC, entangling gates are used to model interactions between clinical features (like tumor stage and lymphovascular invasion), potentially capturing relationships that classical models could miss.

### **X Gate (Pauli-X):**
![pauli-x gate rotation](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.quera.com%2Fglossary%2Fpauli-x-gate&psig=AOvVaw3glFhZ36R7ej9lehYbj7QP&ust=1753546389811000&source=images&cd=vfe&opi=89978449&ved=0CBYQjRxqFwoTCOjOhr-z2I4DFQAAAAAdAAAAABAE)

The Pauli-X gate is the quantum analog of a classical NOT gate, flipping a qubit state:
$$
X|0\rangle = |1\rangle, \quad X|1\rangle = |0\rangle
$$

X gates are used within ansatz circuits to construct complex superpositions and to flip encoded medical data across axes of the Bloch sphere. This contributes to building expressive decision boundaries in the classification process.

### These concepts are directly applied in building, simulating, and training the quantum model.

## To apply these mathematical concepts and quantum techniques, I will use:

**Python:** for preprocessing and interfacing with quantum backends

**Qiskit:** to design quantum circuits, encode features using rotation gates, and simulate quantum measurements. 

**Qiskit Machine Learning:** to build and train a Variational Quantum Classifier

**Matplotlib & Qiskit Visualizations:** for rendering Bloch spheres, quantum circuits, and outcome comparisons

