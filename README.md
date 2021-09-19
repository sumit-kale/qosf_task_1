# QOSF task 1 (bonus) 

### Cohort 4

**Problem Statement: Task 1 **


Design a quantum circuit that considers as input the following vector of integers numbers: 

[1,5,7,10]
returns a quantum state which is a superposition of indices of the target solution, obtaining in the output the indices of the inputs where two adjacent bits will always have different values. In this case the output should be: 1/\sqrt{2}  (|01> + |11>), as the correct indices are 1 and 3.

The file **Task 1 Final-General_Circuit.ipynb** solves the Problem statement 1

The file **Bonus_task_1.ipynb** contains solution for the bonus task.

**Solution to the task**
<p align="center">
  <img src="https://user-images.githubusercontent.com/35228896/133940258-cbb48309-75f5-493c-8b04-b4d85927096b.png" />
</p>



**Bonus:**
Design a general circuit that accepts vectors with random values of size 2n with m bits in length for each element and finds the state indicated above from an oracle.
 

**Generalized circuit**
<p align="center">
  <img src="https://user-images.githubusercontent.com/35228896/133939955-e428364e-8dd7-4e65-8728-dd06fafaffb1.png" />
  <em>Generalized circuit with relevent number of qubits required</em>
</p>

**Extreme limits of the circuit**


Since QASM allows to simulate at max 32 qubits, this restricts the value of  𝑛 < 7  (𝑛 is the number of addresses qubits) and  𝑚 < 8  (number of bits in the binary expansion of the number). At it's extreme i.e. 𝑛 = 6 and 𝑚 = 7. The remaining qubits are either used for the Oracle or ancillas required for the multi control troffoli gates.  


<p align="center">
  <img src="https://user-images.githubusercontent.com/35228896/133940661-d9c970ed-8c8b-4e6b-b030-ef14aa459062.png" />
  <em>Result for the largest problem</em>
</p>

