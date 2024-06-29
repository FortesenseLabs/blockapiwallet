# BlockAPIWallet Documentation

Welcome to the BlockAPIWallet documentation. This guide will help you understand how to use and integrate BlockAPIWallet into your projects.

## Overview

BlockAPIWallet is an open-source, enterprise-grade blockchain wallet-as-a-service solution. It provides a secure, scalable, and API-driven platform for managing digital assets across multiple blockchains. Developed in Golang and based on trust-wallet wallet-core, BlockAPIWallet is containerized using Docker for seamless deployment and integration.

## Features

- **Enterprise-Grade Security**: Utilizes MPC (Multi-Party Computation) technology for secure key management.
- **API-Driven**: Comprehensive APIs for creating and managing accounts, addresses, and transactions.
- **Multi-Blockchain Support**: Compatible with multiple blockchains including Bitcoin, Ethereum, Tron, Binance Smart Chain, Polygon, Solana, and more.
- **Docker Containerized**: Easily deployable in a Docker container for seamless integration with your infrastructure.
- **Customizable Policies**: Configure withdrawal, approval, and collection policies to meet your organization's needs.
- **Smart Contract Interaction**: Generate and deploy gasless smart contract addresses on supported chains.

## Getting Started

### Prerequisites

- Docker
- Golang (1.16+)
- Make sure you have your preferred blockchain node(s) set up and accessible.

### Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/yourusername/blockapiwallet.git
   cd blockapiwallet
   ```

2. **Build and run the Docker container:**

   ```sh
   docker build -t blockapiwallet .
   docker run -d -p 8080:8080 blockapiwallet
   ```

3. **Configure environment variables:**

   Create a `.env` file in the root directory with your configuration settings:

   ```env
   PUBLIC_KEY=your_public_key
   SECRET_KEY=your_secret_key
   NODE_URL=your_blockchain_node_url
   ```

### Usage

- **Authentication:**

  Use the public and secret keys to authenticate API requests. Concatenate them in the format `{public_key:secret_key}`, encode in base64, and include in the Authorization header.

- **API Endpoints:**

  - **Create Account:**

    ```http
    POST /api/v1/accounts
    ```

  - **Generate Address:**

    ```http
    POST /api/v1/addresses
    ```

  - **Transfer Funds:**

    ```http
    POST /api/v1/transactions
    ```

  Refer to the [API Documentation](docs/API.md) for a complete list of endpoints and usage instructions.

## Configuration

- **Supported Blockchains:**

  BlockAPIWallet supports multiple blockchains, with more being added continuously. Check the configuration file for the list of currently supported blockchains.

- **Policies:**

  Customize your policies for withdrawals, approvals, and collections by modifying the `config/policies.json` file.

## References

For more information on wallet infrastructure and similar projects, refer to the [Bitpowr Wallet Infrastructure](https://bitpowr.com/product/wallet-infrastructure).

## License

BlockAPIWallet is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions, issues, or feature requests, please open an issue on GitHub or contact us at support@blockapiwallet.com.
