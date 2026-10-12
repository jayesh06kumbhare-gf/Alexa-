# Alexa-
                  MOBILE PHONE
          ┌──────────────────────────┐
          │  Web App / PWA           │
          │  Microphone & Speaker    │
          │  Voice Input / Text Chat │
          └────────────┬─────────────┘
                       │
                 HTTPS / WebSocket
                       │
                       ▼
          ┌──────────────────────────┐
          │      LAPTOP SERVER       │
          │                          │
          │   Django Backend         │
          │   ├── REST API           │
          │   ├── Authentication     │
          │   ├── Chat Management    │
          │   └── Voice Orchestrator │
          │            │             │
          │            ▼             │
          │   Speech-to-Text (STT)   │
          │            │             │
          │            ▼             │
          │      RAG Pipeline        │
          │   ┌──────────────────┐   │
          │   │ Query Embedding  │   │
          │   │ Document Search  │   │
          │   │ Context Retrieval│   │
          │   └────────┬─────────┘   │
          │            ▼             │
          │       LLM Engine         │
          │            │             │
          │            ▼             │
          │    Text-to-Speech (TTS)  │
          └────────────┬─────────────┘
                       │
                       ▼
          ┌──────────────────────────┐
          │       PostgreSQL         │
          │                          │
          │  • User accounts         │
          │  • Chat history          │
          │  • Document metadata     │
          │  • Vector embeddings     │
          │    (using pgvector)      │
          └──────────────────────────┘
