# Emerging Technologies - Emerging Technologies Assessment

**Author:** Shayanny  
**Institution:** Atlantic Technological University - Year 4  
**Module:** Emerging Technologies
**May 2026**

This repository contains my solutions to quantum computing problems using Qiskit, demonstrating fundamental quantum algorithms and their advantages over classical approaches. All work is my own except where explicitly referenced.

## Repository Contents

- `problems.ipynb` - Main assessment notebook with 5 problems covering Deutsch-Jozsa algorithm
- `requirements.txt` - Python dependencies for the project
- `README.md` - This file
- `.gitignore` - Git ignore rules for Python projects

## Usage

Open the notebook in Jupyter:

```bash
jupyter notebook problems.ipynb
```

The notebook contains 5 problems:
1. Generating random Boolean functions (constant and balanced)
2. Classical testing strategies and query complexity analysis
3. Quantum oracle construction for single-input functions
4. Deutsch's Algorithm implementation and testing
5. Deutsch-Jozsa Algorithm scaling to n-bit inputs

**Before viewing**: All cells should be executed in order. If outputs are missing, select "Kernel" → "Restart & Run All" in Jupyter.

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
- Nielsen, M. A., & Chuang, I. L. (2010). "Quantum Computation and Quantum Information." 
  Cambridge University Press. Chapter 1.4.4 discusses the Deutsch-Jozsa algorithm as a 
  foundational example of quantum computational advantage.


## AI Tool Usage

Throughout this project, I used Claude (Anthropic) as a research and learning assistant to help:
- Understand complex quantum concepts like phase kickback
- Debug code issues and understand error messages
- Improve explanations and documentation clarity
- Structure my thinking about the promise problem

All code implementations, problem-solving approaches, and analysis are my own work. The AI served as a tutor to help me understand concepts, not to generate solutions. All information provided by AI was verified against official sources (IBM Quantum Learning, academic papers)

## License

This project is submitted as part of academic coursework for Atlantic Technological University. Please do not copy or reuse for academic submissions.