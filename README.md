# Quantum Cybernetic Chaos Hybrid Encryption Engine (QCCHEE)



# Quantum-Cybernetic Chaos Hybrid Encryption Engine (QCCHEE)

**Project Overview**  
QCCHEE is an experimental hybrid encryption framework that combines post-quantum cryptographic primitives with adaptive, chaos-derived entropy and hardware-backed key management. The goal is cryptographic agility: dynamically selecting the optimal algorithm per data stream while maintaining high performance and forward secrecy.

**Core Architecture**  
- **Dual Adversarial Deep Learning Layer** (research prototype): An encryption model trained on cryptographic primitives and attack vectors works in tandem with an adversarial model that stress-tests outputs in real time. Weaknesses are fed back to strengthen the system.  
- **Dynamic Triage Engine**: Selects from a rotating set of NIST post-quantum candidates based on sensitivity, latency, and payload size.

**Supported Post-Quantum Primitives**  
**Key Encapsulation (KEM):**  
- ML-KEM (Kyber) – primary for speed  
- FrodoKEM – conservative lattice fallback  
- BIKE – code-based diversity  

**Digital Signatures:**  
- Dilithium – general purpose  
- FALCON – minimal signature size  
- SPHINCS+ – hash-based long-term security  

**Key Generation & Entropy**  
Volatile keys are derived from hardware entropy sources (TPM, Intel RDRAND) combined with chaotic attractors (Lorenz/Logistic maps). Keys mutate per block using ciphertext feedback, eliminating static storage and replay risk. No persistent keys are written to disk.

**Additional Security Features**  
- Zero-trust design  
- Zero-knowledge proof support (ZK-SNARKs/STARKs)  
- Threshold/multi-signature capability  
- Optional timed key self-destruct

**Current Status**  
Proof-of-concept stage. Python implementation with TPM integration available. Deep-learning components are in planning/training phase (see training notes in repo). Not production-ready; intended for research and controlled testing.
