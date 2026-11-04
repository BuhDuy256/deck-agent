# DeckAgent

DeckAgent is an open-source AI agent harness for making presentations. You describe the
presentation you need; DeckAgent interviews you about the audience, the purpose and the
sources, proposes an outline for you to confirm, and then builds the slides with the AI
model you choose.

DeckAgent is developed by a team of five students from HCMUS (the University of Science,
Ho Chi Minh City), Vietnam.

> **Status:** this repository is a rewrite of
> [Luke23127006/DeckAgent](https://github.com/Luke23127006/DeckAgent) on the
> [OpenCode](https://github.com/sst/opencode) runtime. It has no runnable release yet;
> setup instructions will appear here with the first version.

## What makes it different

A model alone can write slide markup. DeckAgent adds the harness around the model:

- **It asks before it builds.** Who the deck is for, how long the talk is, what it must
  achieve, which sources to use, which language and which output format.
- **It keeps you in control.** No slide is built until you confirm the outline and the
  output format.
- **It reuses what is prepared.** Themes, layouts, animations and format renderers are
  built in advance and applied by code. The model is called where judgment is needed:
  understanding the request, interviewing you and writing content. See
  [the LLM boundary](docs/architecture/llm-boundary.md).

## Principles

- **Your model, your key.** You choose the model and bring your own provider key.
  DeckAgent has no model account of its own.
- **Runs on your computer.** No hosted service, no DeckAgent account.
- **Your work stays local.** Chats, decks and files stay on your machine. Content leaves
  it only in requests to the provider of the model you selected.

## Documentation

- [Architecture](docs/architecture/) — the modules of DeckAgent and where the model is
  used, as built.

## Contributing

- [AGENTS.md](AGENTS.md) — the index for contributors and coding agents: rules, roles
  and where everything lives.
- [WORKFLOW.md](WORKFLOW.md) — how a version is planned and how each feature goes from
  spec to verified code.

DeckAgent is inspired by [open-design](https://github.com/nexu-io/open-design), its main
product reference.
