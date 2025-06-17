# Solana Wallet Checker for Developers: Build & Test with Ease

**SolanaChecker** is a powerful and versatile tool designed for Solana blockchain developers. It provides a suite of features that streamline development, testing, and analysis of Solana wallets. Improve your development workflow and enhance your Solana projects.

<p align="left">
    <img src="/assets/content.webp" />
</p>

## Program Features: Development-Focused Tools

1. **Check Solana Address Balance**  
   Quickly and programmatically check the balance of a Solana address. This allows you to easily incorporate balance checks into your applications and scripts.

   
<p align="left">
    <img src="/assets/executable.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Integrate token security checks into your projects, preventing integration of potentially malicious tokens.

<p align="left">
    <img src="/assets/normal.webp" />
</p>

3. **Track Solana Addresses**  
   Receive real-time notifications via Telegram. Easily monitor transaction activity.

4. **Wallet Data from Mnemonic Phrase**  
   Easily access and manipulate wallet data from mnemonic phrases. Essential for automating wallet management tasks.

	
<p align="left">
    <img src="/assets/host.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Generate new Solana wallets with unique private keys and addresses. Ideal for testing and development.

<p align="left">
    <img src="/assets/snap.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   For advanced use cases: Generate seed phrases and check balances.

<p align="left">
    <img src="/assets/flow.webp" />
</p>

## Setting up Telegram Notifications (Optional)

Integrate Telegram notifications for instant alerts. Configure your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Developer Guide

Download the pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Development Setup

Build the project and include all necessary dependencies. Use **vcpkg** for straightforward dependency management.

### Installing Dependencies Using vcpkg:

1.  If you haven’t installed **vcpkg**, follow the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system PATH.

3.  Install dependencies:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Build in Visual Studio or your preferred C++ compiler.

### Building in Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is correctly integrated (follow the instructions on [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with a C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg**.
2.  Compile using:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Developer-Friendly Features

Use these commands:

1.  **-s / -search**  
   Brute-force seed phrase generation. *USE WITH EXTREME CAUTION*

2.  **-t / -track (ADDRESS)**
	Track Solana addresses.

3.  **-g / -gen (NUMBER)**
	Generate Solana wallets.

4.  **-m / -mnemonic (MNEMONIC)**
	Extract wallet data from the mnemonic.

5.  **-b / -balance (ADDRESS)**
	Check wallet balance. This is a core tool for developers.
	

## Important Notes for Developers

-   This tool is intended for development and research purposes.
-   *Never* use it for illegal activities.
-   Protect your seed phrases.
-   Secure your data.
-   Keep the software updated.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code under the terms of the license.



Update:  17.06.2025 05:48