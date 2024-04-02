# QMLHEP-GSoC-24-Tasks
Task I: Quantum Computing Part (Script: Task_1.ipynb)
  1) Implement a simple quantum operation with Cirq or Pennylane
  2) Implement a second circuit with a framework of your choice

Task III: Comment on Quantum Computing

Before Quantum Computing, I’d talk a bit about classical computing and then extend the same to quantum, then I’ll cover certain Quantum Protocols and Algorithms, including Superdense Coding, Quantum Teleportation and Shor’s Algorithm. Then, I will delve into Quantum Machine Learning and Quantum Neural Networks
Classical computers store information in the form of bits (smallest unit of data a Classical Computer can process), which can exist in two states and various classical gates are used to manipulate these bits to construct algorithms and process information.

On the other hand, in Quantum Computers, information is stored in the form of Qubits, which are essentially two-state quantum mechanical systems. These two state systems are selected such that they follow the quantum principles, for instance superposition and entanglement, leading to quantum properties being induced in the qubits as well. Examples of such systems include electron spin (up and down), and polarization of a single photon. 
Qubit States can be pure or mixed. A pure qubit is a coherent superposition of the basis states, which are usually |0> and |1>, which means that a single qubit can be represented via a linear combination of the base states. Coherent superposition only occurs when there is a lack of noise, but in the real world, various forms of interactions with the qubits cause quantum noise to be induced, making them decoherent. This makes it possible to put these quantum states in mixed states, which is an incoherent mixture of various pure states.

Quantum Gates: Quantum Gate is the most basic quantum circuit operating on one or a small number of qubits and are analogous to classical gates. These Quantum Gates are always reversible and are represented via a unitary matrix.

Measurements: Measurement is an irreversible operation which helps us gain information about the qubit it is acted upon. The qubit collapses into one of its base states (in case of non-entangled states) or a state of its other entangled qubits (in case of entangled state). This eliminates coherence.

Quantum Machine Learning: 
The integration and implementation of quantum algorithms in Machine Learning is called Quantum Machine Learning. First, the classical data is encoded into the quantum computer via various methods to make it accessible for quantum information processing. Subsequently, quantum information processing routines are applied and the result of the quantum computation is read out by measuring the quantum system.
One of the Quantum Machine Learning Methods includes the Graph Quantum Neural Networks. Here, the input is represented via a density matrix, and each of the node of the graph represents a quantum state. The edges of the graph is given by the similarity between the two nodes, that is the two quantum states. This can be given by various functions or operators like the dot product between the two states. An unsupervised graph loss function and supervised loss function is then defined using quantum operators and they are linearly combined to give the final loss function. 
Then, similar to a classical neural network, the architecture of a quantum neural network is set up wherein each transformation is given by a product of various matrices and each node of the layer is given by this product. Message Passing, and backpropagation on the basis of the loss function then happens, which trains the quantum graph neural network. 

Suggest methods you think are good and you would like to work on:
While researching about Quantum Machine Learning and reading about various methods, I found Quantum Graph Neural Networks to be extremely fun. I've also described the working of the same in the previous section. I read about various methods like Invariant and Equivariant Graph Neural Networks, Quantum Graph Residual Neural Network, QG Convolutional Neural Networks and Quantum Neural Networks based on the Ego-Graph Learning Approach and Quantum Diffusion Convolution Kernel based GNN. 
It seems really useful and efficent to use graph objects for the purposes of learning, as it accuractely represents the correlations between various nodes, which can't be accurately captures in other architectures. This can be really helpful for making predictions on molecules, social networks, particle jet data and various other datasets which have an inherent correlation between the datapoints.
