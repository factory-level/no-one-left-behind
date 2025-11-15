# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an AI course documentation project designed for beginners transitioning to AI-powered work systems. The project contains extensive course materials covering AI tools, agents, and automation workflows. It uses MkDocs for documentation generation and is structured for educational content delivery.

## Architecture & Structure

- **Main course content**: `COURSE.md` - Comprehensive 12-module curriculum covering prompting to multi-agent orchestration
- **Documentation**: Uses MkDocs with `mkdocs.yml` configuration and `docs/` directory
- **Virtual environment**: Python 3.12 with MkDocs installed in `venv/`
- **Content organization**: Single large markdown file with hierarchical module structure
- **Note-taking**: Obsidian vault configuration in `.obsidian/` for rich markdown editing

## Development Commands

**Activate virtual environment** (required for all operations):
```bash
source venv/bin/activate
```

**Documentation development**:
- `mkdocs serve` - Start live-reloading development server (usually runs on http://127.0.0.1:8000)
- `mkdocs build` - Build static documentation site
- `mkdocs --help` - Show available commands

**Python package management**:
- `pip install <package>` - Install new dependencies
- `pip list` - Show installed packages

## Working with Course Content

The primary course content is in `COURSE.md` - a comprehensive 1200+ line curriculum. When editing:

1. **Module structure**: 12 main modules (0-11) plus appendices covering AI landscape from basic prompting to multi-agent systems
2. **Target audience**: Non-technical professionals learning AI automation
3. **Learning progression**: Sequential modules building from prompting → tools → agents → orchestration
4. **Practical focus**: Heavy emphasis on hands-on labs and real-world applications

Key course themes:
- Claude ecosystem (web, desktop, code)
- Model Context Protocol (MCP) integration
- Agent architecture and multi-agent systems
- Workflow automation tools (n8n, AgentKit)
- RAG (Retrieval Augmented Generation) for large datasets

## Content Management Notes

- Course content spans multiple AI tools and platforms (Claude, ChatGPT, Gemini, etc.)
- Includes technical setup instructions for non-technical users
- Balances conceptual understanding with practical implementation
- Contains extensive appendices with reference materials and troubleshooting

## File Organization

```
├── COURSE.md           # Main curriculum content
├── README.md          # Project overview and hosting info
├── mkdocs.yml         # MkDocs configuration
├── docs/              # Documentation directory
│   └── index.md       # Default MkDocs homepage
├── venv/              # Python virtual environment
└── .obsidian/         # Obsidian note-taking configuration
```

The project is optimized for single-author content development with eventual web deployment for course delivery.