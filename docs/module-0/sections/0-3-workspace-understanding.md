# 0.3 Understanding Your Workspace

## File Organization for AI Work

### Project Folder Structure

```
ai-projects/
├── data/             # Raw and processed data files
│   ├── csv/
│   ├── json/
│   └── xlsx/
├── prompts/          # Saved prompt templates
│   ├── analysis/
│   ├── writing/
│   └── research/
├── agents/           # Agent configurations
│   ├── skills/
│   └── workflows/
└── outputs/          # Generated documents and results
```

### Naming Conventions AI Systems Understand

!!! tip "Naming Best Practices"
    - Use lowercase
    - Separate words with hyphens
    - Include date or version
    - Be descriptive but concise

Examples:
- `quarterly-sales-analysis-2024-q1.csv`
- `customer-communication-template-v2.md`
- `research-summary-climate-tech.txt`

## Document Types in AI Workflows

### Markdown (.md)

!!! warning "Why Markdown is Critical for This Course"
    **Markdown is the universal language for AI work, and you'll use it throughout this entire course.**
    
    - **Every module uses Markdown**: From writing prompts in Module 1 to creating Claude Skills in Module 3, Markdown is your primary tool
    - **AI systems excel at Markdown**: LLMs understand and generate Markdown naturally—it's how they communicate best
    - **Universal compatibility**: Markdown works everywhere—GitHub, documentation sites, AI tools, and more
    - **Future-proof your work**: Skills, prompts, and documentation in Markdown will work with any AI system you use
    
    **Master Markdown now.** If you're not comfortable with it yet, this is the time to learn. You'll use it in every exercise and project from here on out.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; margin: 1em 0;">
  <iframe 
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    src="https://www.youtube.com/embed/t9PiNRSQ_BU" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
  </iframe>
</div>

- Universal AI language
- Supports rich formatting
- Easy to read and process
- Used for documentation, prompts, and agent instructions

=== "Example Markdown"
    ```markdown
    # Project Research Report

    ## Executive Summary

    ### Key Findings
    - **Trend 1**: Emerging AI technologies
    - **Trend 2**: Automation capabilities

    ### Recommendations
    1. Invest in agent-based workflows
    2. Develop in-house AI skills
    ```

### CSV (Comma-Separated Values)
- Perfect for tables
- Easily manipulated by AI
- Lightweight and universal

=== "Sample CSV"
    ```csv
    name,role,department,productivity_score <--- Heading Row
    jane_doe,analyst,research,8.5 <--- Like Excel Rows
    john_smith,manager,operations,7.2 <--- Like Excel Rows
    ```

### JSON (JavaScript Object Notation)
- Structured data format
- Native to most programming languages
- Great for configuration and data exchange

=== "JSON Example"
    ```json
    {
        "project": "AI Workflow Automation",
        "team_members": [
            {"name": "Alice", "role": "Lead Researcher"},
            {"name": "Bob", "role": "AI Engineer"}
        ],
        "status": "In Progress"
    }
    ```

### YAML (Yet Another Markup Language)
- Human-readable configuration
- Used for agent instructions and workflows
- Supports complex nested structures

=== "YAML Agent Configuration"
    ```yaml
    agent:
      name: research_assistant
      goals:
        - Collect relevant research papers
        - Summarize key findings
      tools:
        - academic_search_mcp
        - document_analysis_skill
    ```

## Checkpoint Exercise: Workspace Setup

1. Create the project folder structure in your home directory
2. Create sample files in each document type
3. Practice renaming files following the guidelines
4. Take a screenshot of your organized workspace

### Reflection Questions
- How might these document types help in AI workflows?
- What recurring tasks in your work could benefit from this organization?