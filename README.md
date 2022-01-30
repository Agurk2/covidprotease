# Solving binding energies for the ground state protease in SARS-Cov-2
Computes the ground state binding energies of glutamine in order to facilitate speedups in the development of novel Covid-19 vaccines. This project has been developed during the iQuHack 2022 hackathon. This project caters toward the quantum for good and QuTech category.

Developed by: Oliver N, include your names as well

## A protease-what-now?

A protease is an enzyme that works as a 'hammer', breaking down proteins into smaller amino acids and polypeptides. These amino acids and polypeptides then form long chains, allowing the virus to spread within its host.

Covid-19 contains a protease called glutamine (see image).

![imgsrv fcgi](https://user-images.githubusercontent.com/78431611/151695110-292973a7-323c-4388-aeaa-1ee40cb041fe.png)

*National Center for Biotechnology Information. "PubChem Compound Summary for CID 5961, Glutamine" PubChem, https://pubchem.ncbi.nlm.nih.gov/compound/Glutamine. Accessed 30 January, 2022.*

By blocking the protease's receptors, we effectively halt the virus' ability to spread within its host. This can be done by reacting a protease inhibitor with the protease in order to stop the chemical process from occuring.

## Problem definition

Current quantum hardware is not powerful enough to simulate whole macromolecules. However, as quantum computer's get more and more powerful, so too will the ability to simulate molecular interactions. For this project, we simplified the glutamine molecule to create a so-called toy protease, in order to prove the effectiveness of quantum computer.

The glutamine molecule is simplified to methanamine

![imgsrv-1 fcgi](https://user-images.githubusercontent.com/78431611/151696812-1dba07fd-bac0-4957-9196-ea9fd54ca044.png)

*National Center for Biotechnology Information. "PubChem Compound Summary for CID 450541, (111C)methanamine" PubChem, https://pubchem.ncbi.nlm.nih.gov/compound/111C_methanamine. Accessed 30 January, 2022.*

By computing the bonding energy for the ground state toy protease, we can develop more sophisticated inhibitors that may be more effective against Covid variants

## How to run

Install the following packages:
```
pip install qiskit
```
```
pip install quantuminspire
```
```
pip install qiskit_nature
```
```
pip install PySCF
```
Next, launch the Jupyter Notebook and run the code. Note that a [QuantumInspire account](https://www.quantum-inspire.com/account/create/) is required

## Technologies
- QBraid
- QuantumInsprire, QuTech
- Jupter Notebook

## Software/Packages
- Qisket
- Quantum Inspire
- getPass
- Numpy
- Matplotlib
