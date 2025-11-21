# Installation and Configuration

## Section Overview

A step-by-step guide to setting up Claude Code for professional use, focusing on ease of use for non-technical users.

### Prerequisites

- Command line comfort
- Claude API key
- VS Code (recommended)

## Your AI-Ready Text Editor: VS Code

<img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" alt="Visual Studio Code Logo" width="120" />

Think of VS Code as your mission control for AI work. Unlike basic text editors, VS Code understands code, can work with AI tools, and makes file management simple.

**Why VS Code for AI Work?**
- AI tools can read and write VS Code files directly
- Built-in terminal means everything in one place
- Extensions add AI-specific capabilities
- Free, reliable, and constantly updated

### Installing VS Code

**For All Platforms:**
1. **Visit** [code.visualstudio.com](https://code.visualstudio.com)
2. **Click** the big "Download" button (it detects your operating system)
3. **Run** the installer with default settings
4. **Launch** VS Code when installation completes

### Essential Extensions for AI Work

Extensions are like apps for VS Code. Install these immediately:

**To Install Extensions:**
1. **Open** VS Code
2. **Click** the Extensions icon (looks like four squares) in the left sidebar
3. **Search** for each extension below
4. **Click** "Install" for each one

**Must-Have Extensions:**

1. **Python** (by Microsoft)
   - Enables Python script editing and execution
   - Essential for AI tool integrations

2. **Markdown All in One** (by Yu Zhang)
   - Makes writing and editing markdown files simple
   - Live preview of formatted text

3. **GitLens** (by GitKraken)
   - Shows file history and changes
   - Helps track your project evolution

4. **YAML** (by Red Hat)
   - Support for YAML configuration files
   - Essential for agent and workflow configurations

!!! tip "VS Code First Steps"
    After installing extensions:
    1. **Create** a new file (Ctrl+N or Cmd+N)
    2. **Save** it as "test.md" (this creates a markdown file)
    3. **Type** some text with `# Heading` and `**bold text**`
    4. **Right-click** and select "Open Preview" to see formatted version

    Congratulations! You've created your first AI-ready document.

## Command Line Setup: Your Direct Computer Interface

The command line is like texting with your computer instead of using a mouse. AI tools often work through command-line interfaces, so basic comfort here unlocks advanced capabilities.

**Don't Panic!** You'll only need 4-5 basic commands. Think of it like learning to drive - intimidating at first, but quickly becomes second nature.

### Windows Setup: WSL (Windows Subsystem for Linux)

WSL gives Windows users access to Linux-style commands that most AI tools expect.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1em 0;">
  <iframe 
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    src="https://www.youtube.com/embed/vxTW22y8zV8" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
  </iframe>
</div>

**Step-by-Step Installation:**

1. **Open PowerShell as Administrator**:
   - Press `Windows + X`
   - Select "Windows PowerShell (Admin)" or "Terminal (Admin)"
   - Click "Yes" when prompted

2. **Install WSL**:
   ```powershell
   wsl --install
   ```

3. **Restart** your computer when prompted

4. **Complete Setup**:
   - After restart, Ubuntu will automatically open
   - Create a username (use lowercase, no spaces)
   - Create a password (you won't see characters as you type - this is normal!)

5. **Install Windows Terminal** (Better Interface):
   - Open Microsoft Store
   - Search for "Windows Terminal"
   - Install the official Microsoft app
   - Set as your default terminal application

!!! warning "Common WSL Issues & Solutions"
    **Problem**: "WSL command not found"
    **Solution**: Update Windows to the latest version first

    **Problem**: Installation hangs or fails
    **Solution**: Try `wsl --install -d Ubuntu` for specific distribution

    **Problem**: Can't remember Ubuntu password
    **Solution**: You can reset it through PowerShell with `wsl --user root`

### Installation Steps

1. Verify system requirements
2. Install Claude Code CLI
3. Configure authentication
4. Test initial setup

### Configuration Best Practices

- Secure API key management
- Setting up `.clauderc`
- Configuring default behaviors

### Environment Setup

- Choosing the right workspace
- Organizing your Claude Code projects
- Managing permissions and access