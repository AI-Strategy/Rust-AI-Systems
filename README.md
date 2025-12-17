# Rust-AI-Systems
An Ontology-Driven development assistant. Reifies the codebase into a Semantic Network to enable Tri-Brid Retrieval (Vector + Graph + Cluster). Solves memory loss by tracking the evolution of architectural intent alongside the raw code.


Rust AI Systems: The Digital Brain

Rust AI Systems is an open-source initiative to build a state-aware coding assistant that transcends the limitations of traditional RAG. By treating the Rust codebase as a strict Knowledge Graph (mirroring the compiler's HIR/MIR) rather than flat text, we eliminate hallucinations and "Long Session Amnesia."
Core Architecture

    🧠 The Digital Brain: A Neo4j-backed knowledge graph that models strict Rust relationships (Type → Trait → Implementation) to enforce safety guarantees.

    ⚡ Tri-Brid Retrieval: Combines Vector Search (Semantics), Graph Traversal (Logic/Safety), and Community Clustering (Architectural Intent) for high-fidelity context.

    🦛 Hippocampus Layer: An asynchronous memory worker that processes chat logs in the background, converting ephemeral interactions into persistent "Decisions" and "Constraints" without blocking the user.

Technology Stack

    Language: Rust (Axum, rust-analyzer, neo4rs)

    Memory: Neo4j Aura (Graph + Vector)

    Reasoning: Gemini 3.0 Pro (1M+ Token Context)

    Infrastructure: Google Cloud Platform (Cloud Run, Vertex AI)

    Component,Version,License,Purpose

The Core Stack (High-Level BOM)

Rust,stable (1.75+),MIT/Apache-2.0,Core language for backend logic.
Axum,0.7,MIT,Asynchronous web framework (Tokio-based).
Neo4j,5.x (Aura),Commercial/GPL,Graph Database & Vector Search Engine.
Tokio,1.x,MIT,Async runtime for high-concurrency I/O.
Google Cloud SDK,latest,Apache-2.0,Hosting (Cloud Run) & AI (Vertex).
VS Code API,^1.85.0,MIT,Editor integration framework.
