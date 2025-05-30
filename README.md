# Demo Zk-Snarks Quantum 🌪️

⚠️**This is just research level**

Demo project for P2P Coinjoin using ZK-Snarks to post quantum world

### P2P CoinJoin using zk-SNARKs with McEliece in a Post-Quantum World

The **McEliece cryptosystem**, one of the oldest post-quantum cryptographic schemes, is based on error-correcting codes and is resistant to attacks from quantum computers. Incorporating **McEliece** into **P2P CoinJoin** transactions, along with **zk-SNARKs**, provides a quantum-resistant framework that enhances both privacy and security in decentralized financial systems like Bitcoin.

#### McEliece Overview

The McEliece cryptosystem relies on **Goppa codes**, which are difficult for quantum computers to break due to the hardness of decoding randomly generated linear codes. Its structure makes it highly resistant to quantum attacks, though it requires relatively large public keys, making integration a unique challenge for blockchain applications.

#### Integrating McEliece into CoinJoin

In a post-quantum scenario, McEliece could replace **Elliptic Curve Digital Signature Algorithm (ECDSA)**, providing a quantum-safe signature method. Here’s how McEliece and zk-SNARKs could integrate with P2P CoinJoin:

1. **Quantum-Safe Transaction Signing**:
   - In traditional Bitcoin transactions, users sign inputs with ECDSA. In a McEliece-based CoinJoin, participants would use McEliece's quantum-resistant signatures to sign their transaction inputs.
   - These signatures would be secure against quantum computing attacks, ensuring the long-term integrity of transactions.

2. **zk-SNARKs for Privacy**:
   - **zk-SNARKs** would maintain the privacy of participants in a CoinJoin transaction by proving the validity of their inputs without revealing details.
   - Combining zk-SNARKs with McEliece means the transaction remains private while ensuring the underlying cryptography is quantum-resistant.

3. **P2P Decentralized CoinJoin**:
   - Participants would join together in a decentralized manner to form a joint transaction. The use of McEliece signatures ensures that no one can manipulate the transaction, while zk-SNARKs maintain privacy among participants.
   - In this setup, each participant submits quantum-safe proofs that their inputs are valid, and the final transaction is signed with McEliece keys.

#### Benefits of Using McEliece with zk-SNARKs in CoinJoin

- **Quantum-Resistant Security**: McEliece is one of the strongest candidates for resisting quantum attacks, securing the CoinJoin transaction even in a post-quantum world.
  
- **Enhanced Privacy with zk-SNARKs**: zk-SNARKs enable participants to obscure transaction details without compromising security, ensuring that the source of funds remains hidden from external observers.

- **Decentralization**: McEliece combined with zk-SNARKs supports fully decentralized CoinJoin operations, where no central coordinator is required, preserving both privacy and security.

#### Challenges

- **Large Key Sizes**: McEliece public keys are significantly larger than those used in classical cryptosystems, which could increase storage and transmission overhead in blockchain systems.
  
- **Performance**: While zk-SNARKs are efficient in terms of proof size and verification, McEliece encryption and decryption processes might introduce some inefficiencies due to their large key size and computational complexity.

- **Adoption**: The transition to a McEliece-based system requires widespread changes to the Bitcoin infrastructure, including replacing the ECDSA signature scheme, which is deeply embedded in the network.

#### Conclusion

By integrating **McEliece**, a quantum-resistant signature scheme, with **zk-SNARKs**, P2P CoinJoin can provide both privacy and post-quantum security. This combination ensures that even in the face of quantum threats, participants can safely and privately conduct transactions on decentralized networks like Bitcoin. While there are challenges related to performance and adoption, this approach offers a viable path forward in securing financial transactions in a quantum world.
