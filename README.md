# Excalidraw Diagram Skill

Coding agent skill that generates practical excalidraw diagrams from natural language descriptions in a native obsidian plugin `excalidraw.md` format.

## Installation

Clone this repository into agent's global skills directory:

```bash
git clone https://github.com/waheeb4/excalidrawmd.git ~/.config/agent/skills/excalidrawmd
```

Restart agent after installing the skill.

## Setup

Install the renderer dependencies:

```bash
cd ~/.config/agent/skills/excalidrawmd/references
uv sync
```

The renderer uses Brave Origin.

Edit `references/color-palette.md` to customize the diagram color palette.

## File Structure

```
excalidrawmd/
  SKILL.md                          # Design methodology and workflow
  references/
    color-palette.md                # Diagram color palette
    element-templates.md            # Excalidraw element templates
    json-schema.md                  # Excalidraw JSON format reference
    render_excalidraw.py            # Render .excalidraw and .excalidraw.md files
    render_template.html            # Browser rendering template
    pyproject.toml                  # Python dependencies
```
