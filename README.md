# HashiCorp Vault Integration with Node.js

In this repository, I explore how to integrate **HashiCorp Vault** with a **Node.js** application to securely manage sensitive data such as email-password pairs.

This project demonstrates how to:
- Install HashiCorp Vault on Windows
- Connect Vault with a Node.js application using the `node-vault` library
- Perform basic CRUD (Create, Read, Update, Delete) operations for securely storing email-password pairs

If you're looking to enhance security in your applications or learn about Vault, this project will help you understand the basics.

## Features

- **Store Credentials**: Securely save an email and password pair in Vault.
- **Update Credentials**: Modify the password for a stored email.
- **Retrieve Credentials**: Fetch the password for a given email from Vault.
- **Delete Credentials**: Remove the email-password pair from Vault.

## Prerequisites

Before you begin, make sure you have the following installed:
- [Node.js](https://nodejs.org/) (to run the project)
- [HashiCorp Vault](https://www.vaultproject.io/) (for secret management)

## Setup Instructions

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/vault-node-integration.git
   cd vault-node-integration

2. **Install dependencies**:
    ```bash
    npm install

Download and Install HashiCorp Vault:

Download Vault from the official Vault downloads page.

Extract the files and move the vault.exe to a directory (e.g., C:\vault).

Add C:\vault to your system PATH so you can run the vault command globally.

Verify Vault installation by running the following in your terminal:
    ```bash
    vault

3. **Start Vault in Development Mode**:

In your terminal, start Vault in development mode by running:
        ```bash
        vault server -dev

Copy the Root Token displayed in the terminal after Vault starts. You’ll need this for authentication.

4. **Set up environment variables**:

Create a .env file in the project root directory with the following content (replace <your-root-token> with your Vault token):
    ```bash
    VAULT_ADDR=http://127.0.0.1:8200
    VAULT_TOKEN=<your-root-token>

5. **Run the Application**:

Now that everything is set up, run the Node.js application with:
    ```bash
    node index.js

This will run the example that demonstrates saving, retrieving, updating, and deleting credentials from Vault.

# Medium Article
For a full, step-by-step tutorial and explanation, check out my article on Medium:

👉 [How to Integrate HashiCorp Vault with Node.js: Securely Manage Sensitive Data](https://medium.com/@gowtham06/how-to-integrate-hashicorp-vault-with-node-js-securely-manage-sensitive-data-5201a821c1eb)

License
This project is licensed under the MIT License.




