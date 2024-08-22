# Deutsch-Jozsa Algorithm Implementations in Cirq and Qiskit

## Overview

This project contains two implementations of the Deutsch-Jozsa algorithm, one in [Cirq](https://quantumai.google/cirq) and the other in [Qiskit](https://qiskit.org/). The Deutsch-Jozsa algorithm is a quantum algorithm that efficiently determines whether a given oracle (a black-box function) is balanced or constant. A balanced function returns 0 for half of the inputs and 1 for the other half, while a constant function returns the same value (either 0 or 1) for all inputs.

### Game Concept: "The Oracle's Secret"

To make learning more interactive, the implementations are wrapped in a simple game called "The Oracle's Secret". The player is asked to guess whether the oracle is balanced or constant. The quantum algorithm then runs, and the result is compared with the player's guess, showing whether the quantum algorithm outperformed the player's intuition.

## Implementations

### Qiskit Implementation

The Qiskit implementation of the Deutsch-Jozsa algorithm demonstrates the power of quantum computing to solve specific problems more efficiently than classical computing. Here's a brief overview of how it works:

- **Superposition**: The input qubits are put into an equal superposition of all possible states using Hadamard gates.
- **Oracle Application**: The oracle, which is either balanced or constant, applies its transformation to the qubits.
- **Interference and Measurement**: Another round of Hadamard gates is applied to the input qubits, followed by measurement. The result reveals the nature of the oracle.
- **Game Aspect**: The player guesses whether the oracle is balanced or constant. The quantum algorithm's result is then compared to the player's guess.

**Key Files:**
- `Deutsch-jozsa.ipynb`: Contains the Qiskit implementation of the Deutsch-Jozsa algorithm and the interactive game.

### Cirq Implementation

The Cirq implementation of the Deutsch-Jozsa algorithm follows a similar process:

- **Superposition**: Hadamard gates create a superposition of all possible input states.
- **Oracle Application**: The oracle modifies the qubits based on whether it is balanced or constant.
- **Interference and Measurement**: The final Hadamard gates and subsequent measurement reveal the nature of the oracle.
- **Game Aspect**: The player interacts with the game by making a guess, and the quantum algorithm checks the accuracy of that guess.

**Key Files:**
- `Deutsch-jozsa.ipynb`: Contains the Cirq implementation of the Deutsch-Jozsa algorithm and the interactive game.


## Visualization

Both implementations display the quantum circuit at key stages (initialization, after oracle application, and before measurement) to help you visualize how the algorithm manipulates the qubits. The final measurement results are also displayed in a histogram, showing the outcome of the quantum computation.

## Summary

This project serves as both a practical introduction to the Deutsch-Jozsa algorithm and a fun, interactive game that highlights the power of quantum computing.