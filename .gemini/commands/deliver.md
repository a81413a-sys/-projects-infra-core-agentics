# Command: /deliver
# Description: Synthesize specialist outputs and package the final deliverable.

1. COO reads all specialist outputs in `shared-memory/client/current/{client_name}/`.
2. Generate `final-blueprint.pdf` (or markdown) and `deployment-package.zip`.
3. Move project to `shared-memory/client/archive/` upon completion.
