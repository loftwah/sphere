# Sphere Vault

Sphere Vault leverages the OP Stack (OpenAI + Pinecone Vector Database) to allow users to upload their custom knowledge base files and inquire about their contents.

[sphere.bookloop.club](https://sphere.bookloop.club)

With a quick setup, you can launch your own version of this Golang server, accompanied by a user-friendly React frontend that enables users to ask OpenAI questions about the specific knowledge base provided. The main focus is on human-readable content like books, letters, and other documents, making it a practical and valuable tool for knowledge extraction and question-answering. You can upload an entire library's worth of books and documents and receive pointed answers along with the name of the file and the specific section within the file that the answer is based on!

## What can you do with Sphere Vault?

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

Please follow the setup instructions in the original repository, including installing manual dependencies, setting up API keys and endpoints in the `secret` folder, and running the development environment. Instructions for uploading files, asking questions, and information about the underlying technology can also be found in the original repository.

## Licensing

This project is now licensed under the BSD 3-Clause License. Please find the full license text in the `LICENSE` file of the project repository.
