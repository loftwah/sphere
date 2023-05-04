# Sphere Vault

Sphere Vault leverages the OP Stack (OpenAI + Pinecone Vector Database) to allow users to upload their custom knowledge base files and inquire about their contents.

[sphere.bookloop.club](https://sphere.bookloop.club)

## Features

With Sphere Vault, you can:

* Upload a variety of popular document types via a simple React frontend to create a custom knowledge base
* Retrieve accurate and relevant answers based on the content of your uploaded documents
* See the filenames and specific context snippets that inform the answer
* Explore the power of the OP Stack (OpenAI + Pinecone Vector Database) in a user-friendly interface
* Load entire libraries' worth of books into Sphere Vault

## Manual Dependencies

* node: v19
* go: v1.18.9 darwin/arm64
* poppler

## Setup

1. Install manual dependencies:

   * Install Go: Follow the Go docs [here](https://go.dev/doc/install)
   * Install node v19: Use [nvm to install node v19](https://medium.com/@iam_vinojan/how-to-install-node-js-and-npm-using-node-version-manager-nvm-143165b16ce1)
   * Install poppler: `sudo apt-get install -y poppler-utils` on Ubuntu, or `brew install poppler` on Mac

2. Set up your API keys and endpoints in the `secret` folder:

   * Create a new file `secret/openai_api_key` and paste your [OpenAI API key](https://platform.openai.com/docs/api-reference/authentication) into it: `echo "your_openai_api_key_here" > secret/openai_api_key`
   * Create a new file `secret/pinecone_api_key` and paste your [Pinecone API key](https://docs.pinecone.io/docs/quickstart#2-get-and-verify-your-pinecone-api-key) into it: `echo "your_pinecone_api_key_here" > secret/pinecone_api_key`
   * Create a new file `secret/pinecone_api_endpoint` and paste your [Pinecone API endpoint](https://app.pinecone.io/organizations/) into it: `echo "https://<your-url>.pinecone.io" > secret/pinecone_api_endpoint`

3. Running the development environment:

   * Install JavaScript package dependencies: `npm install`
   * Run the Golang web server (default port `:8100`): `npm start`
   * In another terminal window, run Webpack to compile the JS code and create a bundle.js file: `npm run dev`
   * Visit the local version of the site at <http://localhost:8100>

For more detailed information about uploading files, asking questions, and the underlying technology, please refer to the original repository.

## Licensing

This project is licensed under the BSD 3-Clause License. Please find the full license text in the `LICENSE` file of the project repository.
