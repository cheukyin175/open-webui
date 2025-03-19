backend/
  ├── open_webui/              # Main backend package
  │   ├── config.py            # Configuration management
  │   ├── env.py               # Environment variable handling
  │   ├── main.py              # FastAPI application entry point
  │   ├── constants.py         # Constants used throughout the app
  │   ├── functions.py         # Utility functions
  │   ├── internal/            # Internal modules
  │   │   ├── db.py            # Database connection and management
  │   │   └── migrations/      # Database migration scripts
  │   ├── migrations/          # Alembic migrations
  │   │   └── versions/        # Migration version files
  │   ├── models/              # Database models
  │   │   ├── auths.py         # Authentication models
  │   │   ├── chats.py         # Chat models
  │   │   ├── messages.py      # Message models
  │   │   ├── users.py         # User models
  │   │   ├── prompts.py       # Prompt templates
  │   │   ├── functions.py     # Function models
  │   │   ├── files.py         # File models
  │   │   └── ...              # Other models
  │   ├── retrieval/           # RAG (Retrieval Augmented Generation)
  │   │   ├── loaders/         # Document loaders
  │   │   ├── models/          # Embedding models
  │   │   ├── vector/          # Vector storage
  │   │   │   ├── dbs/         # Vector database adapters
  │   │   │   │   ├── chroma.py # Chroma DB adapter
  │   │   │   │   ├── elasticsearch.py # Elasticsearch adapter
  │   │   │   │   ├── milvus.py # Milvus adapter
  │   │   │   │   ├── opensearch.py # OpenSearch adapter
  │   │   │   │   ├── pgvector.py # Postgres vector adapter
  │   │   │   │   └── qdrant.py # Qdrant adapter
  │   │   │   └── main.py      # Entry point for vector operations
  │   │   └── web/             # Web search modules
  │   │       ├── bing.py      # Bing search
  │   │       ├── google_pse.py # Google programmable search
  │   │       ├── searxng.py   # SearXNG integration
  │   │       └── ...          # Other search providers
  │   ├── routers/             # API routes
  │   │   ├── audio.py         # Audio endpoints (TTS/STT)
  │   │   ├── auths.py         # Authentication endpoints
  │   │   ├── chats.py         # Chat endpoints
  │   │   ├── configs.py       # Configuration endpoints
  │   │   ├── evaluations.py   # Model evaluation endpoints
  │   │   ├── files.py         # File management endpoints
  │   │   ├── folders.py       # Folder management endpoints
  │   │   ├── functions.py     # Function endpoints
  │   │   ├── images.py        # Image generation endpoints
  │   │   ├── models.py        # Model endpoints
  │   │   ├── ollama.py        # Ollama integration endpoints
  │   │   ├── openai.py        # OpenAI API integration endpoints
  │   │   ├── users.py         # User management endpoints
  │   │   └── ...              # Other API routes
  │   ├── socket/              # WebSocket implementation
  │   │   └── main.py          # WebSocket server
  │   ├── static/              # Static files
  │   ├── storage/             # Storage providers
  │   │   └── provider.py      # Storage provider implementation
  │   ├── test/                # Backend tests
  │   └── utils/               # Utility modules
  │       ├── auth.py          # Authentication utilities
  │       ├── chat.py          # Chat utilities
  │       ├── code_interpreter.py # Code execution utilities
  │       └── ...              # Other utilities
  └── requirements.txt         # Python dependencies





  src/
  ├── app.html               # Main HTML template
  ├── routes/                # SvelteKit routes
  │   ├── (app)/             # Authenticated app routes
  │   │   ├── admin/         # Admin panel routes
  │   │   ├── c/[id]/        # Chat routes
  │   │   ├── channels/      # Channels routes
  │   │   ├── home/          # Home page
  │   │   ├── playground/    # Playground routes
  │   │   └── workspace/     # Workspace routes
  │   ├── auth/              # Authentication routes
  │   ├── s/[id]/            # Shared content routes
  │   └── ...                # Other routes
  └── lib/                   # Library code
      ├── apis/              # API client modules
      │   ├── audio/         # Audio API client
      │   ├── auths/         # Authentication API client
      │   ├── chats/         # Chat API client
      │   ├── models/        # Models API client
      │   └── ...            # Other API clients
      ├── components/        # UI components
      │   ├── admin/         # Admin components
      │   ├── chat/          # Chat components
      │   ├── channel/       # Channel components
      │   ├── common/        # Shared components
      │   ├── icons/         # Icon components
      │   ├── layout/        # Layout components
      │   ├── playground/    # Playground components
      │   └── workspace/     # Workspace components
      ├── i18n/              # Internationalization
      │   └── locales/       # Language translations
      ├── pyodide/           # Python in browser integration
      ├── stores/            # Svelte stores
      ├── types/             # TypeScript type definitions
      ├── utils/             # Utility functions
      └── workers/           # Web workers