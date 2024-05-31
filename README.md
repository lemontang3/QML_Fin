# QML_Fin

#Final QNN:

## Repository Overview

This repository contains code and resources for building and training a quantum machine learning model using Qiskit. The primary focus is on creating a quantum autoencoder for feature extraction and applying it to financial data, specifically the S&P 500 index.

## Repository Structure

- **Data Preparation:**
  - Download and preprocess S&P 500 data using the `yfinance` library.
  - Compute rolling averages and ratios for additional features.
  - Normalize and encode data for input into a quantum circuit.

- **Quantum Circuit Construction:**
  - Define parameterized quantum circuits for encoding data.
  - Implement a custom quantum autoencoder circuit.
  - Use Qiskit’s built-in feature maps for data encoding.

- **Training and Evaluation:**
  - Train the quantum machine learning model using the COBYLA optimizer.
  - Evaluate the model's performance using a confusion matrix.

## Key Functions and Classes

- `ansatz(num_qubits, depth)`: Creates a parameterized ansatz circuit with specified depth.
- `auto_encoder_circuit(num_latent, num_trash, depth)`: Constructs a quantum autoencoder circuit.
- `parametrized_gates(params)`: Defines parameterized gates for the quantum network.
- `fit(train_predictors, train_labels)`: Trains the quantum machine learning model.
- `confusion_matrix(train_labels, classifier.predict(train_predictors))`: Computes the confusion matrix for mo
