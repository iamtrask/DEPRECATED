# Homomorphic Encryption 101

The purpose of this text is not to give detailed accounts of [homomorphic encryption](https://en.wikipedia.org/wiki/Homomorphic_encryption) (HE), but rather to provide starting points for those curious about the inner working of these schemes. 

The big distinction between them is the supported operations:

- *Partially Homomorphic Encryption (PHE)* schemes only support certain operations, for instance only addition 

- *Somewhat Homomorphic Encryption (SHE)* schemes support both addition and multiplication yet can only do a bounded number of either

- *Fully Homomorphic Encryption (FHE)* schemes are like SHEs but without a bound on the number of operations

The latter two are the most recent inventions and still under active research. Note SHE and FHE schemes can in principle compute any function securely while PHEs are more limited.


## Suggested Reading for Getting Started

1) Wikipedia articles on [homomorphic encryption](https://en.wikipedia.org/wiki/Homomorphic_encryption) and [Paillier's scheme](https://en.wikipedia.org/wiki/Paillier_cryptosystem)

2) [Computing Arbitrary Functions of Encrypted Data](https://crypto.stanford.edu/craig/easy-fhe.pdf)

3) [A brief survey of Fully Homomorphic Encryption, computing on encrypted data](https://blog.quarkslab.com/a-brief-survey-of-fully-homomorphic-encryption-computing-on-encrypted-data.html)

4) [A Guide to Fully Homomorphic Encryption](https://www.dropbox.com/s/b7ir8o19llggbz7/A%20Guide%20to%20Fully%20Homomorphic%20Encryption.pdf?dl=0)


## Textbooks

### Cryptography

- [Introduction to Modern Cryptography](http://www.cs.umd.edu/~jkatz/imc.html): great rigorous introduction, covering e.g. Paillier but not the more recent lattice-based SHE/FHE schemes; self-contained with respect to required math although not main focus; lacks efficient algorithms

- [Cryptography Made Simple](http://www.springer.com/gp/book/9783319219356): another great introduction, including a brief exposition of lattice-based cryptography; likewise self-contained; giving more implementation hints

### Mathematics

Although cryptography books tend to be self-contained, to get a better grasp of them it's relevant to go deeper into the mathematics behind them, especially abstract algebra and number theory.

- [A Computational Introduction to Number Theory and Algebra](http://www.shoup.net/ntb/): excellent introduction making only a few prior assumptions; covers everything needed to understand the mathematics up to and including e.g. Paillier and secret sharing; gives efficient algorithms for many tasks

- [Modern Computer Algebra](www.cambridge.org/9781107039032): go-to reference for efficient algorithms, but not the easiest to start out with


## Surveys and Courses

- [A Decade of Lattice Cryptography](https://eprint.iacr.org/2015/939.pdf)

- video lectures on [Lattice-based Cryptography and Applications](http://cyber.biu.ac.il/event/the-2nd-biu-winter-school/)

- video lectures on [Cryptography in the Cloud – Verifiable Computation and Special Encryption](http://cyber.biu.ac.il/event/the-6th-biu-winter-school/)

- video lectures on [Advances in Practical Multiparty Computation](http://cyber.biu.ac.il/event/the-5th-biu-winter-school/)


## Papers

- [CryptoNets: Applying Neural Networks to Encrypted Data with High Throughput and Accuracy](https://www.microsoft.com/en-us/research/publication/cryptonets-applying-neural-networks-to-encrypted-data-with-high-throughput-and-accuracy/)


## Libraries

- [phe](https://github.com/n1analytics/python-paillier): Python implementation of Paillier's scheme (using GMP when available)

- [libpaillier](http://hms.isi.jhu.edu/acsc/libpaillier/): C implementation of Paillier's scheme using GMP

- [jspaillier](https://github.com/mhe/jspaillier): JavaScript implementation of Paillier's scheme

- [SEAL](https://sealcrypto.codeplex.com/): C++ implementation of the FV'12 FHE scheme; comes with several useful tools, including noise estimation

- [HElib](https://github.com/shaih/HElib): C++ implementation of the BGW'12 FHE scheme


## Blogs

- [Bristol Cryptography Group](http://bristolcrypto.blogspot.fr/)
