# Simple Blockchain

**Simple Blockchain** is a C-based project that demonstrates the core principles of blockchain technology, including **hash chaining, proof-of-work, and integrity verification**. It’s a hands-on implementation to explore how blockchains maintain secure, tamper-proof records.

## Highlights

- **Blockchain Implementation:** Each block stores its own data, hash, previous block hash, nonce, timestamp, and index.  
- **Proof-of-Work Mining:** Automatically finds a nonce that satisfies a target hash, simulating mining.  
- **Integrity Verification:** Checks the chain to ensure no tampering has occurred by validating all hashes.  
- **Cryptography:** Uses SHA256 hashing via OpenSSL (`libcrypto`) for secure block identification.  
- **Cross-Platform Build:** Uses CMake for Linux/ARM/Intel platforms.

## Tech Stack

- **Language:** C  
- **Build System:** CMake  
- **Libraries:** OpenSSL (`libcrypto`), platform-specific test libraries  

## Project Structure

```
src/       # Source code
include/   # Header files
lib/       # Libraries for testing
CMakeLists.txt  # Build configuration
```

## Getting Started
```bash
git clone https://github.com/marikascrepnek/simple-blockchain.git
cd simple-blockchain
mkdir build && cd build
cmake ..
make
./blockchain
```

## Skills Demonstrated

- Implementing blockchain data structures in C
- Writing proof-of-work logic and nonce calculation
- Using cryptographic hashing for data integrity
- Building and linking C projects with external libraries
- Debugging memory and synchronization issues
