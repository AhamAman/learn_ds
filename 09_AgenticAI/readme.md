# Agentic AI & LangChain/RAG Mastery Checklists

> A complete, phase-by-phase learning roadmap covering Agentic AI systems and LangChain/RAG pipelines — from foundations to production-grade deployment.

---

## Table of Contents

1. [Agentic AI](#1-agentic-ai)
2. [LangChain & RAG](#2-langchain--rag)

---

# 1. Agentic AI

*From Beginner → Master → Production-Grade AI Agents*

---

## Phase 0: Prerequisites

### AI Foundations

- [ ] What is AI?
- [ ] What is Machine Learning?
- [ ] What is Deep Learning?
- [ ] What is NLP?
- [ ] What are LLMs?

### LLM Foundations

- [ ] Transformers
- [ ] Attention Mechanism
- [ ] Tokenization
- [ ] Embeddings
- [ ] Context Windows
- [ ] Inference

### Python

- [ ] Functions & Classes
- [ ] Async Programming
- [ ] APIs & JSON
- [ ] Error Handling
- [ ] Virtual Environments
- [ ] Type Hints

### System Design Basics

- [ ] Client-Server Architecture
- [ ] Databases (SQL + NoSQL basics)
- [ ] REST APIs
- [ ] Queues & Event-Driven Systems

---

## Phase 1: Understanding Agentic AI

### What is an Agent?

- [ ] Definition of an AI Agent
- [ ] Difference between a chatbot and an agent
- [ ] Autonomous decision making
- [ ] Goal-oriented behavior

### Agent Characteristics

- [ ] Reasoning
- [ ] Planning
- [ ] Memory
- [ ] Tool Usage
- [ ] Reflection
- [ ] Learning

### Agent Lifecycle

- [ ] Receive goal
- [ ] Analyze task
- [ ] Plan actions
- [ ] Use tools
- [ ] Observe results
- [ ] Adjust strategy
- [ ] Produce output

### Understand

- [ ] Why traditional software can't do what agents do
- [ ] Where agents succeed vs fail today
- [ ] Real-world agent examples (Devin, AutoGPT, GitHub Copilot Workspace)

---

## Phase 2: Core Components of Agents

### LLM as Brain

- [ ] Prompt processing
- [ ] Reasoning
- [ ] Decision generation

### Tools

**External Tools**
- [ ] Search APIs
- [ ] Calculator
- [ ] Database access
- [ ] Web browsing
- [ ] Code execution
- [ ] File system access
- [ ] Email / Calendar APIs

### Memory

**Short-Term Memory**
- [ ] Context window
- [ ] Conversation history

**Long-Term Memory**
- [ ] Vector databases
- [ ] Knowledge storage
- [ ] Retrieval systems

### Understand

- [ ] Which component handles what
- [ ] How components interact at runtime
- [ ] What happens when a component fails

---

## Phase 3: Prompt Engineering for Agents

### Foundations

- [ ] Zero-shot prompting
- [ ] Few-shot prompting
- [ ] Role prompting
- [ ] System vs user prompts

### Agent-Oriented Prompting

- [ ] Goal specification
- [ ] Constraints definition
- [ ] Tool instructions
- [ ] Planning prompts
- [ ] Output format specification

### Advanced Prompting

- [ ] ReAct pattern
- [ ] Self-reflection prompts
- [ ] Multi-step reasoning
- [ ] Chain-of-thought prompting
- [ ] Step-back prompting

### Understand

- [ ] Why prompt quality is critical for agents
- [ ] Common prompt failure modes
- [ ] How to debug bad agent behavior via prompts

---

## Phase 4: Agent Reasoning

### Chain of Thought

- [ ] Step-by-step reasoning
- [ ] Intermediate thinking
- [ ] Scratchpad approach

### ReAct Framework

- [ ] Thought
- [ ] Action
- [ ] Observation
- [ ] Full loop trace

### Reflection

- [ ] Self-evaluation
- [ ] Error detection
- [ ] Retry strategies
- [ ] Critique-and-revise patterns

### Understand

- [ ] When reasoning helps vs hurts (latency, cost)
- [ ] How to evaluate reasoning quality
- [ ] Reasoning vs hallucination

---

## Phase 5: Planning Systems

### Why Planning Matters

- [ ] Goal decomposition
- [ ] Task sequencing
- [ ] Dependency handling

### Planning Methods

**Simple Planning**
- [ ] Task lists
- [ ] Sequential plans

**Advanced Planning**
- [ ] Tree of Thoughts
- [ ] Graph of Thoughts
- [ ] Search-based planning
- [ ] MCTS (Monte Carlo Tree Search) intuition

### Deep Dive

- [ ] Planning vs reasoning (difference)
- [ ] Dynamic replanning
- [ ] Failure recovery
- [ ] When plans break and how to recover

---

## Phase 6: Memory Systems

### Working Memory

- [ ] Session memory
- [ ] Conversation context

### Episodic Memory

- [ ] Past actions
- [ ] Previous experiences
- [ ] Event logging

### Semantic Memory

- [ ] Facts
- [ ] Knowledge base
- [ ] Structured knowledge stores

### Procedural Memory

- [ ] How-to knowledge
- [ ] Skill memory
- [ ] Reusable task templates

### Retrieval-Augmented Memory

- [ ] Embeddings
- [ ] Similarity search
- [ ] Vector databases

### Tools

- [ ] FAISS
- [ ] ChromaDB
- [ ] Pinecone
- [ ] Weaviate
- [ ] Zep (agent memory)
- [ ] Mem0

### Understand

- [ ] Memory vs context window
- [ ] When to use each memory type
- [ ] Memory compression strategies

---

## Phase 7: Tool Use

### Understanding Tool Calling

- [ ] Function calling
- [ ] Structured outputs
- [ ] Tool schemas (JSON Schema)
- [ ] Tool definitions

### Tool Categories

**Information Retrieval**
- [ ] Web search
- [ ] Internal knowledge base
- [ ] Document lookup

**Computation**
- [ ] Calculators
- [ ] Python execution
- [ ] Data analysis tools

**Actions**
- [ ] Sending emails
- [ ] Updating databases
- [ ] Scheduling tasks
- [ ] File creation/editing

**External Services**
- [ ] Slack, Notion, GitHub APIs
- [ ] CRM systems
- [ ] Payment / ticketing systems

### Deep Dive

- [ ] Tool selection logic
- [ ] Tool reliability & failure handling
- [ ] Parallel tool calling
- [ ] Tool chaining
- [ ] Building custom tools

---

## Phase 8: RAG for Agents

### Retrieval Augmented Generation

- [ ] Why RAG exists
- [ ] LLM knowledge limitations
- [ ] Static vs dynamic knowledge

### Pipeline

- [ ] Document ingestion
- [ ] Chunking
- [ ] Embedding generation
- [ ] Storage in vector DB
- [ ] Retrieval
- [ ] Context injection

### Advanced RAG

- [ ] Hybrid search
- [ ] Reranking
- [ ] Agentic RAG (agent decides when/what to retrieve)
- [ ] Multi-hop retrieval

---

## Phase 9: Agent Frameworks

### LangChain

- [ ] Chains
- [ ] Agents
- [ ] Tools
- [ ] Memory
- [ ] LCEL (LangChain Expression Language)

### LangGraph

- [ ] Nodes
- [ ] Edges
- [ ] State machines
- [ ] Conditional routing

### CrewAI

- [ ] Roles & personas
- [ ] Agent collaboration
- [ ] Task delegation

### AutoGen

- [ ] Multi-agent conversations
- [ ] Human-in-the-loop

### OpenAI Agents SDK

- [ ] Agent architecture
- [ ] Tool integration
- [ ] Handoffs between agents

### Understand

- [ ] When to use which framework
- [ ] Framework tradeoffs (flexibility vs abstraction)
- [ ] When to go framework-free

---

## Phase 10: Multi-Agent Systems

### Why Multiple Agents?

- [ ] Specialization
- [ ] Parallel execution
- [ ] Scalability
- [ ] Separation of concerns

### Architectures

**Supervisor Model**
- [ ] Manager agent
- [ ] Worker agents
- [ ] Task delegation

**Peer-to-Peer**
- [ ] Agent collaboration
- [ ] Negotiation protocols

**Hierarchical Systems**
- [ ] Multi-level planning
- [ ] Sub-agent orchestration

**Pipeline / Sequential**
- [ ] Output of one agent → input of next

### Challenges

- [ ] Coordination
- [ ] Communication protocols
- [ ] Conflict resolution
- [ ] Avoiding redundant work
- [ ] Shared state management

---

## Phase 11: Agent Workflows

### Research Agent

- [ ] Search
- [ ] Summarization
- [ ] Citation generation
- [ ] Cross-source synthesis

### Coding Agent

- [ ] Code generation
- [ ] Testing
- [ ] Debugging
- [ ] Code review

### Customer Support Agent

- [ ] FAQ retrieval
- [ ] Ticket handling
- [ ] Escalation logic

### Data Analysis Agent

- [ ] Data loading
- [ ] Statistical analysis
- [ ] Chart generation
- [ ] Insight summarization

### Business Automation Agent

- [ ] Reporting
- [ ] Workflow automation
- [ ] Document generation

---

## Phase 12: Agent Evaluation

### Metrics

- [ ] Task success rate
- [ ] Tool use accuracy
- [ ] Planning quality
- [ ] Hallucination rate
- [ ] Latency per task
- [ ] Cost per task

### Testing

- [ ] Unit testing (individual tools)
- [ ] Integration testing (full agent loop)
- [ ] Simulation testing
- [ ] Adversarial testing

### Benchmarking

- [ ] AgentBench
- [ ] GAIA
- [ ] SWE-Bench
- [ ] WebArena
- [ ] ToolBench

### Understand

- [ ] Why agent evaluation is hard
- [ ] Human vs automatic evaluation
- [ ] Evaluation vs monitoring

---

## Phase 13: Agent Security

### Risks

- [ ] Prompt injection
- [ ] Data leakage
- [ ] Tool abuse
- [ ] Unauthorized actions
- [ ] Indirect prompt injection (via retrieved content)

### Mitigations

- [ ] Sandboxing
- [ ] Permission systems
- [ ] Input/output validation layers
- [ ] Principle of least privilege
- [ ] Human-in-the-loop checkpoints

### Understand

- [ ] Why agents are harder to secure than chatbots
- [ ] Real-world agent attack vectors

---

## Phase 14: Production Agent Systems

### Reliability

- [ ] Retries with backoff
- [ ] Fallback models
- [ ] Circuit breakers
- [ ] Timeout handling
- [ ] Graceful degradation

### Monitoring

- [ ] Logging (structured)
- [ ] Tracing (LangSmith, OpenTelemetry)
- [ ] Observability dashboards
- [ ] Alert systems

### Scalability

- [ ] Distributed agents
- [ ] Queue systems (Celery, RabbitMQ, Kafka)
- [ ] Async execution
- [ ] Horizontal scaling

### Cost Management

- [ ] Token usage tracking
- [ ] Model tier selection
- [ ] Caching LLM responses
- [ ] Prompt compression

---

## Phase 15: Agent Internals

### Agent Loop

- [ ] Observe
- [ ] Think
- [ ] Plan
- [ ] Act
- [ ] Reflect

### State Management

- [ ] Agent state
- [ ] Memory state
- [ ] Workflow state
- [ ] Checkpointing

### Context Engineering

- [ ] Prompt assembly
- [ ] Context pruning
- [ ] Context retrieval
- [ ] Token budget management

---

## Phase 16: Human-in-the-Loop

### Why It Matters

- [ ] Safety in high-stakes decisions
- [ ] Trust building
- [ ] Handling ambiguous instructions

### Patterns

- [ ] Approval before action
- [ ] Interrupt and ask
- [ ] Review and correct output
- [ ] Collaborative refinement

### Understand

- [ ] When to automate fully vs involve humans
- [ ] How to design good interruption UX

---

## Phase 17: Research-Level Agentic AI

### Foundational Papers

- [ ] ReAct (Yao et al.)
- [ ] Reflexion
- [ ] Tree of Thoughts
- [ ] Voyager (Minecraft agent)
- [ ] AutoGPT
- [ ] BabyAGI
- [ ] Generative Agents (Stanford)

### Advanced Topics

- [ ] Self-improving agents
- [ ] Autonomous learning
- [ ] Agent societies
- [ ] Long-horizon planning
- [ ] World models for agents

---

## Projects

### Beginner

- [ ] Calculator Agent
- [ ] Weather Agent
- [ ] FAQ Agent

### Intermediate

- [ ] RAG Agent
- [ ] Research Assistant
- [ ] PDF Chatbot
- [ ] Web Scraping Agent

### Advanced

- [ ] Coding Agent
- [ ] Autonomous Research Agent
- [ ] Business Workflow Agent
- [ ] Data Analysis Agent

### Expert

- [ ] Multi-Agent Team
- [ ] Autonomous Software Engineer
- [ ] AI Project Manager
- [ ] End-to-End Enterprise Agent Platform

---

## Final Mastery

### Theory

- [ ] Explain Agentic AI from first principles
- [ ] Explain planning systems
- [ ] Explain memory architectures
- [ ] Explain multi-agent coordination

### Practical

- [ ] Build single-agent systems
- [ ] Build RAG agents
- [ ] Build multi-agent workflows
- [ ] Deploy production agents

### Internals

- [ ] Explain ReAct loop
- [ ] Explain tool calling internals
- [ ] Explain agent state management
- [ ] Explain context engineering

### Expert

- [ ] Design enterprise agent architecture
- [ ] Build autonomous workflows
- [ ] Evaluate agent reliability
- [ ] Optimize agent performance
- [ ] Manage agent cost at scale

---

## True Master Level

- [ ] Teach Agentic AI from first principles
- [ ] Build custom agent frameworks
- [ ] Design multi-agent ecosystems
- [ ] Deploy production-grade agents
- [ ] Contribute to agent frameworks (LangChain, CrewAI, etc.)
- [ ] Read and implement research papers
- [ ] Build autonomous AI systems
- [ ] Lead Agentic AI projects end-to-end

---

# 2. LangChain & RAG

*From Beginner → Production → Advanced Agentic RAG*

---

## Phase 0: Prerequisites

### Python

- [ ] Functions & Classes
- [ ] Modules & Virtual Environments
- [ ] Async Programming
- [ ] APIs & JSON Handling
- [ ] Error Handling
- [ ] Type Hints

### AI Foundations

- [ ] Machine Learning overview
- [ ] Deep Learning basics
- [ ] NLP basics
- [ ] Transformers
- [ ] LLM Fundamentals
- [ ] Tokenization & Context Windows

### Databases

- [ ] SQL basics
- [ ] NoSQL basics
- [ ] Vector database concept

### API Concepts

- [ ] HTTP / REST APIs
- [ ] Authentication & API Keys
- [ ] Rate limiting & quotas

---

## Phase 1: Why RAG Exists

### LLM Limitations

- [ ] Hallucinations
- [ ] Knowledge cutoff
- [ ] Context window limitations
- [ ] No organization-specific knowledge
- [ ] No real-time information

### Traditional Solutions & Their Problems

- [ ] Fine-tuning: expensive, requires retraining, knowledge goes stale
- [ ] Knowledge retraining: high cost and complexity

### RAG Solution

- [ ] External knowledge retrieval at inference time
- [ ] Dynamic context injection
- [ ] Reduced hallucinations
- [ ] Always up-to-date knowledge

### Understand

- [ ] When RAG is the right choice vs fine-tuning
- [ ] RAG vs long-context models
- [ ] RAG limitations

---

## Phase 2: RAG Architecture Overview

### Complete Pipeline

```
Documents
    ↓
Chunking
    ↓
Embeddings
    ↓
Vector Database
    ↓
Query → Retriever
    ↓
Context + Question
    ↓
LLM
    ↓
Answer
```

### Two Phases

**Indexing Phase (offline)**
- [ ] Load → Chunk → Embed → Store

**Retrieval Phase (online)**
- [ ] Query → Retrieve → Inject → Generate

---

## Phase 3: LangChain Fundamentals

### What is LangChain?

- [ ] Purpose: composable LLM application framework
- [ ] Architecture overview
- [ ] Ecosystem: LangChain, LangGraph, LangSmith

### Core Components

**Models**
- [ ] Chat Models (GPT-4, Claude, Gemini)
- [ ] LLM Interfaces
- [ ] Embedding Models

**Prompts**
- [ ] Prompt Templates
- [ ] Dynamic Variables
- [ ] Chat Prompt Templates

**Output Parsers**
- [ ] Structured outputs
- [ ] JSON outputs
- [ ] Pydantic parsers

**Chains**
- [ ] Sequential execution
- [ ] Chained workflows

**Runnables (LCEL)**
- [ ] Runnable interface
- [ ] Runnable sequences (`|` operator)
- [ ] Runnable parallel
- [ ] Runnable passthrough

### Understand

- [ ] Why LCEL replaced legacy chains
- [ ] Composability pattern
- [ ] Streaming with LCEL

---

## Phase 4: Document Loading

### Document Loaders

**Files**
- [ ] TXT / PDF / DOCX / CSV / JSON
- [ ] Excel / PowerPoint

**Websites**
- [ ] HTML pages
- [ ] Documentation sites
- [ ] Web scrapers (BeautifulSoup, Playwright)

**External Sources**
- [ ] Databases
- [ ] APIs (Notion, Confluence, SharePoint)
- [ ] YouTube transcripts
- [ ] GitHub repositories

### Deep Dive

- [ ] Metadata handling
- [ ] Source tracking
- [ ] Handling large files
- [ ] Encoding issues

---

## Phase 5: Text Splitting (Chunking)

### Why Chunking Exists

- [ ] Context limits
- [ ] Retrieval efficiency
- [ ] Granularity vs completeness tradeoff

### Chunking Methods

**Fixed Chunking**
- [ ] Character splitting
- [ ] Token splitting

**Recursive Chunking**
- [ ] RecursiveCharacterTextSplitter (most common)
- [ ] Respects natural document structure

**Semantic Chunking**
- [ ] Meaning-based splitting
- [ ] Embedding-based boundaries

**Document-Specific Chunking**
- [ ] Markdown splitter
- [ ] Code splitter
- [ ] HTML splitter

### Parameters

- [ ] Chunk size
- [ ] Chunk overlap

### Deep Dive

- [ ] Retrieval precision vs recall tradeoff
- [ ] Small-to-big chunking strategy
- [ ] Sliding window approach
- [ ] How bad chunking ruins RAG quality

---

## Phase 6: Embeddings

### What are Embeddings?

- [ ] Vector representations of text
- [ ] Semantic similarity concept
- [ ] High-dimensional space intuition

### Embedding Models

**Proprietary**
- [ ] OpenAI text-embedding-3-small / large
- [ ] Cohere Embed

**Open Source**
- [ ] Sentence Transformers
- [ ] BGE (BAAI)
- [ ] E5
- [ ] Nomic Embed

### Deep Dive

- [ ] Embedding dimensions
- [ ] Cosine similarity
- [ ] Euclidean distance
- [ ] Dot product
- [ ] How to choose an embedding model
- [ ] MTEB leaderboard

### Understand

- [ ] Same model must embed both documents and queries
- [ ] Embedding drift over time
- [ ] Multilingual embeddings

---

## Phase 7: Vector Databases

### Why Vector Databases?

- [ ] Fast similarity search at scale
- [ ] Scalable retrieval
- [ ] Metadata filtering alongside vectors

### Vector Stores

**Local / Beginner**
- [ ] FAISS
- [ ] ChromaDB

**Production**
- [ ] Pinecone
- [ ] Weaviate
- [ ] Qdrant
- [ ] Milvus
- [ ] pgvector (Postgres extension)

### Concepts

- [ ] Indexing
- [ ] Similarity search (Top-K)
- [ ] Metadata filtering
- [ ] Namespaces / collections

### Deep Dive

- [ ] ANN (Approximate Nearest Neighbor) search
- [ ] HNSW algorithm
- [ ] IVF indexes
- [ ] Product Quantization
- [ ] Tradeoffs: speed vs accuracy vs memory

---

## Phase 8: Retrieval Systems

### Retrieval Basics

- [ ] Similarity retrieval
- [ ] Top-K retrieval
- [ ] Similarity threshold filtering

### Search Types

**Dense Retrieval**
- [ ] Embedding-based search
- [ ] Semantic understanding

**Sparse Retrieval**
- [ ] BM25 (keyword-based)
- [ ] TF-IDF

**Hybrid Retrieval**
- [ ] Dense + Sparse combination
- [ ] Reciprocal Rank Fusion (RRF)

### Advanced Retrieval

- [ ] Parent document retrieval
- [ ] Multi-query retrieval
- [ ] Self-query retrieval
- [ ] Contextual compression
- [ ] MMR (Maximal Marginal Relevance) for diversity

---

## Phase 9: Building Your First RAG Pipeline

### Step-by-Step

1. [ ] Load documents
2. [ ] Split into chunks
3. [ ] Generate embeddings
4. [ ] Store in vector database
5. [ ] Retrieve relevant chunks on query
6. [ ] Inject context into prompt
7. [ ] Generate answer via LLM

### Understand

- [ ] How to test each step independently
- [ ] Common failure points at each step
- [ ] How to inspect retrieved chunks

---

## Phase 10: Prompt Engineering for RAG

### Prompt Templates

- [ ] Context injection placeholder
- [ ] Question insertion
- [ ] System instructions

### Guardrails

- [ ] Answer only from provided context
- [ ] Gracefully say "I don't know"
- [ ] Avoid hallucinating beyond context

### Citation Prompts

- [ ] Source attribution
- [ ] Reference generation
- [ ] Inline citations

### Understand

- [ ] How prompt quality affects answer quality
- [ ] How to format context for clarity
- [ ] Stuffing vs map-reduce vs refine strategies for long docs

---

## Phase 11: Advanced Retrieval Techniques

### Query Expansion

- [ ] Multi-query generation (generate multiple phrasings)

### Query Rewriting

- [ ] Rewrite query for better search results

### HyDE (Hypothetical Document Embeddings)

- [ ] Generate a hypothetical answer, embed it, search with it

### Contextual Retrieval

- [ ] Metadata-aware retrieval
- [ ] Date / source / category filtering

### Step-Back Prompting

- [ ] Abstract the question before retrieval

---

## Phase 12: Reranking

### Why Reranking?

- [ ] Initial retrieval is approximate; reranking improves precision
- [ ] Two-stage retrieval: recall first, precision second

### Models

- [ ] Cross-Encoders (slower but more accurate)
- [ ] Cohere Rerank API
- [ ] BGE Reranker
- [ ] FlashRank (lightweight)

### Deep Dive

- [ ] Bi-encoder (retriever) vs cross-encoder (reranker)
- [ ] When reranking is worth the latency cost

---

## Phase 13: Advanced RAG Patterns

### Parent-Child Retrieval

- [ ] Store large parent chunks
- [ ] Retrieve small child chunks
- [ ] Return parent for context

### Multi-Hop RAG

- [ ] Multiple sequential retrieval cycles
- [ ] Each hop answers a sub-question

### Graph RAG

- [ ] Knowledge graphs
- [ ] Relationship-aware retrieval
- [ ] Microsoft GraphRAG

### Agentic RAG

- [ ] Agent decides when and what to retrieve
- [ ] Dynamic search planning
- [ ] Self-correcting retrieval

### Corrective RAG (CRAG)

- [ ] Evaluate retrieved docs
- [ ] Fall back to web search if docs are irrelevant

### Self-RAG

- [ ] LLM decides whether to retrieve at all
- [ ] Reflection tokens for self-evaluation

---

## Phase 14: LangChain Chains & LCEL

### Retrieval Chains

- [ ] RetrievalQA (legacy)
- [ ] Modern LCEL retrieval chain

### Custom Chains

- [ ] RunnableSequence
- [ ] RunnableParallel
- [ ] RunnablePassthrough

### LCEL Patterns

- [ ] Streaming responses
- [ ] Batching
- [ ] Async execution
- [ ] Fallback chains

### Understand

- [ ] Why LCEL enables streaming natively
- [ ] Composing complex pipelines

---

## Phase 15: Memory in RAG Systems

### Conversation Memory

- [ ] Chat history management
- [ ] Condensing history for long conversations

### Long-Term Memory

- [ ] User preferences
- [ ] Persistent memory across sessions
- [ ] Mem0 / Zep integration

### Retrieval Memory

- [ ] Semantic memory systems
- [ ] Storing and retrieving past interactions

### Understand

- [ ] Memory vs context window
- [ ] When to summarize vs keep full history

---

## Phase 16: LangGraph

### Why LangGraph?

- [ ] Complex, stateful workflows
- [ ] Loops and conditional branching
- [ ] State management across steps

### Core Concepts

- [ ] Nodes (processing steps)
- [ ] Edges (transitions)
- [ ] State (shared data)
- [ ] Checkpointing

### Workflow Design

- [ ] Conditional routing
- [ ] Loops and retries
- [ ] Error recovery
- [ ] Human-in-the-loop nodes

### Use Cases

- [ ] RAG with reflection
- [ ] Self-correcting pipelines
- [ ] Multi-agent orchestration

---

## Phase 17: Evaluation

### Retrieval Metrics

- [ ] Recall @ K
- [ ] Precision @ K
- [ ] MRR (Mean Reciprocal Rank)
- [ ] NDCG

### Generation Metrics

- [ ] Faithfulness (answer grounded in context?)
- [ ] Answer relevance (answers the question?)
- [ ] Context relevance (retrieved chunks useful?)

### End-to-End Metrics

- [ ] Answer correctness
- [ ] Hallucination rate

### Tools

- [ ] RAGAS
- [ ] TruLens
- [ ] LangSmith
- [ ] DeepEval

### Understand

- [ ] Why RAG evaluation is hard
- [ ] Building a golden evaluation dataset
- [ ] Continuous evaluation in production

---

## Phase 18: Production RAG

### Scaling

- [ ] Large document collections (millions of chunks)
- [ ] Distributed vector databases
- [ ] Batch embedding pipelines

### Observability

- [ ] Structured logging
- [ ] LangSmith tracing
- [ ] OpenTelemetry integration
- [ ] Monitoring dashboards

### Reliability

- [ ] Retry strategies with backoff
- [ ] Fallback models
- [ ] Graceful degradation
- [ ] Cache frequent queries

### Cost Optimization

- [ ] Embedding caching
- [ ] Query result caching
- [ ] Choosing cost-effective models
- [ ] Token budget management

---

## Phase 19: Security

### Risks

- [ ] Prompt injection (direct and indirect)
- [ ] Data leakage via retrieval
- [ ] Sensitive document exposure

### Solutions

- [ ] Input validation
- [ ] Output filtering
- [ ] Permission-based retrieval (user can only access their data)
- [ ] Document-level access control
- [ ] Namespace isolation in vector DBs

---

## Phase 20: Open Source Ecosystem

### Frameworks

- [ ] LangChain
- [ ] LangGraph
- [ ] LlamaIndex
- [ ] Haystack
- [ ] DSPy (programmatic prompting)

### Vector Databases

- [ ] ChromaDB (local)
- [ ] FAISS (local)
- [ ] Pinecone (cloud)
- [ ] Weaviate (cloud/local)
- [ ] Qdrant (cloud/local)
- [ ] pgvector (Postgres)

### Embedding Models

- [ ] OpenAI
- [ ] Cohere
- [ ] Sentence Transformers (HuggingFace)

### Observability

- [ ] LangSmith
- [ ] Phoenix (Arize)
- [ ] TruLens

---

## Phase 21: Build Projects

### Beginner

- [ ] PDF Question Answering
- [ ] Company FAQ Bot
- [ ] Resume Chatbot

### Intermediate

- [ ] Multi-PDF RAG
- [ ] Research Assistant
- [ ] Documentation Chatbot
- [ ] YouTube Video Q&A

### Advanced

- [ ] Agentic RAG system
- [ ] Graph RAG
- [ ] Multi-Agent Knowledge Assistant
- [ ] Corrective RAG (CRAG) pipeline

### Expert

- [ ] Enterprise RAG Platform
- [ ] Autonomous Research Agent
- [ ] Internal Company Knowledge System
- [ ] Multi-tenant RAG with access control

---

## Phase 22: Deep Internals

### Embedding Internals

- [ ] Transformer embeddings (CLS token, mean pooling)
- [ ] Vector generation pipeline
- [ ] Embedding normalization

### ANN Search Internals

- [ ] HNSW (Hierarchical Navigable Small World)
- [ ] IVF (Inverted File Index)
- [ ] Product Quantization
- [ ] Tradeoffs: recall vs speed vs memory

### Retrieval Mathematics

- [ ] Cosine similarity
- [ ] Euclidean distance
- [ ] Dot product
- [ ] When each metric applies

### LangChain Internals

- [ ] Runnable architecture
- [ ] Execution graph
- [ ] Callback systems
- [ ] Streaming internals

---

## Phase 23: Research-Level Knowledge

### Foundational Papers

- [ ] RAG (Lewis et al., Facebook)
- [ ] DPR (Dense Passage Retrieval)
- [ ] ColBERT
- [ ] HyDE
- [ ] GraphRAG (Microsoft)
- [ ] Self-RAG
- [ ] CRAG (Corrective RAG)

### Modern Topics

- [ ] Long-context models vs RAG
- [ ] Agentic retrieval
- [ ] Self-improving RAG
- [ ] Multimodal RAG (images, tables)

---

## Final Mastery

### Theory

- [ ] Explain RAG from first principles
- [ ] Explain embeddings mathematically
- [ ] Explain ANN search
- [ ] Explain chunking tradeoffs

### Practical

- [ ] Build RAG from scratch (no framework)
- [ ] Build Agentic RAG
- [ ] Deploy production RAG system
- [ ] Evaluate RAG quality rigorously

### Internals

- [ ] Explain HNSW internals
- [ ] Explain vector database indexing
- [ ] Explain retrieval ranking math

### Expert

- [ ] Design enterprise RAG architecture
- [ ] Optimize retrieval quality end-to-end
- [ ] Build multi-tenant RAG with access control
- [ ] Evaluate and improve RAG systems continuously

---

## True Master Level

- [ ] Build LangChain alternatives from scratch
- [ ] Build a custom vector database
- [ ] Build a custom retrieval engine
- [ ] Design Agentic RAG platforms
- [ ] Reproduce retrieval research papers
- [ ] Contribute to LangChain / LlamaIndex ecosystem
- [ ] Lead production AI platform development
- [ ] Teach RAG and LangChain from first principles