# 0.2 Essential Setup (Free Tier Start)

Time to build your AI toolkit! This section transforms your computer into a powerful AI development environment. Every step is designed for absolute beginners - no technical experience required.

## Why This Setup Matters

Think of this setup like organizing a workshop. A carpenter needs the right tools accessible and organized to build furniture efficiently. Similarly, AI-powered work requires the right digital tools properly configured.

**What you're building:**
- Your AI account dashboard (like having multiple expert consultants on speed dial)
- A command-line interface (like having a direct line to your computer's capabilities)
- A text editor that AI systems can work with (like having a shared workspace)
- Version control (like having unlimited "undo" for your projects)

## Creating Your AI Accounts

!!! warning "Privacy and Security Strategy"
    **Best Practice**: Create a dedicated email address for AI tools (like `yourname.ai@gmail.com`). This keeps your AI work organized and protects your primary email from promotional messages.

    **Security Tip**: Enable two-factor authentication on all accounts. Most services offer this through your phone's authenticator app.

### AI Platform Setup Guide

We'll set up accounts on the "Big Three" AI platforms that complement each other perfectly:

**Why These Three?**
- **Claude**: Best for analysis, reasoning, and working with documents
- **ChatGPT**: Strong general capabilities and widely supported integrations
- **Gemini**: Excellent for research and integrated with Google services

#### 1. Anthropic Account for Claude

<img src="https://www.malwarebytes.com/wp-content/uploads/sites/2/2025/08/Claude_logo.png" alt="Anthropic Claude Logo" width="120" />

**Step-by-Step Setup:**

1. **Visit** [claude.ai](https://claude.ai)
2. **Click** "Sign Up" in the top right corner
3. **Choose** your signup method:
   - Email address (recommended for beginners)
   - Google account (convenient if you use Gmail)
   - Apple account (for Mac users)
4. **Verify** your email address through the confirmation link
5. **Complete** the brief welcome survey (helps Claude understand your use case)

!!! tip "First Conversation Test"
    Once logged in, try this prompt to test Claude:

    ```
    Help me understand what makes a good AI prompt. Give me 3 examples:
    one bad example, one good example, and one excellent example.
    Explain why each example works or doesn't work.
    ```

    This tests Claude's ability to teach and provide structured examples.

#### 2. OpenAI Account for ChatGPT

<img src="https://upload.wikimedia.org/wikipedia/commons/0/04/ChatGPT_logo.svg" alt="OpenAI ChatGPT Logo" width="120" />

**Step-by-Step Setup:**

1. **Visit** [chat.openai.com](https://chat.openai.com)
2. **Click** "Sign up"
3. **Create account** with:
   - Email address and password, OR
   - Google/Microsoft account
4. **Verify** email address
5. **Set up two-factor authentication** (strongly recommended):
   - Go to Settings → Security
   - Follow the authenticator app setup process

!!! tip "First Conversation Test"
    Test ChatGPT with this prompt:

    ```
    I'm new to AI and want to automate some of my work tasks.
    Ask me 5 questions to understand my work better, then suggest
    one specific AI automation I could start with this week.
    ```

    This tests ChatGPT's ability to have interactive conversations and provide personalized recommendations.

#### 3. Google Account for Gemini

<img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/Google_Gemini_logo.svg" alt="Google Gemini Logo" width="120" />

**If you already have a Google account:**
1. **Visit** [gemini.google.com](https://gemini.google.com)
2. **Sign in** with your Google account
3. **Accept** the Gemini terms of service
4. **Complete** the setup process

**If you need a new Google account:**
1. **Visit** [accounts.google.com](https://accounts.google.com)
2. **Click** "Create account" → "Personal"
3. **Fill out** the registration form
4. **Verify** phone number
5. **Navigate** to [gemini.google.com](https://gemini.google.com)

!!! tip "First Conversation Test"
    Test Gemini with this prompt:

    ```
    Research the latest trends in AI automation for small businesses.
    Create a summary with 5 key trends, why each matters,
    and one specific tool or platform for each trend.
    ```

    This tests Gemini's research capabilities and structured output.

#### 4. GitHub Account (Essential for AI Tools)

<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub Logo" width="120" />

GitHub hosts most AI tools, code samples, and integrations you'll use throughout this course.

**Step-by-Step Setup:**

1. **Visit** [github.com](https://github.com)
2. **Click** "Sign up"
3. **Enter** username (suggestion: use your real name or professional handle)
4. **Use** the same email address as your AI accounts
5. **Choose** a strong password
6. **Verify** your account through email
7. **Complete** the welcome survey (select interests related to AI/automation)

!!! tip "Why GitHub Matters for AI"
    GitHub is where the AI community shares:
    - Pre-built AI tools and integrations
    - Code samples you can copy and customize
    - Documentation for AI platforms
    - Community projects you can contribute to

    You won't need to write code, but you'll frequently download and use AI tools hosted on GitHub.

## Essential Tools Installation

!!! note "VS Code and WSL Setup"
    Detailed installation instructions for Visual Studio Code and Windows Subsystem for Linux (WSL) have been moved to **Module 8: Installation and Configuration**.
    
    For Windows users who need WSL setup, or if you want to install VS Code with recommended extensions, see:
    - [Module 8.2: Installation and Configuration](../../module-8/sections/8-2-installation-and-configuration.md)
    
    These tools are essential for advanced AI work with Claude Code, but not required for the initial modules of this course.

#### Mac Setup: Built-in Terminal + Homebrew

Macs come with excellent command-line tools built-in. We'll enhance them with Homebrew, the standard Mac package manager.

**Step-by-Step Setup:**

1. **Open Terminal**:
   - Press `Cmd + Space` to open Spotlight
   - Type "Terminal" and press Enter
   - Pin to Dock for easy access

2. **Install Homebrew** (Package Manager):
   Copy and paste this command into Terminal:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

3. **Follow Installation Prompts**:
   - Press Enter when prompted
   - Enter your Mac password when requested
   - Wait for installation (5-10 minutes)

4. **Verify Installation**:
   ```bash
   brew --version
   ```
   You should see version information.

!!! tip "Mac Terminal Comfort Tips"
    **Make Text Larger**: Terminal → Preferences → Profiles → Text → Font Size

    **Change Colors**: Try different themes in Terminal → Preferences → Profiles

    **Command History**: Press ↑ arrow to see previous commands

#### Installing Git (Version Control for Everyone)

Git tracks changes to your files and lets you download AI tools from GitHub. Think of it as "unlimited undo" for your projects.

**Windows (WSL) Installation:**
```bash
sudo apt update
sudo apt install git
```

**Mac Installation:**
```bash
brew install git
```

**Verify Installation (Both Platforms):**
```bash
git --version
```

**Basic Git Configuration:**
Run these commands with your information:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Command Line Basics for AI Work

Now let's learn the essential commands that unlock AI tool capabilities. Master these 5 commands and you'll be ready for 90% of AI tool installations and usage.

### Understanding the Command Line Interface

**What it looks like:**
```
your-username@computer-name:~/current-folder$
```

This is called a "prompt" - it's waiting for your command.

**Parts Explained:**
- `your-username`: Your account name
- `computer-name`: Your computer's name
- `~/current-folder`: Where you are in the file system
- `$`: Indicates you can type a command

### The Essential Five Commands

#### 1. `pwd` - "Print Working Directory" (Where Am I?)

**What it does**: Shows your current location in the file system

**Example:**
```bash
pwd
```
**Output**: `/home/your-username` or `/Users/your-username`

**Real-world use**: Before installing AI tools, confirm you're in the right folder

#### 2. `ls` (Mac/Linux) or `dir` (Windows) - List Contents

**What it does**: Shows files and folders in your current location

**Examples:**
```bash
ls                    # Basic listing
ls -la                # Detailed listing with hidden files
```

**Real-world use**: See what files are available before working with AI tools

#### 3. `cd` - "Change Directory" (Move Around)

**What it does**: Moves you to different folders

**Examples:**
```bash
cd Documents          # Move to Documents folder
cd ..                 # Move up one level
cd ~                  # Go to home folder
cd /                  # Go to root folder
```

**Real-world use**: Navigate to where you store AI projects and data

#### 4. `mkdir` - "Make Directory" (Create Folders)

**What it does**: Creates new folders

**Examples:**
```bash
mkdir ai-projects                    # Create one folder
mkdir -p ai-projects/data/csv       # Create nested folders
```

**Real-world use**: Organize your AI work into logical project structures

#### 5. `cp` (Mac/Linux) or `copy` (Windows) - Copy Files

**What it does**: Copies files and folders

**Examples:**
```bash
cp file.txt backup-file.txt         # Copy file
cp -r folder/ backup-folder/        # Copy folder and contents
```

**Real-world use**: Backup important files before AI tools modify them

### Practice Exercise: Command Line Confidence Builder

Complete this hands-on exercise to build command-line confidence:

**Exercise Steps:**

1. **Open your terminal/command prompt**

2. **Find your location:**
   ```bash
   pwd
   ```

3. **See what's here:**
   ```bash
   ls
   ```
   (or `dir` on Windows)

4. **Create your AI workspace:**
   ```bash
   mkdir ai-learning-workspace
   ```

5. **Move into it:**
   ```bash
   cd ai-learning-workspace
   ```

6. **Create project structure:**
   ```bash
   mkdir data prompts outputs
   ```

7. **Verify your work:**
   ```bash
   ls
   ```
   You should see three folders: `data`, `prompts`, `outputs`

8. **Navigate back home:**
   ```bash
   cd ~
   ```

!!! success "Command Line Achievement Unlocked!"
    If you completed this exercise, you now have the command-line skills needed for 90% of AI tool installations and usage. Everything else builds on these fundamentals.

### Troubleshooting Common Command Line Issues

??? question "Command not found"
    **Problem**: You type a command and get "command not found"

    **Solutions**:
    - Check spelling (commands are case-sensitive)
    - Ensure you're in the right operating system (ls vs dir)
    - For Windows, ensure you're using WSL for Linux commands

??? question "Permission denied"
    **Problem**: Can't create folders or copy files

    **Solutions**:
    - Try adding `sudo` before the command (Mac/Linux/WSL)
    - Ensure you have write permissions in the current directory
    - Navigate to your home directory first: `cd ~`

??? question "Can't find files I just created"
    **Problem**: Created files but can't see them

    **Solutions**:
    - Use `ls -la` to show hidden files
    - Confirm you're in the right directory with `pwd`
    - File might be created in a different location than expected

## Checkpoint Exercise: Setup Verification

Time to verify your complete AI development environment! This exercise ensures everything is properly configured before moving forward.

### Part 1: Account Verification Screenshots

Take screenshots showing successful login to each platform:

1. **Claude Screenshot**:
   - Login to [claude.ai](https://claude.ai)
   - Take screenshot showing your username/profile in top-right corner
   - Test with the prompt provided earlier

2. **ChatGPT Screenshot**:
   - Login to [chat.openai.com](https://chat.openai.com)
   - Take screenshot showing the interface with your account
   - Test with the interactive prompt provided earlier

3. **Gemini Screenshot**:
   - Login to [gemini.google.com](https://gemini.google.com)
   - Take screenshot showing the interface
   - Test with the research prompt provided earlier

4. **GitHub Screenshot**:
   - Login to [github.com](https://github.com)
   - Take screenshot showing your profile/dashboard

### Part 2: Tool Verification Checklist

Create your first AI project file to verify all tools work together:

1. **Open VS Code**

2. **Create a new file** (Ctrl+N or Cmd+N)

3. **Save as** `ai-setup-verification.md` in your home directory

4. **Copy and paste this template, then fill it out:**

```markdown
# My AI Learning Setup Verification

**Date**: [Today's date]
**Computer**: [Windows/Mac/Linux]

## Account Status

### AI Platform Accounts
- [ ] Claude (Anthropic) - Account created and verified
- [ ] ChatGPT (OpenAI) - Account created and verified
- [ ] Gemini (Google) - Account created and verified
- [ ] GitHub - Account created and verified

### Test Conversations Completed
- [ ] Claude: Tested prompt engineering explanation
- [ ] ChatGPT: Tested interactive work automation planning
- [ ] Gemini: Tested research and trend analysis

## Tool Installation Status

### Essential Tools
- [ ] VS Code installed and configured
- [ ] VS Code extensions installed (Python, Markdown All in One, GitLens, YAML)
- [ ] Command line interface ready (Terminal/WSL)
- [ ] Git installed and configured

### Command Line Verification
- [ ] Can open terminal/command prompt
- [ ] Successfully used `pwd` command
- [ ] Successfully used `ls`/`dir` command
- [ ] Successfully used `cd` command
- [ ] Successfully used `mkdir` command
- [ ] Created ai-learning-workspace folder structure

## First AI Conversation Results

### Most Helpful AI Response
**Platform**: [Claude/ChatGPT/Gemini]
**Prompt**: [What you asked]
**Why it was helpful**: [Your assessment]

### Biggest Setup Challenge
**Issue**: [What was difficult]
**Solution**: [How you solved it or what help you needed]

## Readiness Assessment

**Confidence Level** (1-10 scale):
- Using command line: ___/10
- AI conversation quality: ___/10
- Overall setup readiness: ___/10

**Next Learning Priority**:
[What do you want to focus on in Module 0.3?]

## Notes and Observations
[Any additional thoughts, concerns, or discoveries]
```

5. **Save the file** (Ctrl+S or Cmd+S)

6. **Take a screenshot** of VS Code with your completed verification file

### Part 3: Command Line Final Test

Open your terminal and run these commands to verify everything works:

```bash
# Verify you're in the right place
pwd

# Check your workspace exists
ls ai-learning-workspace

# Verify git works
git --version

# Create a test file
echo "Hello AI World!" > test-file.txt

# Verify the file was created
ls -la test-file.txt

# Clean up
rm test-file.txt
```

!!! success "Setup Complete!"
    If all commands ran successfully, you now have a complete AI development environment. You're ready to start building AI-powered workflows!

### What's Next?

You've successfully created your AI command center! In section 0.3, you'll learn how to organize this workspace for maximum AI efficiency, including:

- File naming conventions that AI systems love
- Project organization that scales with complexity
- Working with CSV, JSON, YAML, and Markdown files
- Creating your first structured AI prompt that gets consistent results

The technical foundation is complete - now we'll focus on making it productive and organized.