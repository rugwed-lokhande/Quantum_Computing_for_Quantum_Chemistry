# Seniority‐Restricted CC on Quantum Hardware

This repository contains our implementation of a seniority‐restricted coupled‑cluster (sr‑CC) ansatz 
for use in Variational Quantum Eigensolver (VQE) workflows.  

## Features
- Fermion→qubit mapping via OpenFermion  
- Trotterized circuit generators  
- Built‑in benchmarking against UCCSD  

## Getting Started
```bash
git clone https://github.com/yourusername/my-srCC-quantum.git
cd my-srCC-quantum
pip install -r requirements.txt

#requirements
🧠 Classical Electronic Structure Packages
You need these to get integrals (Hamiltonian parameters) as input for UCCSD:
PySCF – lightweight Python library for HF, DFT, CCSD, integrals (most common choice).
Psi4 – open-source package for ab initio methods, supports integral generation and CC references.
Gaussian / GAMESS – traditional quantum chemistry codes (but not as easy to interface programmatically).
🔗 Fermion-to-Qubit Mapping & Ansatz Construction
These packages handle Jordan–Wigner / Bravyi–Kitaev transforms and build UCCSD circuits:
OpenFermion – Google’s library for fermionic Hamiltonians, mappings, and UCCSD operator generation.
Qiskit Nature – IBM’s package for chemistry on quantum computers, includes UCCSD ansatz, qubit mapping, tapering.
PennyLane-QChem – from Xanadu, integrates electronic structure with variational circuits.
Tequila – Python library focused on chemistry VQE, very customizable for UCC variants.
⚛️ Quantum Circuit Simulation & Execution
For actually simulating or running circuits:
Qiskit – quantum circuit construction, transpilation, simulators, and IBM Quantum backend execution.
Cirq – Google’s quantum circuit library, integrates well with OpenFermion.
PennyLane – great for hybrid classical–quantum optimization loops and autodiff.
Braket SDK – AWS framework for running on multiple quantum hardware backends.
QuTiP – for exact statevector or density-matrix simulation (good for validation).