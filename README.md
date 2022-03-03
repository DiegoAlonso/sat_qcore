# Generation of Qiskit code for solving SAT problems
This repository contains metamodels, model transformations and some example models of the generation of quantum circuits for IBM Qiskit language for solving SAT problems. These tools run on the [Eclipse IDE] (https://eclipse.org) and require the [Epsilon](https://www.eclipse.org/epsilon/) family of meta-modelling languages. The structure of the repository is the following one:

- Folder *cnfQcore* contains the developed metamodels and model transformations
- Folder *tests* contains some example models of SAT equation in CNF, the generated quantum circuit implementing Grover's algorithm, and the generated Qiskit code, each in a separate sub-folder.

In order to execute the examples, you first need the Eclipse editor and the Epsilon plug-in, and then follow the instructions on the Epsilon webpage on how to install the provided metamodels and how to configure the execution of each model transformation through the "Run as" menu option in Eclipse.
