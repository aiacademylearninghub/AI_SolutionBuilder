# Solution Builder Server
Solution Builder Server is responsible for backend operations, providing APIs, business logic, and integration with LLMs for the Solution Builder application. It serves the frontend, processes user input, and generates architecture diagrams and code templates.

## Project File Documentation

### Server Folder (`server/`)

- **pyproject.toml**: Poetry configuration file; manages Python dependencies and project metadata.
- **poetry.lock**: Locked dependency versions for reproducible environments.
- **app/**
  - **main.py**: FastAPI application entry point; sets up middleware, routes, and static file serving.
  - **config.py**: Loads environment variables and configuration settings.
  - **api/v1/endpoints/solution_builder.py**: Defines API endpoints for question generation and code template retrieval.
  - **api/v1/models/solution_builder.py**: Pydantic models for request/response validation (e.g., SolutionBuilderRequest, SolutionBuilderResponse).
  - **functions/solution_builder.py**: Core backend logic for processing questions, formatting history, and handling code templates.
  - **llm/gemini.py**: Utility to instantiate the Gemini LLM using environment variables.
  - **prompts/solution_builder.py**: Contains prompt templates for the LLM to generate questions and architecture updates.
- **static/**: Serves static files for the frontend (copied from the client build).
  - **css/**, **js/**: Bundled frontend assets.
  - **decision_tree.json**: (if present) Backend copy of the decision tree.
  - **test-embeddings.pdf**, **favicon.ico**, **index.html**, **robots.txt**: Additional static assets.

---


# Solution Builder Server
Solution Builder Server is responsible for handling backend operations and providing APIs for the client application. Currently it is required only for AI enabled features.

## Setup
To setup the Solution Builder Server, follow these steps:
1. Navigate to the server directory
```cmd
cd server
```
2. Install dependencies
```cmd
poetry install
```
3. Run the server
```cmd
poetry run python app\main.py
```