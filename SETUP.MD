uv venv
uv pip install -r requirements.txt

pnpm i

ollama --version
ollama pull qwen3:0.6b
ollama pull qwen3:8b
ollama serve

python run_system.py
python run_system.py --mode dev
open http://localhost:3000

python system_health_check.py
python -c "from backend.database import ChatDatabase; ChatDatabase().init_database()"
python -c "from rag_system.main import get_agent; print('✅ Installation successful!')"

python run_system.py --health
