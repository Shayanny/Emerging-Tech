# Emerging Technologies - Emerging Techonologies Assessment

**Author:** Shayanny  
**Institution:** Atlantic Technological University - Year 4  
**Module:** Emerging Technologies
**May 2026**

This repository contains my solutions to quantum computing problems using Qiskit, demonstrating fundamental quantum algorithms and their advantages over classical approaches.

## Overview

This assessment explores the Deutsch-Jozsa problem and related quantum algorithms, showcasing how quantum computers can solve certain problems exponentially faster than classical computers.

Through a series of progressive problems, this work builds from basic Boolean function generation to the full implementation of the Deutsch-Jozsa algorithm, illustrating the transition from classical to quantum approaches and the resulting computational advantages.

## Key Concepts Explored

**Query Complexity**  
The project analyzes how many queries (function evaluations) are required to determine properties of Boolean functions in both classical and quantum settings. Classical approaches require multiple queries that scale with input size, while quantum algorithms achieve constant query complexity.

**Quantum Oracles**  
Quantum oracles are unitary operations that encode classical Boolean functions into quantum circuits. This project implements oracles for single-input and multi-input functions, demonstrating the transformation |x⟩|y⟩ → |x⟩|y ⊕ f(x)⟩ where function evaluation occurs in quantum superposition.

**Phase Kickback**  
A crucial mechanism in quantum algorithms where the auxiliary qubit in the |−⟩ state causes the function value to be encoded as a phase on the input qubit rather than changing the auxiliary state. This enables the interference patterns that give quantum algorithms their advantage.

**Quantum Parallelism**  
By placing input qubits in superposition, quantum algorithms can effectively evaluate a function on multiple inputs simultaneously with a single oracle call. This principle underlies the exponential speedup demonstrated in the Deutsch-Jozsa algorithm.

## Technologies Used

- **Python 3.9+** - Programming language
- **Qiskit 1.0+** - IBM's open-source quantum computing framework
- **Qiskit Aer** - High-performance quantum circuit simulator
- **Jupyter Notebook** - Interactive development and documentation environment
- **Matplotlib** - Visualization of quantum circuits and measurement results
- **NumPy** - Numerical computation support