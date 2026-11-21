# BadaLedger_open
A simple way to open specific Claude chats from BadaLedger directly.

A one-file "bounce" page for BadaLedger's chat buttons. The repository and the page GitHub Pages serves from it are both public, so anyone can read them.

**What it does:** opened as `https://badalao.github.io/BadaLedger_open/#chat/<id>` (or `#project/<id>`), it sends you on to that Claude chat or project. On a computer it opens the Claude desktop app (`claude://claude.ai/...`); on a phone it opens `https://claude.ai/...`. The Claude desktop app won't open `claude://` links from inside a page, but it does open them from the browser, which is why this page exists.

**What it reads:** only the part of its own address after `#`, which browsers never send to the server. The id must be a UUID; anything else shows "Invalid link" and does nothing. It loads no scripts, fonts or analytics, is not indexed, and sends no referrer.

**Rules:**
- This repository must never contain any data: no chat ids, reports, notes, logs, holdings or anything else from BadaLedger. Only `index.html` and this README.
- Chat ids arrive in the address when the page is used; they are never stored here.
- BadaLedger itself lives in a separate, private repository.
