---
layout: page
author: Gianfranco Abrusci
mathjax: true
---
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>


In this session we will introduce the ingredients we need to performa a molecular dynamics simulation.
It is a mesh up of information you can find scattered on different sources. [^1]

[^1]: This tutorial is inspired by
1.  [Using VMD](https://www.ks.uiuc.edu/Training/Tutorials/vmd/vmd-tutorial.pdf)

### Overview
Let's recap the so called **MD machinery**.

<IMG class="displayed" src="../../img/tut1/md_machinery.png" alt="">


## Amagabula magicabula bibidi-bobidi-bu
The idea is to solve the Newton's equations of motion for all the atoms in the
system. For each atom in 1D we can write:

$$m\frac{d^2 x}{dt^2} = -\nabla U$$

We need then to know what the potential $$U$$ is. The set of functions and parameters
that composes the $$U$$ is called **Force Field** (**ff** from now on).

The idea behind **ffs** is to mimic the experimental behaviour of proteins with a
potential for atoms that has a
feasible computational cost.
There are several force field available:
- CHARMm, AMBER for all-atom simulations;
- Martini for coarse grained simulations.

Each ff has its own functional form and its protocol to define parameters. The parameters, in fact, hide under the hood assumptions that make the functional formation viable for simulations. Using CHARMm parameters with an AMBER potential
definition will lead you to unreliable results.

<p class="prompt prompt-attention">Do not mix parameters from different force
fields!<p>

Moreover, ff parameters evolve as more data and simulations are gathered.

<p class="prompt prompt-attention">Check for the latest version of force fields!</p>
We will mainly use CHARMm ff (version 36)


## PDB PSF

Newton's equation:

Force field

What is a pdb

what is a psf

top/par

bonds (covalent) disu/h-bonds

# alalnine with not CHARMM36.
- creazione dialanina (sia modding pdb che usando ALA + N-C-term)



# fors
creazione del pdb together - lizo/ubi

da soli : bpti