# Overview

Burrow is an open-source RAG-as-a-service platform that provides teams with a complete ETL pipeline and advanced retrieval techniques. By automating document processing and implementing production-grade retrieval methods, Burrow enables developers to easily integrate high-quality document retrieval into their RAG applications.

The platform provides a web interface where documents are uploaded. Once a document is added, Burrow uses event-driven architecture to automatically spin up ECS Fargate tasks that parse, chunk, and convert the content into vector embeddings using AWS Bedrock. These embeddings are stored in a PostgreSQL database with pgvector and made available through query APIs that support keyword search, semantic search, reranking, and metadata filtering to retrieve the most relevant chunks for LLM generation.

To learn more about Burrow, visit our [website](https://burrow-io.github.io/) and [case study](https://burrow-io.github.io/case-study/).

To get started deploying Burrow, visit our [instructions here](https://github.com/burrow-io/burrow-cli).

## Burrow Components

Burrow is built with several different components:

- [burrow-cli](https://github.com/burrow-io/burrow-cli) - CLI to deploy Burrow's AWS infrastructure with just a few terminal commands.
- [burrow-frontend](https://github.com/burrow-io/burrow-frontend) - React dashboard for uploading documents and querying your RAG pipeline.
- [burrow-management-api](https://github.com/burrow-io/burrow-management-api) - Express.js API for document lifecycle management and authentication.
- [burrow-query-api](https://github.com/burrow-io/burrow-query-api) - FastAPI service for semantic search and RAG query processing.
- [burrow-ingestion](https://github.com/burrow-io/burrow-ingestion-task) - Python pipeline for document parsing, chunking, and embedding generation.
- [burrow-infrastructure](https://github.com/burrow-io/burrow-infrastructure) - Terraform configurations to provision all AWS resources.
- [burrow-load-tests](https://github.com/burrow-io/burrow-load-tests) - Performance testing suite to validate system scalability.
- [burrow-case-study](https://github.com/burrow-io/burrow-io.github.io) - Technical documentation website with architecture deep-dives and design decisions.

## The Team

[Zach Bajcar](https://github.com/ZBajcar) Software Engineer • Poughkeepsie, NY

[Wilson Chen](https://github.com/wchen22) Software Engineer • New York City, NY

[Daniela Pavlova](https://github.com/pavlovadb) Software Engineer • Sparks, NV

[Trixy Fabrigar](https://github.com/t-fb) Software Engineer • Vancouver, BC
