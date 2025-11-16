# Overview
This project is for course materials for a beginner's AI Course for mostly non-technical users attempting to become skilled in today's main AI landscape.

## Course Overview
The course overview exists outside of this `README.md` to ensure that the project's updates are decoupled from changes to the META of this project and getting it to run as it will be a webapp for documentation eventually using something like docusaurus or equivalent.

# Getting Started with MkDocs

## Prerequisites
- Python 3.12 or higher
- Git (for cloning and version control)

## Setup Instructions

### 1. Clone and Navigate to Project
```bash
git clone <repository-url>
cd ai-course-beginner
```

### 2. Activate Virtual Environment
The project includes a pre-configured Python virtual environment with MkDocs installed:

```bash
source venv/bin/activate
```

### 3. Verify MkDocs Installation
```bash
mkdocs --version
```

## Development Workflow

### Start Development Server
Launch the live-reloading development server to preview changes:

```bash
mkdocs serve
```

The site will be available at http://127.0.0.1:8000

### Build Static Site
Generate the static documentation site:

```bash
mkdocs build
```

Built files will be in the `site/` directory.

### Available Commands
- `mkdocs serve` - Start development server with live reload
- `mkdocs build` - Build static site
- `mkdocs --help` - Show all available commands

## Project Structure
```
├── COURSE.md           # Main curriculum content (1200+ lines)
├── mkdocs.yml         # MkDocs configuration
├── docs/              # Documentation source files
│   └── index.md       # Homepage content
├── venv/              # Python virtual environment (pre-configured)
└── .obsidian/         # Obsidian vault for rich markdown editing
```

## Course Content Management
The primary course material is in `COURSE.md` - a comprehensive 12-module AI curriculum covering:
- Module 0-11: Progressive AI learning from prompting to multi-agent orchestration
- Target: Non-technical professionals transitioning to AI-powered workflows
- Focus: Hands-on labs with Claude ecosystem, MCP integration, and automation tools

## Hosting this Course

### Requirements
