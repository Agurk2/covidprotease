[Presentation](https://docs.google.com/presentation/d/1nQ6jEULpBLEJL_xdE9jlFi61gCe786L6GbkFQqGCZh0/edit?usp=sharing)
# Solving binding energies for the ground state protease in SARS-Cov-2
Computes the ground state binding energies of glutamine in order to facilitate speedups in the development of novel Covid-19 vaccines. This project has been developed during the iQuHack 2022 hackathon. This project caters toward the quantum for good and QuTech category.

Developed by: Oliver, Jay, Agni, Mustafa, Vardaan

Inspiration from the [IBM Africa Challenge 2021](https://github.com/qiskit-community/ibm-quantum-challenge-africa-2021)

## A protease-what-now?

A protease is an enzyme that works as a 'hammer', breaking down proteins into smaller amino acids and polypeptides. These amino acids and polypeptides then form long chains, allowing the virus to spread within its host.

Covid-19 contains a protease called glutamine (see image).

![imgsrv fcgi](https://user-images.githubusercontent.com/78431611/151695110-292973a7-323c-4388-aeaa-1ee40cb041fe.png)

*National Center for Biotechnology Information. "PubChem Compound Summary for CID 5961, Glutamine" PubChem, https://pubchem.ncbi.nlm.nih.gov/compound/Glutamine. Accessed 30 January, 2022.*

By blocking the protease's receptors, we effectively halt the virus' ability to spread within its host. This can be done by reacting a protease inhibitor with the protease in order to stop the chemical process from occurring.

This [video](https://www.youtube.com/watch?v=WBYOfqlC8hQ) explains it well.

## Problem definition

Current quantum hardware is not powerful enough to simulate whole macromolecules. However, as quantum computers get more and more powerful, so too will the ability to simulate molecular interactions. For this project, we simplified the glutamine molecule to create a so-called toy protease, in order to prove the effectiveness of quantum computer.

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

## Results

While we encountered some problems with simulating on QI's backend, we found that carbon binds with the nitrogen in the azanide molecule at -89.8 Hartrees (-3.19 x 10¹⁶ joules). 

<img width="401" alt="Screenshot 2022-01-30 at 13 12 42" src="https://user-images.githubusercontent.com/78431611/151699135-a6aa5433-7428-4715-a553-7bf01a1f7979.png">

While we only bounded a single carbon atom to the glutamince molecule, it demonstrates the ability of quantum computational chemistry in current chemical problems. As long as SARS-Cov-2 remains in the world, it will mutate and become resistent to current vaccines. By demonstrating these results using VQE, we effectively achieve speedups in the development of novel vaccines to combat the novel mutations.

While we used VQE, QAOA could also be used, perhaps even preferred.

## Our experience with iQuHack

### Oliver
"As a high school student, this experience has been eye-opening. Being able to work closely with undergrads and masters from all over the world, has given me greater insight into the world of quantum. It has shown me that I'm not alone in learning quantum -- that there are peopple out there just like me. I finally felt as though I was surrounded by people who understood and valued what I said (, as opposed to forcing my parents to listen). They filled me with optimism and believed in me. I now know that I am preparing myself for a bright and exciting future. For that, I am thankful."

### Jay
"Not many times I've got the chance to work with people who are as passionate about Quantum as this team. Being my first Quantum hackathon, iQuHACK2022 has changed my perspective about approaching problems outside the comfort zone, As to say Quantum Chemistry or Biology isn't my strong area but this team filled me with enthusiasm and enabled me to me tackle this challenge. The experience was like forming new bonds by breaking some chemical ones!! I'm thankful to my team and the whole iQuHACK2022 team for this fun event!!"

### Agni
"I enjoyed working with teamates from around the globe on this endeavor. The workshops, guest speakers ang guidance was great, I especially loved working and assiting on a new innovative project learning new things I didnt know previously about using quantum and chemistry etc."

### Mustafa
"iQuHACK was a brilliant opportunity for me to get started with applications of quantum computing in chemistry. I've discovered how quantum optimization can help us develop new drugs by computing bonding energies. I'm looking forward to further learning in the field of quantum computing and building more applications of what I've learned."

### Vardaan
'iQuHACK-2022 is the coolest hackathon till date'. I feel this statement pretty much sums up my experience. Every hackathon has challenging problems, but what makes this one special, is the overall fun experience. From Dungeon Escape to Scavenger Hunt, and not to forget the chance to use a real quantum computer and interact with the various industry sponsors on Gathertown... it was definitely a one of kind experience for me :)

## Technologies
- QBraid
- QuantumInsprire, QuTech
- Jupter Notebook

## Software/Packages
- Qiskit
- Quantum Inspire
- getPass
- Numpy
- Matplotlib

## Team Statement
We wanted to thank iQuHack2022 and its sponsors for organizing such a wonderful event. We enjoyed the guest speakers, workshops, guidance and much more.
