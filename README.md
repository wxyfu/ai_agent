# Prepare the OCI ununtu env.
## Step 1. Install Docker (Minimal)
```bash
curl -fsSL https://get.docker.com | sudo sh
sudo usermod -aG docker ubuntu \
newgrp docker \
docker --version
```

## Step 2: Create RAG App (API-only LLM)
```bash
mkdir ~/api-rag && cd ~/api-rag
python3 -m venv venv
source venv/bin/activate
pip install langchain langchain-community langchain-groq \
            langchain-faiss langchain-text-splitters \
            fastapi uvicorn python-dotenv pypdf oci unstructured
pip freeze > requirements.txt
deactivate
```

## Step 3: Get FREE Groq API key: https://console.groq.com/keys → Create API key → copy.

## Step 4: 


