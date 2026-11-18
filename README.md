# Reyu AI

A private, free AI chat that runs on your own computer. No API key, no account, no cost.

## Quick start

1. Install [Ollama](https://ollama.com).
2. Download a model once:
   ```
   ollama pull llama3.2
   ```
3. Allow the page to talk to Ollama, then start it:
   ```
   # macOS / Linux
   OLLAMA_ORIGINS="*" ollama serve

   # Windows (PowerShell)
   $env:OLLAMA_ORIGINS="*"; ollama serve
   ```
4. Open `index.html` in your browser.

## Put it on GitHub

```
git init
git add .
git commit -m "Add Reyu AI"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/reyu-ai.git
git push -u origin main
```

To host it as a web page: **Settings → Pages → Deploy from branch → main**.
Visitors will still need Ollama running on their own computer.
Replace `*` in `OLLAMA_ORIGINS` with `https://YOUR-USERNAME.github.io` to be stricter.

## Make it stronger

- Bigger models answer better: `ollama pull qwen2.5:14b` (needs more RAM/GPU).
- Edit the `SYSTEM` text in `index.html` to change Reyu’s personality.
