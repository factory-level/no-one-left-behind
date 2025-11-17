# 6.2 Setup & Your First Agent: From Zero to Working AI Assistant

## What You'll Accomplish
By the end of this section, you'll have AgentKit installed and a working agent that can help with a real business task.

## The Assembly Line Analogy

Think of building your first agent like setting up a new workstation in a factory:
- **First**: Install the equipment (AgentKit setup)
- **Second**: Train a new worker (configure your agent)
- **Third**: Give them their first assignment (test functionality)
- **Fourth**: Watch them work independently

## Prerequisites Check

Before we start, ensure you have:
- ✅ OpenAI account with API access
- ✅ Computer with internet connection
- ✅ Basic file navigation skills (from Module 0)
- ✅ Email access for verification steps

## Step 1: AgentKit Account Setup

### Creating Your AgentKit Account

1. **Visit the AgentKit Portal**
   - Go to `https://agentkit.openai.com`
   - Click "Get Started"

2. **Link Your OpenAI Account**
   - Choose "Sign in with OpenAI"
   - Authorize the connection
   - Verify your email address

3. **Choose Your Plan**
   - Start with "Developer Free Tier"
   - Provides 100 agent actions per month
   - Perfect for learning and testing

### Understanding Your Dashboard

When you first log in, you'll see:

```
┌─ AgentKit Dashboard ─────────────────────┐
│ ┌─ Quick Start ─┐  ┌─ Templates ──────┐ │
│ │ • New Agent   │  │ • Email Helper    │ │
│ │ • From Template│  │ • Data Processor │ │
│ │ • Import      │  │ • Task Manager   │ │
│ └───────────────┘  └──────────────────┘ │
│ ┌─ Recent Activity ─────────────────────┐ │
│ │ No agents created yet                 │ │
│ └───────────────────────────────────────┘ │
└─────────────────────────────────────────┘
```

## Step 2: Understanding Agent Components

### The Three Essential Parts

Every agent needs these components:

#### 1. Identity (Who)
- **Name**: What you call your agent
- **Role**: What job they perform
- **Personality**: How they communicate

#### 2. Instructions (What)
- **Primary task**: Main responsibility
- **Secondary tasks**: Supporting activities
- **Constraints**: What they cannot do

#### 3. Tools (How)
- **Input sources**: Where they get information
- **Output destinations**: Where they send results
- **Processing capabilities**: What they can do with data

## Step 3: Building Your First Agent

### Choosing Your First Project

Start with something simple but valuable:
- ✅ **Email summarizer** (good first choice)
- ✅ **Task organizer**
- ✅ **Meeting note formatter**
- ❌ Complex data analysis (save for later)
- ❌ Customer-facing interactions (too advanced)

### Example: Building an Email Prioritizer Agent

Let's create an agent that helps you prioritize your daily emails.

#### Step 1: Create New Agent

1. Click "New Agent" on your dashboard
2. Choose "Start from Scratch" (not template yet)
3. Fill in basic information:

```yaml
Agent Name: Email Priority Assistant
Description: Helps prioritize daily email inbox
Category: Productivity
```

#### Step 2: Define Agent Identity

```yaml
Role: Professional Email Analyst
Personality Traits:
  - Concise and clear
  - Focuses on urgency and importance
  - Professional tone
  - Actionable recommendations
```

#### Step 3: Write Agent Instructions

```markdown
## Your Primary Job
Analyze emails in my inbox and categorize them by priority:
- HIGH: Requires immediate action (same day)
- MEDIUM: Important but can wait (2-3 days)
- LOW: Informational or non-urgent (when time permits)

## For Each Email, Provide:
1. Priority level (HIGH/MEDIUM/LOW)
2. One-sentence reason for priority
3. Suggested action (Reply, Schedule, File, etc.)
4. Estimated time needed

## Guidelines:
- Emails from my boss = always HIGH priority
- Customer complaints = HIGH priority
- Internal meetings = MEDIUM priority
- Newsletters/promotions = LOW priority
- Consider deadlines mentioned in content

## Output Format:
Create a simple priority list I can review in 2 minutes each morning.
```

#### Step 4: Configure Tools and Permissions

For this first agent, we'll use:
- **Input**: Email reading capability
- **Output**: Text summary report
- **Permissions**: Read-only access to inbox

```yaml
Tools Enabled:
  - Email Reader (Gmail/Outlook)
  - Text Generator
  - Priority Classifier

Security Settings:
  - Read-only access
  - No email sending capability
  - No attachment downloading
```

#### Step 5: Set Automation Schedule

```yaml
Trigger: Every weekday at 8:00 AM
Action: Scan inbox from last 24 hours
Output: Send priority report to me
Duration: Stop after 30 days (review period)
```

## Step 4: Testing Your Agent

### The Test Run Process

1. **Start Small**: Give your agent 5-10 test emails
2. **Review Results**: Check if priorities make sense
3. **Adjust Instructions**: Refine based on what you see
4. **Scale Up**: Let it process your full inbox

### What to Look For

#### Good Signs ✅
- Priorities match your expectations
- Reasons make logical sense
- Format is easy to read
- Completes tasks within time limit

#### Warning Signs ⚠️
- Inconsistent priority assignments
- Takes too long to process
- Output format is confusing
- Missing important context

### Making Adjustments

Common first-agent improvements:

```markdown
Before: "Categorize my emails"
After: "Categorize emails using these specific criteria..."

Before: "High priority emails"
After: "HIGH: Needs response within 4 hours"

Before: "Send me a report"
After: "Send a 5-item bulleted list with action items"
```

## Step 5: Monitoring and Iteration

### Week 1 Checklist

- [ ] Agent runs successfully each day
- [ ] Priority assignments are 80%+ accurate
- [ ] You save at least 15 minutes daily
- [ ] No security or access issues
- [ ] Output format works for your workflow

### Improvement Questions

1. **Accuracy**: Are priorities correct 8 out of 10 times?
2. **Usefulness**: Do you actually use the output?
3. **Efficiency**: Does it save more time than it takes to review?
4. **Reliability**: Does it run consistently without errors?

## Common First-Agent Mistakes

### Mistake 1: Too Complex Initially
**Problem**: Trying to automate your entire workflow at once
**Solution**: Start with one specific task

### Mistake 2: Vague Instructions
**Problem**: "Help me be more productive"
**Solution**: "Categorize my emails by these specific criteria..."

### Mistake 3: No Success Metrics
**Problem**: Not knowing if the agent is actually helping
**Solution**: Track time saved, tasks completed, accuracy rate

### Mistake 4: Set-and-Forget
**Problem**: Never reviewing or improving the agent
**Solution**: Weekly 10-minute review sessions

## Step 6: Preparing for Scale

### What You've Learned
- How to translate business needs into agent instructions
- The importance of specific, measurable tasks
- Testing and iteration cycles
- Basic security and permission management

### Next Steps
- Create 2-3 similar simple agents
- Learn to use pre-built templates (Section 6.3)
- Explore more complex automation scenarios

## Troubleshooting Your First Setup

### Can't Connect to Email
**Issue**: Agent can't access your inbox
**Solutions**:
1. Check OAuth permissions in your email provider
2. Verify AgentKit has necessary scopes
3. Try disconnecting and reconnecting

### Agent Doesn't Run on Schedule
**Issue**: No automated reports arriving
**Solutions**:
1. Check your timezone settings
2. Verify trigger conditions are met
3. Look for error messages in agent logs

### Poor Quality Results
**Issue**: Agent priorities don't match expectations
**Solutions**:
1. Add more specific examples in instructions
2. Include edge case scenarios
3. Refine your criteria definitions

## Security Best Practices for First Agents

### Start with Read-Only
- Never give write permissions initially
- Test thoroughly before enabling actions
- Use sandbox environments when possible

### Review Access Regularly
- Check what data your agent can see
- Revoke unused permissions
- Monitor for unusual activity

### Keep Instructions Private
- Don't include sensitive information in agent descriptions
- Use variables for confidential data
- Regular review shared agents for exposure

## Your First Agent Success Framework

### Day 1: Setup and Basic Test
- Install and configure agent
- Run manual test with 3-5 items
- Verify basic functionality

### Week 1: Daily Monitoring
- Check agent output each morning
- Note accuracy and usefulness
- Make small adjustments as needed

### Week 2: Optimization
- Analyze patterns in results
- Refine instructions based on learning
- Consider adding new capabilities

### Week 3: Expansion Planning
- Identify next automation opportunity
- Plan second agent project
- Document lessons learned

---

**Ready to explore pre-built templates?** In Section 6.3, we'll discover how to use AgentKit's ready-made solutions to fast-track your automation journey.