# Crafter AI Course

This repository keeps the Crafter environment separate from the agents built
for the course:

```text
.
├── crafter-core/   # Crafter environment and its reference examples
└── ai/             # Course agents and their experiments
```

## Setup

Create and activate a virtual environment from the repository root, then
install Crafter in editable mode:

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -e ./crafter-core
```

The installation includes `tqdm`, which is required by the random-agent
example.

Install the optional GUI dependencies when needed:

```sh
python -m pip install -e './crafter-core[gui]'
```

The Crafter GUI can then be started with:

```sh
python -m crafter.run_gui
```

Agent implementations belong in [`ai/`](./ai/). See
[`ai/README.md`](./ai/README.md) for the expected workflow.
