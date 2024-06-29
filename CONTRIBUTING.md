# Contributing to BlockAPIWallet

Thank you for your interest in contributing to BlockAPIWallet! We welcome contributions from the community and appreciate your efforts to improve our project. Please follow these guidelines to ensure a smooth and collaborative process.

## How Can I Contribute?

### Reporting Issues

If you encounter any bugs, glitches, or have suggestions for improvements, please report them using the GitHub issues tracker. Provide as much detail as possible, including:

- A clear and descriptive title
- A detailed description of the issue or suggestion
- Steps to reproduce the issue, if applicable
- Any relevant logs, screenshots, or code snippets

### Forking the Repository

1. Fork the repository by clicking the "Fork" button on the GitHub page.
2. Clone your forked repository to your local machine:

    ```sh
    git clone https://github.com/yourusername/blockapiwallet.git
    cd blockapiwallet
    ```

### Setting Up Your Development Environment

1. Install Golang (1.16+).
2. Install Docker.
3. Ensure your preferred blockchain node(s) are set up and accessible.
4. Create a `.env` file in the root directory with your configuration settings:

    ```env
    PUBLIC_KEY=your_public_key
    SECRET_KEY=your_secret_key
    NODE_URL=your_blockchain_node_url
    ```

### Making Changes

1. Create a new branch for your feature or bug fix:

    ```sh
    git checkout -b feature/your-feature-name
    ```

2. Make your changes in the new branch.
3. Test your changes thoroughly to ensure they work as expected.
4. Commit your changes with a clear and concise commit message:

    ```sh
    git commit -m "Add feature X to improve Y"
    ```

5. Push your changes to your forked repository:

    ```sh
    git push origin feature/your-feature-name
    ```

### Submitting a Pull Request

1. Go to the original repository on GitHub and navigate to the "Pull requests" tab.
2. Click the "New pull request" button.
3. Select the branch you want to merge into the main repository.
4. Provide a clear and detailed description of your changes in the pull request.
5. Submit the pull request for review.

### Code Style and Standards

- Follow the Golang coding standards and best practices.
- Write clear and concise code with comments where necessary.
- Ensure your code passes all tests and does not introduce any new issues.

### Reviewing and Merging

- A project maintainer will review your pull request.
- You may be asked to make additional changes or provide more information.
- Once approved, your changes will be merged into the main repository.

## Community Guidelines

- Be respectful and considerate in your interactions.
- Provide constructive feedback and be open to feedback from others.
- Focus on improving the project and helping the community.

## License

By contributing to BlockAPIWallet, you agree that your contributions will be licensed under the MIT License.

Thank you for your contributions and for helping make BlockAPIWallet better! If you have any questions, feel free to open an issue or contact us.

