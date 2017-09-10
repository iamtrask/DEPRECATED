# Helium : YASHE Tensor Demo

<b>Background:</b> One of the most valuable contributions of the PySyft library to the Cryptography and AI communities is our Tensor level abstractions of Homomorphic Encryption algorithms. This allows users with no knowledge of Encryption to perform Encrypted Linear Algebra using a wide variety of encryption techniques. In this (and similar) tickets, we want to extend this ability to new Homomorphic Encryption schemes, such that users with no knowledge of Encryption can empirically try out various backend encryption techniques for their front end use cases with minimal effort. As such, while the backend API will differ from Tensor to Tensor, we want the front-end Linear Algebra interface to be as similar as possible, and to give intuitive explanations if the API differs such that calling functions in an Encrypted Tensor that doesn't support those operations explains WHY that specific type of Encryption cannot support the operation (i.e., Paillier can't multiply two encrypted numbers together... perhaps you should try another backend Encryption scheme).

### Part 1: User Stories

* <b>User Story A:</b> As a <b>Linear Algebra</b> user, but NOT a Cryptography expert, I want the ability to perform linear algebra on Homomorphically Encrypted data using the YASHE Homomorphic Encryption technique. If operations are unsupported as a result of the limitations of YASHE, I want Error messages to explain so and recommend alternate options. Furthermore, if operations must be approximated using operations such as Taylor Series (or other Polynomial Approximations), I want the option to turn these approximations on or off, with the default functionality to be ON. If I perform an operation for which approximation is necessary (non-linear), and have the "allow_approximations" feature turned off, it should return an error.

* <b>User Story B:</b> As a <b>Linear Algebra</b> user, but NOT a Cryptography expert who has implemented an algorithm in one of PySyft's other Encrypted Tensor libraries, I want the ability to simply change out the tensor type and be able to run all the same operations in this tensor library, with good error messages explaining why functions may not be supported (when relevant).

### Part 2: Mockup

[This Notebook](https://github.com/OpenMined/PySyft/blob/master/notebooks/Syft%20-%20Paillier%20Homomorphic%20Encryption%20Example.ipynb) is an excellent mockup of the functionality that we want to see with this new encrypted tensor class. It should be able to do all the operations in this notebook, with the added functionality of multiplication between two encrypted tensors (since that is explicitly supported by YASHE).

### Part 3: Acceptance Criteria

[PySyft: Epic - YASHE Tensor Demo](https://github.com/OpenMined/PySyft/issues/227)
