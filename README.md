This repository contains an example illustration of the framework developed in the paper: Toscano-Duran,V., Gonzalez-Diaz,R., and Gutiérrez-Naranjo, M.A., "Barycentric Neural Networks and Length-Weighted Persistent Entropy Loss: A Geometric and Topological Framework for Function Approximation". (Submitted to DGMM 2027)

## Usage

To run the Jupyter notebooks correctly, you need to create a Python virtual environment (This has been developed with Python3.9.13):

```bash
virtualenv -p python env
```

Next, activate the virtual environment (we use the source command because we are working in WSL):

```bash
env\Scripts\activate
```

Finally, install the required libraries:

```bash
pip install numpy pandas matplotlib tqdm gudhi tensorflow
```

If Jupyter Notebook cannot find a kernel, you may need to install ipykernel. Run the following command to resolve this issue:

```bash
pip install ipykernel
```

## Repository structure

- `utilsBaricentricNeuralNetwork.py`: It contains the implementation of the proposed Barycentric Neural Network (BNN) in TensorFlow framework.

- `utilsTopology.py`: It provides the topological tools necessary for the experiments.

- `utils.py`: It contains some necessary functions used in the experiments.

- `RepresentCPLF_BNN.ipynb`: It includes experiments on representing certain continuous piecewise linear functions (CPLFs) using the proposed barycentric neural network.

- `ApproximatingFunctionsUsingBNN_ComparisonMSEandLWPE.ipynb`: This contains experiments aimed at optimising the base points used to construct the barycentric neural network that approximates continuous functions in the TensorFlow framework using the LWPE loss function. It also compares the proposed persistent entropy-based loss function (LWPE) with the mean squared error (MSE) loss function.


## Citation and Reference

If you want to use our code for your experiments, please cite our paper.

For further information, please contact us at: vtoscano@us.es
