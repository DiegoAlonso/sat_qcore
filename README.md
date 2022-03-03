# Generation of Qiskit code for solving SAT problems
This repository contains metamodels, model transformations and some example models of the generation of quantum circuits for [IBM's Qiskit SDK](https://qiskit.org/) for solving SAT problems. These tools run on the [Eclipse IDE] (https://eclipse.org) and require the [Epsilon](https://www.eclipse.org/epsilon/) family of meta-modelling languages. The set of tools available on this repository implement the following MDE scheme:

![MDE scheme, from SAT to Qiskit code](/../main/assets/mde_scheme.png)

The structure of the repository is the following one:

- Folder *cnfQcore* contains the developed metamodels and model transformations
- Folder *tests* contains some example models of SAT equation in CNF, the generated quantum circuit implementing Grover's algorithm, and the generated Qiskit code, each in a separate sub-folder.

In order to execute the examples, you first need the Eclipse editor and the Epsilon plug-in, and then follow the instructions on the Epsilon webpage on how to install the provided metamodels and how to configure the execution of each model transformation through the "Run as" menu option in Eclipse.

As an example of the application of this toolchain, for the SAT equation  (x1 ∨ x2 ) ∧ (¬x1 ∨ x3 ) ∧ (¬x2 ∨ x3 ), we generate the following Qiskit circuit:

![Qiskit circuit](/../main/assets/sat3_circuit.png)

which simulation on IBM's Quantum facilities generate the following histogram of possible solutions, when run 1024 times:

![Histogram of possible solutions](/../main/assets/sat3_solutions.png)


