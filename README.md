# Proverif-Automatic-Security-Verification
Mutual Authentication and Message Integrity Verification
This project aims to provide Message Integrity Verification and Mutual authentication in a smart home scenario where there is a Server, an IoT device, and a Smartphone user. Mutual authentication is when the sides of a communication channel verify each other. It is a two-way authentication because it goes in both directions. Message Integrity verification is a way of ensuring that the message received has not been tampered with. These are very important to guarantee security from a rogue network.
Proverif is a software tool for evaluating several cryptographic protocols and primitives including symmetric and asymmetric cryptography. For beginners, the Proverif software can be installed on Windows and MACOS as follows;

For Windows:
1. Install Cygwin from the following link https://www.cygwin.com/install.html by running setup-x86_64.exe.
2. Open the Cygwin terminal.
3. Download the Proverif binary from https://bblanche.gitlabpages.inria.fr/proverif/ and
then uncompress using tar -xzf proverifbin2.04.tar.gz

For MACOS:
1. Install the Homebrew package manager for Mac OS by running the following command: /bin/bash
-c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
2.  Run the following commands:
• echo 'eval "$(/opt/homebrew/bin/brew shellenv)"'
• eval "$(/opt/homebrew/bin/brew shellenv)"
3.  Install Opam using the following commands:
• brew install opam
• opam init
• eval $(opam env –-switch=default)
4.  Now install ProVerif using the following commands:
• opam install proverif
• opam depext proverif

After installation
Open the Cygwin64 Terminal, 
cd proverif2.04
./proverif IOT_auth_2.pv to run your proverif script. Make sure the script is in a directory where Proverif can see it. The correspondence assertions and results will be displayed on the terminal.

This project outlines 3 parts protocol design namely,
1. Mutual authentication between the IoT and the server.
2. Mutual authentication between the smartphone user and the server.
3. Data Integrity and Confidentiality for messages sent by the IoT devices to the server.
The report written for this project can be provided on request via Email: oguchiebuka919@gmail.com.
 
The project can be scaled to multiple IoT devices and servers if you so desire. The communication between the Smartphone user and the Server uses a public key (asymmetric cryptography) while The IoT and server use symmetric cryptography due to their lightweight nature.
