Subject: Vector store data for RAG
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Thu, 15 Oct 2026 09:14:11 -0400) ---
# Vector Store Architecture & Optimization Strategies for Sim.ai RAG
Knowledge Bases

## 1. Native Engine: `pgvector` (PostgreSQL)

The Sim.ai Knowledge Base uses **`pgvector` (PostgreSQL vector extension)**
as its core default vector engine, alongside support for third-party vector
databases depending on your deployment model.

### Default Backend Architecture
* **Under the Hood:** Sim’s native architecture is built on **Bun, Next.js,
and PostgreSQL with `pgvector`**.
* **Sim Cloud Execution:** On the managed Sim Cloud, `pgvector` powers the
knowledge base automatically behind the scenes. It generates
1,536-dimensional vector embeddings (using OpenAI's
`text-embedding-3-small` model by default) and manages index storage
seamlessly.
* **Self-Hosting:** In self-hosted Docker Compose / local deployments, Sim
packages PostgreSQL with `pgvector` right out of the box.

---

## 2. Native Retrieval Capabilities

Sim's underlying knowledge layer supports advanced retrieval paradigms out
of the box:

* **Hybrid Search:** Combines full-text (BM25-style keyword scoring) with
semantic vector search (cosine similarity via `pgvector`) using Reciprocal
Rank Fusion (RRF).
* **Reranking:** Optional cross-encoder reranking pass on top of vector or
hybrid results to re-order returned chunks by true relevance before feeding
them to agents.

---

## 3. Dedicated External Vector Store Integrations

While `pgvector` serves as Sim's native engine, Sim.ai supports connecting
or syncing with dedicated external vector databases for larger scale,
complex metadata needs, or specific enterprise infrastructure requirements:

### Qdrant Optimization: High-Speed Payload Filtering & Memory Efficiency
* **Single-Stage Payload Filtering:** Performs metadata filtering during
HNSW graph traversal rather than as a post-retrieval step, preserving
search recall and speed when agents use strict tag filters (e.g.,
`department: legal`).
* **In-Memory Quantization:** Supports scalar and binary quantization,
allowing millions of chunk vectors to remain in memory at sub-10ms query
latencies.
* **Best Used For:** Workflows requiring ultra-low latency, complex
metadata filtering, or high-performance Rust-based self-hosted deployment
models.

### Pinecone Optimization: Fully Managed Enterprise Scale & Multi-Tenancy
* **Serverless Elasticity:** Automatically scales vector index storage and
compute as the Sim.ai Knowledge Base expands from thousands to tens of
millions of chunks without requiring database sharding or cluster
maintenance.
* **Multi-Tenant Namespaces:** Isolates vector data per enterprise user or
tenant within a single index, preventing cross-tenant data leaks.
* **Best Used For:** Enterprise applications requiring managed low-latency
cloud vector search, turnkey scaling, and SOC2/HIPAA compliance.

### Weaviate Optimization: Multi-Modal RAG & Schema-Rich Hybrid Search
* **Built-in Hybrid Search:** Native schema-rich vector store combining
sparse keyword matching (BM25) with dense vector embeddings natively out of
the box, improving retrieval precision for exact terms like product serial
numbers or code functions.
* **Multi-Modal Vector Spaces:** Supports joint text-and-image vector
spaces natively, enabling retrieval of technical diagrams, wireframes, or
charts alongside standard Markdown text.
* **Best Used For:** Document corpora containing exact codes, SKU numbers,
or multi-modal assets like images and PDFs.

### Chroma Optimization: Embedded Local Prototyping
* **Zero-Cloud Friction:** Operates embedded in-memory or on local disk
without external cloud API dependencies.
* **Rapid Sandboxing:** Allows local testing of custom chunking strategies,
metadata tag structures, and reranking logic before pushing to production.
* **Best Used For:** Local development, offline testing, and lightweight
prototyping of Sim agent workflows. ## 4. Architectural Summary Matrix

| Vector Store | Engine Type / Role | Primary Optimization for Sim.ai |
Ideal Deployment Use Case |
| :--- | :--- | :--- | :--- |
| **`pgvector`** | Native PostgreSQL extension | Integrated default vector
engine with RRF hybrid search | Default Sim Cloud & local Compose setups |
| **Qdrant** | High-performance Rust-based store | Single-stage payload
filtering & memory quantization | High-speed, tag-heavy routing &
enterprise filtering |
| **Pinecone** | Managed cloud vector search | Fully serverless elasticity
& multi-tenant namespace isolation | Large enterprise scale, SOC2
compliance & multi-tenancy |
| **Weaviate** | Schema-rich vector store | Native BM25 + dense hybrid
search & multi-modal support | Keyword-dense technical documents, code &
image retrieval |
| **Chroma** | Embedded local store | Lightweight in-memory or on-disk
storage | Local testing and rapid workflow prototyping |
