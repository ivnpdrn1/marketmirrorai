# Event-Driven Market Forecasting (AWS Bedrock)

Goal: predict short-term SPY behavior based on **present events** by retrieving and comparing **historically similar events** (“analogs”).

## Core idea
1) Ingest current events (CPI, PPI, FOMC, Fed speakers, earnings, geopolitics) + market context (trend, vol, yields).
2) Retrieve similar historical events via **embeddings + vector search**.
3) Use **Bedrock LLM (Claude 3 Sonnet)** to reason over analogs and produce a **probabilistic forecast** (direction, magnitude, vol regime, confidence).
4) Validate with backtests and guardrails (no hallucinated events, enforce citations to dataset rows).

## Recommended Bedrock models
- **Primary reasoning LLM:** Anthropic Claude 3 Sonnet (best for multi-step comparisons and causal narratives)
- **Embeddings:** use a Bedrock embedding model + vector DB (OpenSearch Serverless, Aurora pgvector, Pinecone, etc.)

## Pipeline
- Data -> Event labeling -> Embeddings -> Similarity retrieval -> LLM forecast -> Quant evaluation

## Next steps
- Build event dataset (macro + news + labels)
- Implement vector retrieval
- Create forecast prompt with strict JSON output
- Backtest and calibrate
