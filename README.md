<p align="center">
<img src="figures/Q&ML.png" alt="Q&ML Logo" width="600">
</p>

<h2><p align="center">A PyThon Library for Quantum Computation and Machine Learning</p></h2>
<h3><p align="center">Updated, Scalable, Easy Implement, Easy Reading and Comprehension</p></h3>


<p align="center">
    <a href="https://github.com/QUANTUM-AND-ML/QAOA-ML-Detection-PLA/blob/main/LICENSE">
        <img alt="MIT License" src="https://img.shields.io/github/license/QUANTUM-AND-ML/QAOA-ML-Detection">
    </a>
   <a href="https://github.com/QUANTUM-AND-ML/QAOA-ML-Detection-PLA/activity">
        <img alt="Activity" src="https://img.shields.io/github/last-commit/QUANTUM-AND-ML/QAOA-ML-Detection-PLA?color=%23f38b51">
    </a>
       <a href="https://www.nsfc.gov.cn/english/site_1/index.html">
        <img alt="Fund" src="https://img.shields.io/badge/supported%20by-NSFC-green">
    </a>
    <a href="https://twitter.com/FindOne0258">
        <img alt="twitter" src="https://img.shields.io/badge/twitter-chat-2eb67d.svg?logo=twitter">
    </a>


</p>
<br />



## Quantum & Machine Learning
Relevant data for the paper entitled "Rapidly Trainable and Shallow-Compiled Quantum Approximate Optimization Algorithm for Maximum Likelihood Detection"

## Table of contents
* [**Main work**](#Main-work)
* [**Our contributions**](#Our-contributions)
* [**Results display**](#Results-display)
* [**Citation**](#Citation)

## Main work
In multiple-input and multiple-output (MIMO) systems, the maximum likelihood (ML) detection problem is NP-hard and becomes increasingly complex with more transmitting antennas and symbols. The quantum approximate optimization algorithm (QAOA), a leading candidate algorithm running in the noisy intermediate-scale quantum (NISQ) devices, can show quantum advantage for approximately solving combinatorial optimization problems. In this paper, we propose an improved QAOA based maximum likelihood detection. In the proposed scheme, we use ZX-calculus to prove the parameter symmetry in QAOA circuits, which can be used to reduce the search space and accelerate the training process. Moreover, to run QAOA on quantum devices, an improved qubit mapping method with simultaneous gate absorption is proposed, which can compile the quantum circuit of the QAOA to satisfy the connectivity constraints of real quantum devices with fewer CNOT counts. In numerical experiments, our scheme accelerates parameter training by an average of 29.8% and uses fewer CNOT gates and shallower circuit depth during compilation. This demonstrates that our scheme has significant advantages over the traditional scheme.
<p align="center">
<img src="figures/workflow.png" alt="Figure 1" width="500">
</p>

**Figure 1.** The workflow of the improved QAOA based ML detection.

## Our contributions
* Use ZX-calculus to demonstrate that the parameters in the quantum approximate optimization algorithm exhibit symmetry under specific conditions and utilize this symmetry to accelerate parameter training.
* Propose a circuit optimization enhanced qubit mapping method to reduce the number of CNOT gates during circuit compilation.
* Numerical simulations showcase the advantages of the proposed scheme, including accelerated parameter training and reduced CNOT gates and circuit depth during the compilation process.

## Results display

<p align="center">
<img src="figures/figure1.png" alt="Figure 2" width="600">
</p>

**Figure 2.** The decoding result obtained by $N_{t} = 5$, $p = 6$ improved QAOA in the noisy circuit.

<p align="center">
<img src="figures/figure2.png" alt="Figure 3" width="600">
</p>

**Figure 3.** Average convergence curve of the cost function under random channel matrices in the noisy circuit.

<p align="center">
<img src="figures/figure3.png" alt="Figure 4" width="600">
</p>

**Figure 4.** The maximum probability obtained by $N_{t} = 8$ and $N_{t}=10$ in each of the 12 simulations.

<p align="center">
<img src="figures/figure4.png" alt="Figure 5" width="600">
</p>

**Figure 5.** The quantum circuit after the OLSQ-GA compilation.

<p align="center">
<img src="figures/figure5.png" alt="Figure 6" width="600">
</p>

**Figure 6.** The process of quantum circuit optimization.


## Citation
```
- 3.9 >= Python >= 3.7 (Python 3.10 may have the `concurrent` package issue for Qiskit)
- Qiskit >= 0.36.1
- Qiskit-aer >= 0.12.0
- The calculation may require the large amount of RAM
```
