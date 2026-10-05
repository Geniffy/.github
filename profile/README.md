<p align="center">
  <a href="https://geniffy.com"><img src="https://geniffy.com/brand/geniffy-lockup-ink.png" alt="Geniffy" height="44"></a>
</p>

<p align="center">
  <b>Memory for AI apps.</b> Every fact with the line it came from, and a plain "nothing stored" instead of a guess.
</p>

<p align="center">
  <a href="https://geniffy.com">Website</a> ·
  <a href="https://docs.geniffy.com">Docs</a> ·
  <a href="https://geniffy.com/app">Get a key</a> ·
  <a href="https://github.com/Geniffy/examples">Examples</a>
</p>

---

Geniffy gives each user of your app a memory. Write what they tell you, and before your model answers, put
what is known about them in front of it. Every memory keeps where it came from and when it was said, a newer
fact replaces an older one, and when nothing supports an answer Geniffy says so.

```bash
pip install geniffy        # or: npm install geniffy
```

```python
from geniffy import Geniffy

mem = Geniffy().space("customer_1042")             # one memory per user; no other space can read it

mem.memories.add("Priya Nair signs the Lumen renewal, and it comes up in March.")
print(mem.context("Who signs the Lumen renewal?"))
# - Priya Nair signs the Lumen renewal.  [note, 2026-10-05]
```

## Repositories

| | |
| --- | --- |
| [**geniffy-python**](https://github.com/Geniffy/geniffy-python) | The Python SDK, sync and async. `pip install geniffy` |
| [**geniffy-typescript**](https://github.com/Geniffy/geniffy-typescript) | The TypeScript and JavaScript SDK, for Node, Bun, Deno and edge runtimes. `npm install geniffy` |
| [**geniffy-mcp**](https://github.com/Geniffy/geniffy-mcp) | Your memory inside Claude, ChatGPT, Cursor, VS Code and Codex, with sign-in. `https://api.geniffy.com/mcp` |
| [**examples**](https://github.com/Geniffy/examples) | Runnable programs: a quickstart, a support bot with one memory per customer, and a chat with Claude that remembers you |

Report a vulnerability to ops@geniffy.com, not in a public issue.
