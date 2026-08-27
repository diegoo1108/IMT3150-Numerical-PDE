# Simplified Keller-Segel Model: Analysis and Study of Turing Patterns

This repository contains the numerical implementation, continuous/discrete theoretical analysis, and Turing pattern simulation scripts for the **simplified (minimal) Keller-Segel model** governing chemotaxis. 

The work forms part of the course **IMT3130: Applications of Partial Differential Equations and Functional Analysis in Engineering** at the **Pontificia Universidad Católica de Chile**.

## Authors
* Montserrat Jiménez
* Diego Pérez

---

## Background & Motivation

Bacterial communities frequently encounter unfavorable environments. Given their limited adaptive capacity, many microorganisms rely on migration toward more hospitable regions. The ability to sense chemical gradients and move in response to them is known as **chemotaxis**.

First documented by Engelmann and Pfeffer in the 1880s, the quantitative mathematical study of chemotaxis began in earnest during the 1960s. Beyond bacterial aggregation, chemotactic mechanisms play key roles in slime mold dynamics, tumor growth, and embryonic blood vessel formation (angiogenesis).

Introduced in 1971, the **Keller-Segel model** provides a classical continuum framework for chemotaxis. Due to the nonlinear coupling between cell motion and chemical signaling, traditional analytical tools often prove insufficient. Under specific initial conditions, the competition between chemical attraction (which concentrates cells) and diffusion (which acts to disperse them) can trigger instabilities, causing the system to evolve into spatial structures known as **Turing patterns**.

---

## Project Objectives

1. **Model Derivation & Simplification:** Derive the coupled Keller-Segel system from first principles and justify natural simplifications that yield the minimal parabolic-elliptic formulation.
2. **Well-Posedness Analysis:** Discuss the continuous framework and establish initial conditions ensuring the well-posedness of the minimal model.
3. **Discrete Formulations & FEM:** Analyze spatial discretization via the Finite Element Method (FEM) and temporal decoupling schemes, including existence, uniqueness, and convergence rate guarantees for the discrete system.
4. **Numerical Implementation:** Implement robust solvers in `dolfinx` (FEniCS ecosystem) to simulate characteristic phenomena (such as blow-up and concentration effects) associated with the minimal model.
5. **Turing Pattern Analysis:** Study stationary Turing instabilities in the presence of logistic growth, establishing existence criteria and simulating representative pattern topologies (e.g., spots, hexagons, and stripes).

---

## Repository Structure

```text
.
├── Patrones.py
├── error.py
├── soluciones_manufacturadas.py
├── solver.py
├── final_draft.pdf
├── Referencias/
│   ├── Adrien_Blanchet.pdf
│   ├── Elena_Floris.pdf
│   ├── Kolade_M_Owolabi.pdf
│   ├── NORIKAZU_SAITO.pdf
│   └── SUZUKI.pdf
└── README.md
