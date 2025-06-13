# Crypto Password Recovery: Regain Access to Your Digital Assets with WalletGen

**Locked out of your crypto wallet due to a forgotten password or seed phrase?** **WalletGen** offers a powerful, open-source solution, acting as a versatile **crypto password recovery** tool. It helps you potentially recover lost or inactive **Bitcoin (BTC)**, **Ethereum (ETH)**, **BNB**, **Polygon (MATIC)**, and other **EVM-compatible wallets** using a high-performance C++ engine with real-time balance checks.

<!--
Meta description:
Need crypto password recovery? WalletGen is your open-source solution. Recover lost Bitcoin, Ethereum, and EVM-compatible wallets with speed and efficiency. Brute-force seed recovery & balance checks. Get your crypto back!
-->

## Quick Navigation
- [How It Works: Understanding WalletGen's Core Features](#how-it-works)
- [Why Choose WalletGen for Crypto Password Recovery?](#why-walletgen)
- [Features: Key Advantages in Crypto Recovery](#features)
- [Download WalletGen: Start the Recovery Process](#how-to-start)
- [Optimize Your Search: Database Downloads and Usage](#download-and-use-database-for-more-speed)
- [What Happens When a Wallet Is Found: Next Steps](#the-program-found-a-wallet--whats-next)
- [Recovering Your Bitcoin: A Step-by-Step Guide](#recovery-your-bitcoin-wallet)
- [My Finds: Success Stories and Real Results](#my-finds)
- [FAQ: Crypto Password Recovery - Your Questions Answered](#-frequently-asked-questions-faq)
- [Build Instructions: Compile the Project Yourself](#building-the-project)
- [Support Development: Donate to the Project](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="crypto password recovery" title="WalletGen wallet generator" height="460" src="/storage/new.webp" />
</p>

⚠️ **Disclaimer**:  WalletGen is a research and educational tool. It's not meant for unauthorized access or malicious activities. Use it responsibly and only with wallets you own or have permission to access.

## How It Works

WalletGen relies on the well-established [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki), [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki), and [Bech32](https://en.bitcoin.it/wiki/Bech32) for Bitcoin wallet generation.  For EVM-based chains such as Ethereum, the software leverages the [Keccak256](https://emn178.github.io/online-tools/keccak_256.html) hashing algorithm.

The core process of WalletGen is to generate a multitude of potential wallet addresses, and then verify their current balance. This is accomplished either by conducting live balance checks against public blockchain explorers, or, much more efficiently, by comparing the generated addresses against a pre-existing database of known wallets which contain funds. The C++ foundation of WalletGen allows for significantly faster speeds than many of the Python based alternatives, with the overall speed mainly relying on your CPU and GPU.

## Why Choose WalletGen for Crypto Password Recovery?

Need to get back into your crypto wallets?  **WalletGen** has been crafted for speed and efficiency!  Unlike slower Python-based alternatives, it has been written in C++ and optimized for multi-threaded CPU and GPU usage. It delivers up to **10x faster** performance.  Whether you're working to recover lost wallets, validating private key spaces, or aiming to regain control of your crypto holdings, WalletGen offers speed, security, and ease.

## Features

-   **Cryptocurrency Wallet Generation**: Create single wallets for Bitcoin, Ethereum, BNB, MATIC, and more.
-   **Balance Finding with Brute-Force**: Employ brute-force techniques to search for wallets with balances on Bitcoin and EVM networks.
-   **Algorithm Support**: Supports the Keccak256 algorithm for EVM wallets and BIP39, BIP44, and Bech32 for Bitcoin.
-   **Database Integration for Speed**: Leverage databases to greatly improve search efficiency.
-   **High-Speed Operation**: WalletGen uses the power of your CPU and GPU for peak performance.
-   **Bitcoin Seed Phrase Recovery**: Recover your Bitcoin wallet using your mnemonic seed phrase.

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="WalletGen search lost bitcoin wallets on Windows Demo" title="WalletGen search lost bitcoin wallets on Windows" src="/storage/wide.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="WalletGen search lost bitcoin wallets on Linux Demo" title="WalletGen search lost bitcoin wallets on Linux" src="/storage/snap.webp" />
</p>

# How to start

## Windows
-   Download [Release](../../releases)
-   Unpack anywhere
-   Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## Linux (x86-64bit)

Use wget
or download [Release for Linux](../../releases)




## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** employs brute-force methods for searching wallets with balances.

### Bitcoin (BTC) Wallet Search:

*   Press `3` in the menu or run `start_search_btc.bat` to search Bitcoin wallets over the internet. This may take longer since it does real-time balance checks.
*   Press `6` to search using the database. This is faster as it compares generated wallets with a database.

### EVM Wallet Search (Ethereum, BNB, MATIC, etc.):

*   Press `5` or run `start_search_evm.bat` for an internet-based search. Balances are checked in real-time with blockchain explorers.
*   Press `6` to use the database. This is faster as it compares against the known database.

### Speed Considerations:

*   Your hardware, especially the graphics card (GPU), greatly affects search speed. Run multiple instances (1 to 4) to increase your chances.

Databases improve search efficiency by avoiding the need for real-time blockchain queries.

## The Program Found a Wallet — What’s Next?

If WalletGen finds a wallet with a balance:
*   The search will **Stop** immediately.
*   The wallet details are **Displayed** in the console.
*   The data is **Saved** in the `found_wallets.txt` file.

### How to Access the Funds?

1.  Import the **mnemonic seed phrase** into any compatible crypto wallet (such as Metamask, Trust Wallet, or Electrum).
2.  You can then transfer the funds to your own wallet.

>  Consider donating a portion of the recovered balance as a thank you!

## Recovery Your Bitcoin Wallet

WalletGen can help you recover your Bitcoin wallet using the seed phrase. Enter the full phrase, or use wildcards to search for missing words.

### Process Description

#### Search for Missing Words:

Use * if words are missing. WalletGen checks all combinations.

#### Entering a Complete Seed Phrase:

If you have all 12 words, enter them. WalletGen then generates and checks addresses.

![recovery](/storage/maximized.webp)

### Important Recommendations

*   Seed phrases have 12 words.
*   Use * only for missing words.
*   Searching for missing words can take time.
*   Upon recovery, data is saved.

## My Finds

![mywallet](/storage/scr.webp)

I've recovered two BTC wallets with balances. The first had 0.000032 BTC; the second, 0.0528 BTC (about $4800).
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/storage/patch.webp" />
</p>

### New Find 4/9/2025

After a week of searching, I found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my largest find!

![image](/storage/alert.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/storage/summary.webp)

## Building the Project

1.  Open the project file (`CryptoWalletGen.sln`) in Visual Studio or a compatible C++ compiler.
2.  Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
Download WalletGen on the [release download page](../../releases).

### ❓ Where can I download a database of known addresses?
Find the latest database on the [release page](../../releases).

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes, WalletGen can help recover lost Bitcoin wallets with brute-force seed generation and a known-address database.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute, submit a pull request.

## Donate

Consider donating a portion of the recovered balance as a thank you.

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)



Update: Link is now reachable