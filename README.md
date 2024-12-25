# Quantum-Cryptography-Simulator

History
The concept of cryptography has evolved significantly over the past century. In 1977, RSA encryption revolutionized secure communication by introducing public-key cryptography, relying on the computational difficulty of factoring large numbers. However, this system faces a significant threat from quantum computing, as Peter Shor’s algorithm (1994) demonstrated the ability to efficiently factor integers, breaking RSA and other classical encryption methods.

In response, quantum cryptography emerged, offering security based on the principles of quantum mechanics rather than computational assumptions. The first quantum key distribution (QKD) protocol, BB84, was introduced in 1984 by Charles Bennett and Gilles Brassard.

Problem
Classical cryptographic methods, like RSA, are vulnerable to attacks by quantum computers. Quantum computing algorithms can break the mathematical complexity underpinning RSA, leaving secure communication at risk.

How Quantum Cryptography Solves the Problem
Quantum cryptography provides a fundamentally different approach:
- It uses quantum properties (superposition and entanglement) to encode information in particles such as photons.
- Eavesdropping detection: Any attempt to intercept the quantum states (e.g., polarized photons) disturbs the system, making the interference detectable.
- This ensures that only Alice (sender) and Bob (receiver) can securely share a key, while any intrusion by Eve (eavesdropper) is revealed.

How Code Explains Quantum Cryptography:
This code simulates the foundational concepts of QKD:
- Random Basis Selection: Alice, Bob, and Eve randomly choose measurement bases (+ or x), representing photon polarization directions.
- Message Encoding and Decoding: Alice encodes a binary message using her basis, and Bob decodes it using his. Their results align only when their bases match.
- Eve's Interference: When Eve intercepts and measures the message, her random guesses disturb the system, introducing errors detectable by Alice and Bob.
- Accuracy and Error Detection: The simulation shows how Eve's interference reduces accuracy, highlighting the security of quantum communication.

This program bridges abstract quantum mechanics with practical cryptography, providing a hands-on way to understand how quantum cryptography detects eavesdropping and ensures secure communication.
