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
OpenFermion – Google’s library for fermionic Hamiltonians, mappings, and UCCSD operator generation.
Qiskit Nature – IBM’s package for chemistry on quantum computers, includes UCCSD ansatz, qubit mapping, tapering.
PennyLane-QChem – from Xanadu, integrates electronic structure with variational circuits.
Tequila – Python library focused on chemistry VQE, very customizable for UCC variants.