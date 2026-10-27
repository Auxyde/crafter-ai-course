# Course agents

Put each agent implementation in its own subdirectory under this folder. The
Crafter environment is installed from the sibling `crafter-core/` directory,
so agent code can import it as `import crafter` without copying environment
source into the agent folders.

Example layout:

```text
ai/
├── README.md
└── dqn/
    ├── train.py
    └── evaluate.py
```

Run agent commands from the repository root so relative paths to checkpoints
and logs remain consistent.
