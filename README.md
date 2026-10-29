# Three-project workspace

A temporary, static launchpad for FreeLLMAPI, `free-claude-code`, and Hackthon. It keeps all
three repositories independent and does not copy source code, configure integrations, or replace
the Hackthon app.

## Run locally

From the repository root, run:

```powershell
python -m http.server 8000 --bind 127.0.0.1
```

Then open <http://localhost:8000>. Python's standard library is sufficient; there is no build step
or package installation.

## Project notes

- **FreeLLMAPI**: the local OpenAI-compatible endpoint is `http://localhost:3001/v1`. Use its
  repository's own README for starting the service and its own configuration for credentials.
- **free-claude-code**: use the repository's own README and configuration. The workspace does not
  contain that repository, so this hub does not make claims about its commands or compatibility.
  The page links to GitHub's repository search rather than guessing a repository owner.
- **Hackthon**: the repository linked from the page. This hub is only static navigation and setup
  guidance, not the Hackthon product.

The page makes no API calls. Never put an API key in the HTML, CSS, a URL, or a committed file.
Keep repositories in separate checkouts. A client can use the FreeLLMAPI endpoint only if that
client's own documented configuration supports it.

## Files

- `index.html` — the project hub
- `styles.css` — local page styling
