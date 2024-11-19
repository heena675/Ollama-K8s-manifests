# Ollama-K8s-manifests
A private chatgpt solution.

Openweb UI image as used in frontend POD.
https://docs.openwebui.com/
To connect to Ollama on another server, change the OLLAMA_BASE_URL to the server's URL:
docker run -d -p 3000:8080 -e OLLAMA_BASE_URL=https://example.com -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main

Ollama image as used in backend POD.
ollama/ollama
Model	Parameters	Size	Download
Llama 3.2	1B	1.3GB	ollama run llama3.2:1b
