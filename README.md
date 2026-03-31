Simple Blockchain

Simple Blockchain is a C-based project that demonstrates the core principles of blockchain technology, including hash chaining, proof-of-work, and integrity verification. It’s designed as a hands-on way to understand how blockchains like Bitcoin maintain secure, tamper-proof records.

Highlights
Blockchain Implementation: Each block stores data, its own hash, the previous block’s hash, a nonce, timestamp, and index.
Proof-of-Work Mining: Automatically finds a nonce that satisfies a target hash, mimicking real-world mining.
Integrity Verification: Ensures the chain hasn’t been tampered with by validating hashes and links between blocks.
Cryptography: Uses SHA256 hashing via OpenSSL (libcrypto) for secure block identification.
Cross-Platform Build: CMake-based build system for Linux/ARM/Intel platforms.
Tech Stack
Language: C
Build System: CMake
Libraries: OpenSSL (libcrypto), platform-specific test libraries
Structure
src/       # Source code
include/   # Header files
lib/       # Libraries for testing
CMakeLists.txt  # Build configuration
Getting Started
git clone https://github.com/yourusername/simple-blockchain.git
cd simple-blockchain
mkdir build && cd build
cmake ..
make
./blockchain
Skills Demonstrated
Implementing blockchain data structures in C
Writing proof-of-work logic and nonce calculation
Using cryptographic hashing for data integrity
Building and linking C projects with external libraries
Debugging memory and synchronization issues
