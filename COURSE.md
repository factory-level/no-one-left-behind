# **AI-Powered Work Systems: From Prompting to Multi-Agent Orchestration**

---

## **MODULE 0: FOUNDATION & SETUP**

_Getting your environment ready and understanding what you're building toward_

### 0.1 Course Orientation

- **What you'll be able to do by the end**: Vision casting for multi-agent systems
- **The learning path**: From single prompts → tool-using AI → autonomous agents → orchestrated systems
- **Mindset shift**: From "AI as search engine" to "AI as intelligent workforce"

### 0.2 Essential Setup (Free Tier Start)

- **Creating accounts** (free tiers):
    - Google account for Gemini
    - Anthropic account for Claude
    - OpenAI account for ChatGPT
    - GitHub account (for accessing tools/MCPs)
- **Installing your first tools**:
    - VS Code (text editor for viewing/editing files)
    - Windows Terminal or PowerShell basics
    - Git for Windows (basic installation only)
- **Command Line Basics for the Non-Technical**:
    - What is CLI and why it matters for agents
    - Essential commands: `cd`, `ls`/`dir`, `mkdir`, basic navigation
    - How to read file paths (absolute vs relative)
    - Running simple commands (demystifying the terminal)

### 0.3 Understanding Your Workspace

- **File organization for AI work**:
    - Creating project folders
    - Naming conventions that AI systems understand
    - Where to store: data files, prompts, agent configurations
- **Document types you'll work with**:
    - Markdown (.md) - the universal AI language
    - CSV files - your data playground
    - JSON - configuration files explained simply
    - YAML - agent instruction format

---

## **MODULE 1: PROMPTING MASTERY**

_The foundation skill that everything else builds upon_

### 1.1 How LLMs Actually Work (Non-Technical)

- **The prediction engine**: Understanding "next token prediction"
- **Tokens explained**: Why character count matters, estimating tokens
- **Context window**: The AI's "working memory"
    - Why it's limited and how to work within constraints
    - Visual analogy: Filing cabinet vs. entire library
- **Temperature and randomness**: Why AI gives different answers
- **What AI can and cannot do**: Setting realistic expectations

### 1.2 Prompt Engineering Fundamentals

- **Anatomy of a good prompt**:
    - Role/persona assignment
    - Clear task definition
    - Context provision
    - Output format specification
    - Constraints and boundaries
- **The Clarity Principle**: Detractors and clear prompt intent
    - What confuses LLMs
    - How to remove ambiguity
    - Examples: vague vs. precise prompts
- **Structured prompting formats**:
    - Using markdown headers in prompts
    - XML tags for complex instructions
    - JSON for structured outputs

### 1.3 Advanced Prompting Techniques

- **Chain-of-thought prompting**: Making AI "show its work"
- **Few-shot learning**: Teaching by example
- **Reverse prompting**:
    - What is it and why it's powerful
    - Starting with desired output and working backward
    - Practical exercise: Reverse engineering a data analysis report
- **Prompt chaining**: Breaking complex tasks into steps
- **Meta-prompting**: Asking AI to improve your prompts

### 1.4 Reasoning and Why It Matters

- **What is "reasoning" in AI context?**
- **Extended thinking models**: o1, Claude Sonnet 4.5 capabilities
- **When to use reasoning vs. speed**:
    - Complex analysis = reasoning
    - Simple tasks = fast models
- **How to trigger better reasoning**:
    - Prompting techniques that encourage deep thinking
    - "Think step-by-step" and variations
    - Asking AI to consider alternatives

### 1.5 Practical Prompting Lab

- **Exercise 1**: Transform a messy spreadsheet analysis task into a perfect prompt
- **Exercise 2**: Create a prompt template for recurring work tasks
- **Exercise 3**: Build a prompt that outputs exactly what you need (format control)
- **Exercise 4**: Use reverse prompting to design a policy document template

---

## **MODULE 2: LLM LANDSCAPE & PRODUCT ECOSYSTEM**

_Understanding your AI toolkit and choosing the right tool for each job_

### 2.1 The Major LLMs: Strengths & Use Cases

- **Claude (Anthropic)**:
    
    - Model family: Opus 4.1/4, Sonnet 4.5/4
    - **Your workhorse for**: Analytical work, long documents, reasoning tasks
    - Strengths: 200K context, nuanced analysis, following complex instructions
    - Weaknesses: Not best for creative writing, sometimes overly cautious
    - When to choose Claude
- **ChatGPT (OpenAI)**:
    
    - Model family: GPT-4, GPT-4o, o1-preview/mini
    - **Your choice for**: Quick tasks, brainstorming, general knowledge
    - Strengths: Fast, conversational, great plugin ecosystem
    - Weaknesses: Smaller context than Claude, can be verbose
    - When to choose ChatGPT
- **Gemini (Google)**:
    
    - Model family: 1.5 Pro, 1.5 Flash
    - **Your secret weapon for**: Massive context (2M tokens), multi-file analysis
    - Strengths: Can process entire databases, integrates with Google Workspace
    - Weaknesses: Less sophisticated reasoning than Claude
    - When to choose Gemini
- **Model comparison matrix**: Speed vs. reasoning vs. context vs. cost
    

### 2.2 Product Ecosystem: Web Interfaces

- **Claude.ai**:
    - Projects feature (organizing work contexts)
    - Artifacts (living documents)
    - When to use web vs. API vs. Desktop
- **ChatGPT interface**:
    - Custom GPTs (pre-configured assistants)
    - Memory features
    - Canvas mode for iterative work
- **Gemini interface**:
    - Google Workspace integration
    - Extensions ecosystem
    - Long context file uploads

### 2.3 Specialized AI Products

- **NotebookLM**: Curating your own knowledge base
    - What it is: Turn your documents into an interactive expert
    - Use cases: Policy manuals, training materials, research synthesis
    - How it works: Upload sources → Ask questions → Generate guides
    - **Practical lab**: Create a NotebookLM from your work documents
    - Audio overviews: Turn documents into podcast-style summaries
- **ChatGPT Deep Research / Claude Research (coming)**:
    - What autonomous research means
    - When to use vs. manual prompting
    - Understanding: Research plans → Execution → Synthesis
    - Cost considerations
- **Perplexity**:
    - AI-powered search vs. traditional Google
    - When to use: Current events, fact-checking, source verification
    - Pro features: Deeper research, file analysis
    - Citation tracking

### 2.4 Choosing Your Tools: Decision Framework

- **Task categorization exercise**: Map your duties to optimal tools
- **The escalation ladder**: Start simple, escalate to powerful tools when needed
- **Cost-benefit analysis**: Free tier vs. subscription vs. API usage

---

## **MODULE 3: CLAUDE DEEP DIVE**

_Mastering your primary AI workhorse_

### 3.1 Claude Products Explained

- **Claude.ai (Web)**: Your daily driver
    
    - Projects: Contextual workspaces
    - Team plans vs. individual
    - When web is enough
- **Claude Desktop**: Native app with superpowers (we'll expand on this)
    
- **Claude API**: When you need programmatic access (overview for now)
    
- **Claude Code**: Your agent builder (dedicated module later)
    

### 3.2 Claude Projects: Organizing Context

- **What are Projects?**: Persistent context containers
- **Setting up effective Projects**:
    - One project per major work domain
    - Uploading background documents
    - Writing custom instructions
    - Managing project knowledge
- **Practical exercise**: Create projects for:
    - Data analysis workspace
    - Team management assistant
    - Stakeholder communication hub

### 3.3 Claude Skills: The Game-Changer

- **What are Skills?**: Extended capabilities through guided tools
- **Why Skills matter**: Emergent functionality beyond base model
- **Built-in Skills**:
    - Document creation (DOCX, PPTX, XLSX)
    - PDF manipulation
    - Spreadsheet analysis
    - Data visualization
- **How Skills work behind the scenes**:
    - Skills are enhanced prompt templates + tools
    - Understanding the `.md` skill format
    - How Claude "learns" from skills
- **Value proposition**:
    - Consistency in output
    - Complex workflows simplified
    - Reusable expertise

### 3.4 Creating Your First Custom Skill

- **Skill anatomy**:
    - Markdown structure
    - Clear instructions
    - Input/output specifications
    - Example patterns
- **Use case examples**:
    - "Weekly report generator" skill
    - "Data validation" skill
    - "Meeting summary formatter" skill
- **Hands-on lab**: Build a skill for a recurring task from your work

### 3.5 Advanced Claude Techniques

- **Artifacts mastery**: Using Claude's interactive document editor
- **Multi-turn analysis**: Building context across conversations
- **Handling long documents**: Strategies for documents exceeding context
- **Extracting structured data**: CSV/JSON outputs from analysis

---

## **MODULE 4: MODEL CONTEXT PROTOCOL (MCP)**

_Connecting AI to your actual work tools_

### 4.1 What is MCP? The Breakthrough Explained

- **The problem MCP solves**: AI locked in a chat box vs. AI with hands
- **Visual metaphor**: AI as brain, MCPs as arms and legs
- **How MCP works** (non-technical explanation):
    - Server (the tool connection)
    - Client (Claude Desktop, Claude Code)
    - Protocol (the language they speak)
- **Why this is groundbreaking**:
    - Real-time data access
    - Action execution (not just analysis)
    - Multi-tool orchestration

### 4.2 MCP Architecture (Simplified)

- **The MCP server**: A small program that connects to a service
- **The MCP client**: Claude Desktop or Claude Code reading from servers
- **Configuration files**: How to tell Claude which tools to use
- **Security note**: Why MCPs running locally is important

### 4.3 Essential MCPs for Your Work

- **File system MCP**:
    
    - Reading/writing local files
    - CSV manipulation
    - Markdown document management
- **Google Workspace MCP**:
    
    - Google Sheets integration
    - Google Drive access
    - Gmail context (if needed)
- **Microsoft 365 MCP**:
    
    - Outlook calendar
    - OneDrive documents
    - Excel file access
- **Database MCPs** (overview):
    
    - SQLite for local data
    - PostgreSQL if you scale up
- **Brave Search MCP**: Real-time web information
    
- **Memory MCP**: Persistent knowledge across sessions
    

### 4.4 Case Studies: MCP in Action

- **Case Study 1**: Automating monthly data reports
    - Problem: 8 hours of manual spreadsheet work
    - Solution: File system MCP + Claude reasoning
    - Outcome: 30-minute process with Claude
- **Case Study 2**: Stakeholder communication tracking
    - Problem: Scattered emails and notes
    - Solution: Outlook MCP + Memory MCP
    - Outcome: Instant context recall for any stakeholder
- **Case Study 3**: Cross-referencing policy documents
    - Problem: Finding contradictions across 50+ files
    - Solution: File system MCP + semantic search
    - Outcome: Comprehensive compliance audit in hours

### 4.5 Installing Your First MCP Servers

- **Prerequisites check**: Node.js, npm (what they are, simple install)
- **Finding MCP servers**:
    - Official Anthropic repository
    - Community servers (modelcontextprotocol.io)
    - Quality indicators to look for
- **Step-by-step installation**:
    - Using `npx` to install (no permanent installation needed)
    - Creating the MCP configuration file
    - Testing the connection
- **Hands-on lab**: Install and configure:
    1. File system MCP
    2. Brave Search MCP
    3. One choice MCP relevant to your work

### 4.6 Claude Desktop + MCP Configuration

- **Locating the config file**: `claude_desktop_config.json`
- **Configuration syntax** (explained for non-technical):
    - JSON structure basics
    - Adding new MCP servers
    - Environment variables (simple explanation)
    - Debugging common errors
- **Testing your setup**:
    - Verifying MCPs are loaded
    - Running first MCP-powered query
    - Troubleshooting connection issues

### 4.7 Docker MCP Gateway (Advanced)

- **What is Docker?** (Container concept for non-technical)
- **Why Docker MCP Gateway matters**:
    - Running multiple MCPs easily
    - Isolation and security
    - Easier management
- **Setup overview** (guided):
    - Installing Docker Desktop
    - Using MCP Gateway
    - Configuring multiple services
- **When to use Gateway vs. direct MCPs**: Decision framework

---

## **MODULE 5: INTRODUCTION TO AGENTS**

_From tool-using AI to autonomous workers_

### 5.1 What Are AI Agents?

- **Agent vs. chatbot**: The critical distinction
- **Agent characteristics**:
    - Goal-oriented (not just responsive)
    - Tool-using capability
    - Multi-step planning
    - Environment interaction
    - Learning/adaptation (in context)
- **The agent spectrum**:
    - Simple: Single-task automation (move file when condition met)
    - Moderate: Multi-step workflows (research → analyze → report)
    - Complex: Multi-agent systems (orchestrated team of specialists)
- **Real-world analogies**: Virtual employee vs. virtual assistant

### 5.2 Agent Architecture Fundamentals

- **The core loop**:
    1. Perceive (receive input/observe environment)
    2. Think (plan next action using LLM)
    3. Act (use tool/execute action)
    4. Repeat until goal achieved
- **Components of an agent**:
    - LLM (the brain)
    - Tools/MCPs (the hands)
    - Memory (short-term and long-term)
    - Instructions/prompt (the personality and job description)
- **Visualization exercise**: Diagram your first simple agent

### 5.3 Multi-Agent Systems: The Power of Specialization

- **Why multiple agents?**:
    - Context window management (each agent has focused knowledge)
    - Specialization (expert agents for specific tasks)
    - Parallel processing (multiple agents working simultaneously)
    - Error isolation (one agent failing doesn't crash the system)
- **Multi-agent patterns**:
    - **Sequential**: Agent 1 completes → passes to Agent 2 → Agent 3
    - **Parallel**: Multiple agents work simultaneously, results merged
    - **Hierarchical**: Manager agent delegates to specialist agents
    - **Collaborative**: Agents negotiate and refine each other's work
- **Examples from your work**:
    - Data Collector Agent → Analysis Agent → Report Generator Agent
    - Scheduling Agent + Communication Agent working in parallel
    - Manager Agent coordinating Research + Writing + Compliance agents

### 5.4 Agent Design Principles

- **Single Responsibility**: Each agent should do one thing well
- **Clear interfaces**: Well-defined inputs and outputs
- **Fail gracefully**: What happens when an agent can't complete a task
- **Observable**: You should be able to see what agents are doing
- **Modular**: Easy to add, remove, or replace agents

### 5.5 Planning Your First Agent System

- **Use case identification**: Pick a real workflow from your work
- **Workflow decomposition**:
    - Break down into discrete steps
    - Identify decision points
    - Map dependencies
- **Agent design exercise**:
    - How many agents do you need?
    - What does each agent specialize in?
    - What tools does each agent need?
    - How do they communicate?
- **Practical example walkthrough**: Designing a "Monthly Compliance Report" agent system

---

## **MODULE 6: OPENAI AGENTKIT**

_Low-code agent building for rapid prototyping_

### 6.1 What is OpenAI AgentKit?

- **Overview**: Visual workflow builder for AI agents
- **Why it's valuable**: No coding required to build capable agents
- **What you can build**: API integrations, web automation, data workflows
- **Free tier capabilities**: What you can do without subscription

### 6.2 AgentKit Fundamentals

- **Creating an account and setup**
- **Interface tour**:
    - Workflow canvas
    - Node library
    - Testing panel
    - Deployment options
- **Core concepts**:
    - Nodes: Individual action blocks
    - Edges: Connections between nodes
    - Triggers: What starts your agent
    - Variables: Passing data between nodes

### 6.3 Building Your First Agent in AgentKit

- **Tutorial: "Automated Email Categorizer"**
    - Trigger: New email received
    - Node 1: Extract email content
    - Node 2: Claude analyzes category
    - Node 3: Move to appropriate folder
    - Testing and refinement
- **Understanding LLM nodes**:
    - Prompt configuration
    - Model selection
    - Output parsing

### 6.4 Connecting Tools and MCPs in AgentKit

- **Available integrations**:
    - HTTP requests (connecting to any API)
    - Database operations
    - File operations
    - Scheduling
- **MCP integration** (when available):
    - Adding MCP servers to AgentKit
    - Configuring permissions
    - Testing connections

### 6.5 Practical Agent Projects

- **Project 1**: Data validation agent
    - Monitors spreadsheet folder
    - Validates against business rules
    - Flags errors for review
- **Project 2**: Stakeholder update generator
    - Pulls data from multiple sources
    - Generates personalized updates
    - Drafts emails for review
- **Project 3**: Meeting prep assistant
    - Scans calendar for upcoming meetings
    - Gathers relevant documents
    - Creates briefing notes

### 6.6 AgentKit Best Practices

- **Error handling**: Designing robust workflows
- **Testing strategies**: How to validate agent behavior
- **Monitoring**: Keeping track of agent performance
- **Iteration**: Improving agents based on real-world use

---

## **MODULE 7: N8N - WORKFLOW AUTOMATION**

_Self-hosted agent orchestration_

### 7.1 What is n8n?

- **Overview**: Open-source workflow automation (like Zapier but more powerful)
- **Why n8n for agents**: Self-hosted, unlimited, integrates with AI
- **n8n vs AgentKit**: When to use which
- **Free tier options**: Cloud vs. self-hosted

### 7.2 Setting Up n8n

- **Installation options**:
    - n8n Cloud (easiest start)
    - Docker installation (recommended)
    - Windows installation guide
- **First login and configuration**
- **Understanding the interface**:
    - Workflow canvas
    - Node palette
    - Credentials management
    - Execution log

### 7.3 n8n Core Concepts

- **Nodes**: Building blocks of workflows
    - Trigger nodes (start workflows)
    - Action nodes (do things)
    - Logic nodes (make decisions)
- **Connections and data flow**
- **Credentials and authentication**
- **Variables and expressions**
- **Error workflows**: What happens when things fail

### 7.4 AI Integration in n8n

- **OpenAI nodes**: Using GPT models
- **HTTP Request node**: Connecting to Claude API
- **Webhook triggers**: Receiving data from external sources
- **Database nodes**: Storing and retrieving data

### 7.5 Building Multi-Agent Workflows in n8n

- **Tutorial: "Data Analysis Pipeline"**
    - Trigger: File uploaded to folder
    - Agent 1 (via Claude API): Extract key metrics
    - Agent 2 (via GPT-4): Generate insights
    - Agent 3: Create visualization
    - Final: Email summary report
- **Designing for reliability**:
    - Retry logic
    - Timeout handling
    - Notification on failure

### 7.6 Advanced n8n Patterns

- **Sub-workflows**: Reusable workflow components
- **Scheduling**: Time-based agent execution
- **Queue management**: Handling high-volume triggers
- **Conditional routing**: Different paths based on data

### 7.7 Practical n8n Projects

- **Project 1**: Automated data reconciliation
    - Compare multiple spreadsheets
    - Identify discrepancies
    - Generate exception report
- **Project 2**: Intelligent document router
    - New document arrives
    - AI categorizes and extracts metadata
    - Routes to appropriate team member
    - Updates tracking system
- **Project 3**: Stakeholder communication manager
    - Tracks communication history
    - Suggests optimal contact timing
    - Drafts personalized messages
    - Logs all interactions

---

## **MODULE 8: CLAUDE CODE - YOUR AGENT DEVELOPMENT ENVIRONMENT**

_Where power users become agent builders_

### 8.1 What is Claude Code?

- **Beyond coding**: Claude Code is for automation, not just programming
- **What makes it special**:
    - Native file system access
    - MCP integration out of the box
    - Project-aware context
    - Sub-agent coordination
- **Use cases for non-coders**:
    - Batch processing documents
    - Complex CSV transformations
    - Multi-file analysis
    - Building agent workflows

### 8.2 Installing and Configuring Claude Code

- **Prerequisites**:
    - Command line comfort (from Module 0)
    - Claude API key (getting one)
    - VS Code (already installed)
- **Installation walkthrough**:
    - Using npm to install Claude Code CLI
    - Initial configuration
    - Testing the installation
- **Configuration file**: `~/.clauderc` explained

### 8.3 Claude Code Fundamentals

- **How it works**:
    - You give instructions in natural language
    - Claude Code executes in your file system
    - You review and approve actions
- **Basic commands**:
    - Starting a session: `claude`
    - Working in a specific directory
    - Approving/rejecting actions
    - Reviewing what changed
- **Safety features**:
    - Approval mode (nothing happens without your OK)
    - Undo capabilities
    - Change preview

### 8.4 Working with Files in Claude Code

- **Practical tutorial: "CSV Data Cleaning"**
    - Task: "Clean this CSV file: remove duplicates, standardize dates, fix formatting"
    - Watching Claude Code work
    - Reviewing changes
    - Iterating to perfection
- **Markdown document management**:
    - Creating templates
    - Batch updating documents
    - Cross-referencing information
- **Multi-file operations**:
    - "Analyze all CSVs in this folder and create summary"
    - "Update all markdown files with new policy section"
    - "Cross-reference data across three spreadsheets"

### 8.5 Claude Skills in Claude Code

- **Bringing your Skills to the command line**:
    - Where Skills are stored
    - Referencing Skills in Claude Code
    - Creating Skills optimized for automation
- **Hands-on**: Convert a web-based skill to Claude Code workflow

### 8.6 MCPs in Claude Code

- **Configuration**: Setting up MCPs for CLI use
- **Available MCPs automatically work** with Claude Code
- **Power combinations**:
    - File system MCP + Claude reasoning
    - Database MCP + analysis task
    - Search MCP + research automation

### 8.7 Sub-Agents: Managing Context Windows

- **The context window challenge**: Even 200K tokens has limits
- **Sub-agent pattern**:
    - Main agent (orchestrator)
    - Sub-agents (specialists with focused context)
    - Communication between them
- **How sub-agents work in Claude Code**:
    - Creating specialized agent instructions
    - Passing work between agents
    - Aggregating results
- **Practical example**: "Policy Document Analysis"
    - Main agent: Coordinates overall task
    - Sub-agent 1: Analyzes Section A (uses 50K tokens)
    - Sub-agent 2: Analyzes Section B (uses 50K tokens)
    - Sub-agent 3: Analyzes Section C (uses 50K tokens)
    - Main agent: Synthesizes all findings

### 8.8 The `.claude` Directory: Your Agent Configuration Hub

- **What is `.claude`?**: Project-specific settings for Claude Code
- **Directory structure**:
    
    ```
    .claude/├── commands/         (Custom commands)├── prompts/          (Reusable prompts)├── skills/           (Project-specific skills)└── config.json       (Project settings)
    ```
    

### 8.9 Creating Custom Commands

- **What are commands?**: Shortcuts for common tasks
- **Command structure**:
    - Name (what you type)
    - Description (what it does)
    - Prompt (instructions to Claude)
- **Examples to build**:
    - `/analyze-weekly-data`: Runs your weekly analysis routine
    - `/prep-stakeholder-update`: Gathers info and drafts update
    - `/validate-compliance`: Checks documents against rules
- **Hands-on lab**: Create 3 commands for your recurring tasks

### 8.10 `agents.md` Files: Defining Your Agent Team

- **What is `agents.md`?**: Master instructions for Claude Code behavior in this project
- **Structure**:
    - Project context
    - Available tools and MCPs
    - Specialized sub-agents definitions
    - Workflow procedures
- **Writing effective `agents.md`**:
    - Clear role definitions
    - Tool usage guidelines
    - Expected outputs
    - Error handling instructions
- **Nesting agents**:
    - Main `agents.md` at project root
    - Specialized `agents.md` in subdirectories
    - How Claude Code uses the hierarchy

### 8.11 Reading Documentation Like a Pro

- **The Claude Code documentation** (where to find it)
- **How to read technical docs as a non-technical person**:
    - Focus on examples first
    - Skim the jargon, grasp the concepts
    - Use Claude to explain confusing parts
- **Community resources**:
    - GitHub discussions
    - Example projects to learn from
    - Common patterns library

### 8.12 Practical Claude Code Projects

- **Project 1**: Automated monthly reporting system
    - Pull data from multiple CSVs
    - Run analysis using Claude reasoning
    - Generate formatted report
    - Save to standard location
- **Project 2**: Document compliance checker
    - Read all policy documents
    - Check against compliance requirements
    - Generate exception report
    - Flag items needing human review
- **Project 3**: Stakeholder communication tracker
    - Scan emails and meeting notes
    - Extract stakeholder interactions
    - Maintain relationship log
    - Generate timely follow-up reminders

---

## **MODULE 9: RETRIEVAL AUGMENTED GENERATION (RAG)**

_Handling massive datasets beyond context windows_

### 9.1 The Problem RAG Solves

- **Context window limitation**: Even 2M tokens isn't infinite
- **Real-world scenario**: You have 500 policy documents, 10GB of data
- **The challenge**: How does AI access relevant information?
- **Old approach**: Manually find and copy → limited and tedious
- **RAG approach**: AI automatically finds and uses relevant information

### 9.2 How RAG Works (Simple Explanation)

- **The RAG process**:
    1. **Indexing**: Your documents are chunked and stored with "embeddings"
    2. **Query**: You ask a question
    3. **Retrieval**: System finds most relevant chunks
    4. **Generation**: LLM answers using retrieved context
- **Embeddings explained** (no math):
    - Converting text to numbers that capture meaning
    - Similar concepts have similar numbers
    - Allows "semantic search" (meaning-based, not keyword)
- **Visual analogy**: Library with smart librarian who fetches relevant books

### 9.3 RAG vs. Long Context Models

- **When to use each**:
    - **Long context** (Gemini 2M): ≤100 documents, need holistic view
    - **RAG**: 1000s of documents, need specific information
- **Hybrid approach**: RAG to find relevant docs → long context to analyze deeply

### 9.4 RAG Architecture Components

- **Document storage**: Where your files live
- **Vector database**: Stores embeddings (e.g., Pinecone, Chroma, FAISS)
- **Embedding model**: Converts text to vectors (e.g., OpenAI, Voyage)
- **LLM**: Generates answers using retrieved context
- **Retrieval logic**: How the system decides what's relevant

### 9.5 Simple RAG Setup (No-Code Options)

- **Option 1: NotebookLM** (easiest RAG-like experience)
    - Upload your documents
    - Ask questions
    - Limitations: ~50 sources, no customization
- **Option 2: ChatGPT with file upload**
    - Upload files to conversation
    - Limited to conversation context
- **Option 3: Glean, Hebbia** (commercial RAG platforms)
    - Enterprise-focused
    - Connect to your document repositories
    - Cost considerations

### 9.6 Building Your Own RAG System (Overview)

- **Why build your own?**: Control, privacy, customization
- **Tools needed**:
    - Vector database (we'll use ChromaDB - runs locally)
    - Embedding API (OpenAI or open-source)
    - LLM API (Claude or GPT)
    - Orchestration (LangChain or similar - we'll use simple version)

### 9.7 Practical RAG Implementation (Guided)

- **Use case**: "Search across all company policy documents"
- **Step 1**: Document preparation
    - Collecting your documents
    - Converting to plain text/markdown
    - Chunking strategy (how big should pieces be?)
- **Step 2**: Creating embeddings
    - Using Claude Code or Python script
    - Storing in ChromaDB
    - Testing retrieval quality
- **Step 3**: Query interface
    - Simple command-line query
    - Integration with Claude Code
    - Testing with real questions

### 9.8 RAG Best Practices

- **Chunking strategies**:
    - Too small: Loses context
    - Too large: Retrieves irrelevant info
    - Sweet spot: Usually 200-500 tokens
- **Metadata matters**:
    - Add document title, date, author to each chunk
    - Helps LLM understand context
    - Enables filtering (e.g., "only 2024 policies")
- **Query optimization**:
    - Retrieve more chunks than you think you need
    - Re-rank results by relevance
    - Use metadata filters to narrow search
- **Evaluation**:
    - Test with known questions
    - Verify correct information is retrieved
    - Iterate on chunk size and retrieval count

### 9.9 RAG in Multi-Agent Systems

- **Pattern**: Specialist agents with RAG access
    - **Compliance Agent**: RAG over policy documents
    - **Historical Data Agent**: RAG over past reports
    - **Stakeholder Agent**: RAG over communication history
- **Coordination**: Main agent routes questions to appropriate RAG agent

### 9.10 When NOT to Use RAG

- **Small document sets**: Just use long context
- **Highly structured data**: Use database queries instead
- **Real-time data**: Use APIs/MCPs for live data
- **Exact search**: Traditional search engines work better

---

## **MODULE 10: INTEGRATION & ORCHESTRATION**

_Bringing it all together into production systems_

### 10.1 Designing Your Personal AI Infrastructure

- **Taking inventory**:
    - Your recurring tasks (from Module 0)
    - Which tools you've learned
    - What MCPs you have access to
- **System design exercise**:
    - Map tasks to tools (web Claude, Claude Code, AgentKit, n8n)
    - Identify dependencies
    - Plan data flows
- **Your AI stack**:
    - Daily work: Claude.ai with Projects
    - Complex analysis: Claude Code with MCPs
    - Automation: AgentKit or n8n
    - Massive data: RAG system
    - Quick research: Perplexity, NotebookLM

### 10.2 Multi-Tool Workflows

- **Example workflow**: "Monthly stakeholder report"
    - **n8n**: Schedules job, pulls data from multiple sources
    - **Claude Code**: Processes and analyzes data
    - **Claude.ai**: Final review and refinement (human-in-loop)
    - **n8n**: Distributes final report
- **Building your first integrated workflow**:
    - Choose a real task
    - Break into stages
    - Assign each stage to appropriate tool
    - Connect the pieces
    - Test end-to-end

### 10.3 Human-in-the-Loop Design

- **Why full automation isn't always best**:
    - High-stakes decisions need human judgment
    - Building trust in AI systems
    - Learning from AI suggestions
- **Where to add human review**:
    - Before sending communications
    - Final approval on reports
    - Exception handling
    - Quality spot-checks
- **Practical patterns**:
    - AI drafts → human edits → AI finalizes
    - AI flags issues → human investigates → AI documents
    - AI provides options → human chooses → AI executes

### 10.4 Monitoring and Maintenance

- **What to monitor**:
    - Agent success/failure rates
    - Execution times (is it slowing down?)
    - Cost (API usage)
    - Output quality (spot-checking)
- **Setting up alerts**:
    - Agent failed notification
    - Unusual patterns detected
    - Human review required
- **Regular maintenance**:
    - Update agent instructions based on learnings
    - Refresh RAG databases with new documents
    - Review and optimize workflows
    - Update MCPs and dependencies

### 10.5 Security and Privacy Considerations

- **Data sensitivity**:
    - What should never leave your computer
    - When cloud AI is appropriate
    - Local-only processing options
- **Access controls**:
    - API key management
    - MCP permissions
    - File system access boundaries
- **Best practices**:
    - Regular credential rotation
    - Audit logs for agent actions
    - Testing in sandbox before production

### 10.6 Scaling Your Systems

- **From personal to team**:
    - Sharing agents with colleagues
    - Centralized RAG systems
    - Team-wide MCP servers
- **Performance optimization**:
    - Caching frequent queries
    - Parallel agent execution
    - Batch processing strategies
- **Cost management**:
    - Choosing the right model for each task
    - Monitoring token usage
    - Free tier optimization

### 10.7 Troubleshooting Common Issues

- **Agent isn't working**:
    - Check MCP connections
    - Verify API keys
    - Review error logs
    - Test components in isolation
- **Results aren't good enough**:
    - Refine prompts/instructions
    - Adjust retrieval settings (RAG)
    - Try different model
    - Add examples to training
- **System is too slow**:
    - Profile where time is spent
    - Use faster models for simple tasks
    - Implement caching
    - Parallelize independent steps

---

## **MODULE 11: CAPSTONE PROJECT**

_Build your comprehensive AI work system_

### 11.1 Project Planning

- **Selecting your capstone scope**:
    - Choose 3-5 of your most time-consuming tasks
    - Tasks should span different tools (web, code, automation)
    - Include at least one multi-agent workflow
- **Requirements definition**:
    - What does success look like?
    - What are the inputs?
    - What are the outputs?
    - Where does human review happen?

### 11.2 Architecture Design

- **System diagram**:
    - Draw out your entire system
    - Show data flows
    - Identify all tools and agents
    - Mark human-in-the-loop points
- **Component list**:
    - Claude Projects needed
    - Claude Code scripts
    - AgentKit/n8n workflows
    - MCPs required
    - RAG databases (if applicable)

### 11.3 Implementation Phase

- **Week 1**: Core foundation
    - Set up all Projects
    - Configure MCPs
    - Create Skills
    - Test basic functionality
- **Week 2**: Automation workflows
    - Build AgentKit/n8n flows
    - Create Claude Code scripts
    - Implement sub-agents
    - Test individual components
- **Week 3**: Integration
    - Connect all pieces
    - Test end-to-end workflows
    - Handle edge cases
    - Optimize performance
- **Week 4**: Polish and documentation
    - User guide for yourself
    - Maintenance procedures
    - Troubleshooting guide
    - Lessons learned

### 11.4 Testing and Validation

- **Test scenarios**:
    - Happy path (everything works)
    - Error cases (what if data is missing?)
    - Edge cases (unusual but valid inputs)
    - Load testing (can it handle volume?)
- **Quality checks**:
    - Output accuracy
    - Time savings measurement
    - User experience (is it actually easier?)

### 11.5 Documentation and Handoff

- **System documentation**:
    - Overview of architecture
    - How to use each component
    - Configuration files and where to find them
    - Maintenance schedule
- **Knowledge transfer** (if sharing with team):
    - Recorded demo
    - User guide
    - Troubleshooting FAQ
    - Contact for questions (you!)

### 11.6 Iteration and Improvement

- **Collecting feedback**:
    - What works well?
    - What's frustrating?
    - What's missing?
- **Version 2 planning**:
    - Quick wins (easy improvements)
    - Major enhancements
    - New capabilities to add
- **Continuous learning**:
    - New MCPs to explore
    - Model updates to leverage
    - Community patterns to adopt

---

## **MODULE 12: STAYING CURRENT & NEXT STEPS**

_The AI landscape evolves rapidly_

### 12.1 Keeping Up with AI Developments

- **Resources to follow**:
    - Anthropic blog (Claude updates)
    - OpenAI blog (GPT updates)
    - r/ClaudeAI, r/LocalLLaMA communities
    - MCP server directory (new integrations)
- **What to pay attention to**:
    - New models and capabilities
    - MCP server releases
    - Integration updates
    - Best practice evolutions
- **What to ignore** (for now):
    - Hype and speculation
    - Cutting-edge research (not production-ready)
    - Platform debates (use what works for you)

### 12.2 Advanced Topics (Future Learning)

- **If you want to go deeper into agents**:
    - LangChain / LangGraph
    - AutoGen framework
    - CrewAI
- **If you want custom MCPs**:
    - Basic Python or Node.js
    - MCP SDK documentation
    - Contributing to open-source MCPs
- **If you want production-grade systems**:
    - LLMOps (monitoring, versioning)
    - Kubernetes for agent orchestration
    - Vector database optimization

### 12.3 Community and Collaboration

- **Sharing your learnings**:
    - Write about your use cases
    - Share agent templates
    - Contribute to MCP ecosystem
- **Finding collaborators**:
    - Discord servers (Anthropic, MCP)
    - LinkedIn AI communities
    - Local meetups (AI in business)

### 12.4 Ethical Considerations

- **Using AI responsibly**:
    - Bias awareness and mitigation
    - Transparency with stakeholders
    - Data privacy vigilance
    - Human oversight for important decisions
- **Environmental considerations**:
    - Choosing efficient models
    - Batch processing vs. real-time
    - Local compute when appropriate

### 12.5 Your AI Learning Path Forward

- **Quarterly review ritual**:
    - What's working in your system?
    - What new capabilities are available?
    - What should you add/remove/change?
- **Experiment budget**:
    - Set aside time to try new tools
    - Fail fast on things that don't work
    - Document what you learn
- **Teaching others**:
    - Best way to solidify your knowledge
    - Builds your reputation
    - Creates a support network

---

## **APPENDICES**

### Appendix A: Tool Reference Guide

- Quick reference for each tool
- When to use what
- Cost comparison
- Capability matrix

### Appendix B: Prompt Library

- Templates for common tasks
- Specialized prompts for your work domain
- Debugging prompts
- Meta-prompts for improvement

### Appendix C: MCP Server Directory

- Curated list of essential MCPs
- Installation instructions
- Configuration examples
- Troubleshooting common issues

### Appendix D: Glossary

- All technical terms explained simply
- Analogies for complex concepts
- Common abbreviations

### Appendix E: Troubleshooting Guide

- Common error messages and solutions
- "When nothing works" checklist
- How to ask for help effectively
- Diagnostic procedures

### Appendix F: Resource Links

- Official documentation
- Community forums
- Video tutorials
- Example projects

---

## **COURSE STRUCTURE NOTES**

### Suggested Learning Path

1. **Modules 0-3**: Foundation (2-3 weeks)
    - Focus: Understanding and using Claude effectively
    - Milestone: Comfortable with prompting and Claude Projects
2. **Modules 4-5**: Tools and concepts (2 weeks)
    - Focus: MCP setup, agent concepts
    - Milestone: Have working MCPs, understand agent architecture
3. **Modules 6-7**: Automation platforms (2 weeks)
    - Focus: AgentKit and n8n
    - Milestone: Built at least one automated workflow
4. **Module 8**: Claude Code mastery (2-3 weeks)
    - Focus: Local agent development
    - Milestone: Comfortable running multi-step automations
5. **Module 9**: RAG (1 week)
    - Focus: Handling large datasets
    - Milestone: Understand when/how to use RAG
6. **Modules 10-12**: Integration and beyond (2-3 weeks)
    - Focus: Building comprehensive systems
    - Milestone: Capstone project complete

### Total Time Estimate

- **Fast track**: 8-10 weeks (10-15 hours/week)
- **Comfortable pace**: 12-16 weeks (5-8 hours/week)
- **Deep dive**: 20-24 weeks (5 hours/week with lots of experimentation)

### Prerequisites for Each Module

- Each module clearly states what you need from previous modules
- "Can skip if..." conditions for non-essential modules
- Checkpoint exercises to verify readiness

---

**END OF OUTLINE**

This outline takes someone from "using ChatGPT like Google" to building sophisticated multi-agent systems with proper context management, tool integration, and production-ready workflows. Every concept builds on previous ones, with ample hands-on practice throughout.