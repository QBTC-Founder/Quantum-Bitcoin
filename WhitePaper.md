# Quantum Bitcoin ($QBTC) Whitepaper

## 1. Introduction
Quantum Bitcoin (QBTC) is a post-quantum resistant digital asset. By implementing the **W-Protocol**, we ensure that transactions remain secure even against Shor’s algorithm and other quantum-level attacks.

---

## 2. The W-Protocol Architecture
The heart of QBTC is the **W-Protocol v1.1.0**. Unlike traditional blockchain security, W-Protocol utilizes **Lattice-Based Cryptography**, specifically optimized for mobile and decentralized nodes.

### 2.1 Gateway Implementation
The W-Protocol Gateway acts as a quantum-secure bridge. It intercepts standard transaction requests and wraps them in a lattice-based signature (**LWE-encrypted**) before executing the smart contract on the Solana SPL layer. This prevents "Harvest Now, Decrypt Later" attacks.

**Key Technical Parameters:**
* **Mathematical Foundation:** Short Integer Solution (SIS) and Learning With Errors (LWE).
* **Prime Modulus (q):** 12289 (NewHope Standard).
* **Security Hashing:** SHA-384 for enhanced post-quantum resistance.

---

## 3. Implementation Logic
The protocol's core functions are simulated in `car_logic.py`, focusing on lattice vector generation and secure node initialization.

