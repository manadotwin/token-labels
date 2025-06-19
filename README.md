# MANA.WIN Community Address Labels

This repository contains the community-maintained list of address labels for [mana.win](https://mana.win) built on the Hyperliquid EVM network.

## Purpose

The `labels.json` file maps blockchain addresses to human-readable labels. These labels help the mana.win platform and its users quickly identify important addresses, such as:

* Team wallets and treasury contracts
* Liquidity and staking contracts
* Special-purpose addresses (e.g., burn address)

> **Example**:
>
> ```json
> {
>   "0x000000000000000000000000000000000000dead": "Burn Address"
> }
> ```

## How to Add an Address Label (`labels.json`)

1. **Fork** this repository to your GitHub account.
2. **Clone** your fork locally.
3. Open the `labels.json` file.
4. Add a new key-value entry:

   * **Key**: the Hyperliquid EVM address in checksummed format (string).
   * **Value**: the desired label (string).

   ```json
   {
     "0x000000000000000000000000000000000000dead": "Burn Address",
     "0xYourNewAddress________________________": "Your Label"
   }
   ```
5. Ensure the JSON remains valid after adding your entry.
6. **Commit** your changes with a clear message, for example:

   ```bash
   git commit -m "feat: Add label for <Description>"
   ```
7. **Push** your updates to your fork.
8. **Open a Pull Request** against the `main` branch of this repository. In your PR description, briefly explain why this label is needed (e.g., “Official treasury address for Project X”).

## Pull Request Review Process

* We will verify the address format and the accuracy of the suggested label.
* Labels for publicly recognizable contracts or project addresses usually receive faster approval.
* Once validated, your PR will be merged.

## Questions & Support

If you have any questions or encounter issues, reach out to us on Telegram: **@manadotwin**

Thank you for contributing to the **mana.win** ecosystem!
