# Trading Action Extraction Agent

An agentic application that extracts trading actions (buy/sell, stock symbols, prices) from expert messages in Discord/Telegram channels, with initial testing support via PDF message extraction.

## Project Structure

```
follow_trader/
├── src/
│   ├── platforms/      # Platform adapters (PDF, Discord, Telegram)
│   ├── extractors/     # Trading action extraction logic
│   ├── models/         # Data models (Message, TradingAction)
│   ├── storage/        # Database layer
│   ├── services/       # Business logic services
│   └── ui/             # User interface (Streamlit dashboard)
├── config/             # Configuration files
├── tests/              # Unit tests
├── requirements.txt    # Python dependencies
└── main.py            # Application entry point (to be created)
```

## Setup Instructions

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Set up environment variables:**
   - Copy `.env.example` to `.env` (or create manually)
   - Add your LLM API key (OpenAI or Anthropic)

3. **Configure the application:**
   - Copy `config/config.yaml.example` to `config/config.yaml`
   - Update PDF file path and other settings as needed

## Development Status

Currently in Phase 1: Message Extraction Agent
- Step 1: ✅ Project structure setup (completed)

## Next Steps

- Step 2: Create data models (Message, TradingAction)
- Step 3: Implement PDF message reader
- Step 4: Build LLM-based extraction agent
- Step 5: Create monitoring dashboard

