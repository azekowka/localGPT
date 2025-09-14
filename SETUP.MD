uv venv
uv pip install -r requirements.txt

pnpm i

ollama --version
ollama pull qwen3:0.6b
ollama pull qwen3:8b
ollama serve

python run_system.py

open http://localhost:3000