# Overview

Burrow is a self-hosted RAG pipeline designed to transform unstructured documents into vectorized formats for semantic search and retrieval. By automating document ingestion and vector embedding, Burrow enables teams to easily build production-grade RAG applications on their own infrastructure.

The platform accepts documents through a user-provided interface, where they are uploaded to S3. Once a document is added, Burrow processes the content by extracting meaningful features and converting them into vector embeddings using AWS Bedrock. These embeddings are stored in a PostgreSQL database with pgvector, making them ready for semantic search and integration with downstream AI applications.

To learn more about Burrow, visit our [website](https://burrow-io.github.io/burrow-case-study/) and [case study](https://burrow-io.github.io/burrow-case-study/case-study).

To get started deploying Burrow, visit our [instructions here](https://github.com/burrow-io/burrow-cli).

## Burrow Components

Burrow is built with several different components:

- **burrow-cli** - CLI to deploy Burrow's AWS infrastructure with just a few terminal commands.
- **burrow-frontend** - React dashboard for uploading documents and querying your RAG pipeline.
- **burrow-management-api** - Express.js API for document lifecycle management and authentication.
- **burrow-query-api** - FastAPI service for semantic search and RAG query processing.
- **burrow-ingestion** - Python pipeline for document parsing, chunking, and embedding generation.
- **burrow-infrastructure** - Terraform configurations to provision all AWS resources.
- **burrow-load-tests** - Performance testing suite to validate system scalability.
- **burrow-case-study** - Technical documentation website with architecture deep-dives and design decisions.
