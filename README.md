# Anthropic Courses

A personal learning repository containing all notebooks from Anthropic's courses. Currently working through the **Building with the Claude API** course.

## 📚 Courses

### 🔵 Building with the Claude API — In Progress
Topics covered across the course:
- API fundamentals & authentication
- Single and multi-turn conversations
- System prompts & model configuration
- Prompt engineering & evaluation
- Tool use & structured outputs
- Retrieval-Augmented Generation (RAG)
- Prompt caching & streaming
- Model Context Protocol (MCP)
- Agentic workflows (parallelization, chaining, routing)

## 📁 Repository Structure
```
├── requests.ipynb               # Basic API requests — lesson
├── requests_exercise.ipynb      # Basic API requests — exercise
└── ...                          # More notebooks added as course progresses
```

## 🛠️ Setup

### Prerequisites
- VS Code with the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
- Python 3.8+

### Installation

1. Clone the repo
```bash
   git clone https://github.com/nikshep1/Anthropic-Courses.git
   cd Anthropic-Courses
```

2. Install dependencies
```bash
   pip install anthropic python-dotenv
```

3. Create a `.env` file in the root folder
```
   ANTHROPIC_API_KEY=your-api-key-here
```

4. Load it inside your notebooks
```python
   import os
   from dotenv import load_dotenv
   import anthropic

   load_dotenv()
   client = anthropic.Anthropic(api_key=os.environ.get("ANTHROPIC_API_KEY"))
```

> ⚠️ Never commit your `.env` file. Make sure `.env` is in your `.gitignore`.

## 🔗 Resources

- [Anthropic Academy](https://anthropic.skilljar.com/)
- [Claude API Docs](https://docs.anthropic.com/)
- [Anthropic GitHub Courses](https://github.com/anthropics/courses)
