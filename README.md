# Icy Shadow

I build software end to end — from low-level engine internals to the web
apps that sit on top of them. My main project is a Godot/GDScript coding
assistant trained from scratch: the corpus, the tokenizer, the transformer,
the training loop, and the Studio web app around it. On the side I write
desktop tools, game prototypes, and automation.

I like to understand the whole pipeline before I touch any part of it, and
I prefer building things myself over wiring up black boxes.

## Featured Projects

### [godot-coder-ai](https://github.com/IcyShadow5/godot-coder-ai)

Local training studio for a compact Godot/GDScript language model — corpus,
training, and chat in one pipeline, running entirely on your own GPU.

- **Stack:** Python · PyTorch · FastAPI · Godot headless · GitHub Actions
- **The interesting part:** every script in the training corpus is verified
  by Godot itself — full project import or per-file parse — so the model
  only learns code that actually parses and runs. The transformer (attention,
  RoPE, KV-cache) is written from scratch, and the whole thing runs locally
  at `127.0.0.1:8765`, no cloud, no API keys.
- **Docs:** [icyshadow5.github.io/godot-coder-ai](https://icyshadow5.github.io/godot-coder-ai/)

### [IcySW](https://github.com/IcyShadow5/IcySW)

Local analysis and optimization tool for Summoners War.

- **Purpose:** data processing, recommendation logic, and optimization for
  the game's rune system, wrapped in a desktop app.
- **Stack:** TypeScript · React · Tauri · Rust
- **The interesting part:** a Rust core keeps the data-heavy work close to
  the metal while React drives the desktop UI.

## Currently Building

- **godot-coder-ai** — next stage is instruction tuning, so the model goes
  from continuing code to answering prompts
- **EngineSandbox** — a C++ engine architecture project: engine lifecycle,
  systems design, and low-level programming concepts
- **Game development** — [SpaceEX](https://github.com/IcyShadow5/SpaceEX)
  (modular block construction, pilotable vehicles, survival systems in Godot 4)
  and [ember-idle](https://github.com/IcyShadow5/ember-idle) (mobile idle game)

## Technology

| Area | Stack |
|---|---|
| **Languages** | Python · GDScript · TypeScript · C++ · Rust · JavaScript · PowerShell |
| **AI / Machine Learning** | PyTorch · from-scratch transformers · tokenizers · custom training loops |
| **Game development** | Godot Engine · GDScript |
| **Systems / Desktop** | Rust · Tauri · C++ engine internals |
| **Web / Tooling** | React · FastAPI · GitHub Actions · Git · MkDocs · SQLite |

## Elsewhere

- [godot-coder-ai docs](https://icyshadow5.github.io/godot-coder-ai/) —
  architecture, config reference, changelog

Always happy to talk about training small models, engine design, or why your
dataset deserves more attention than your model does.
