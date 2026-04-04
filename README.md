# Emerging Technologies - Emerging Technologies Assessment

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

- **[Python 3.9+](https://www.python.org/)** - Programming language
- **[Qiskit 1.0+](https://qiskit.org/)** - IBM's open-source quantum computing framework
  - [Qiskit Documentation](https://docs.quantum.ibm.com/)
- **[Qiskit Aer](https://qiskit.github.io/qiskit-aer/)** - High-performance quantum circuit simulator
- **[Jupyter Notebook](https://jupyter.org/)** - Interactive development and documentation environment
- **[Matplotlib](https://matplotlib.org/)** - Visualization of quantum circuits and measurement results
- **[NumPy](https://numpy.org/)** - Numerical computation support

## Installation

To run this project locally:
```bash
# Clone the repository
git clone https://github.com/Shayanny/Emerging-Tech.git
cd Emerging-Tech

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook problems.ipynb
```

## References

### Educational Resources
- [IBM Quantum Learning - Deutsch-Jozsa Algorithm](https://learning.quantum.ibm.com/course/fundamentals-of-quantum-algorithms/quantum-query-algorithms#the-deutsch-jozsa-algorithm)
- [IBM Quantum Learning - Phase Kickback](https://learning.quantum.ibm.com/course/fundamentals-of-quantum-algorithms/phase-kickback-and-eigenvalues)

### Academic Literature
- Montanaro, A. (2016). "Quantum algorithms: an overview." *npj Quantum Information*, 2(1), 15023. [DOI](https://doi.org/10.1038/npjqi.2015.23)
- Deutsch, D., & Jozsa, R. (1992). "Rapid solution of problems by quantum computation." *Proceedings of the Royal Society A*, 439(1907), 553-558.

## License

This project is submitted as part of academic coursework for Atlantic Technological University.