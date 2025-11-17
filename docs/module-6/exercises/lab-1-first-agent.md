# Lab 1: Building Your First AgentKit Agent - Email Task Manager

## Lab Overview
**Duration:** 2-3 hours
**Difficulty:** Beginner
**Prerequisites:** AgentKit account setup completed

In this hands-on lab, you'll build your first working agent that processes and prioritizes your daily emails, turning inbox chaos into organized action items.

## Learning Objectives
By the end of this lab, you will:
- ✅ Create a functional AgentKit agent from scratch
- ✅ Configure agent instructions and personality
- ✅ Set up email integration and permissions
- ✅ Test and iterate on agent performance
- ✅ Understand basic agent monitoring and improvement

## The Business Problem

**Your Current Email Situation:**
- 50-100 emails per day across multiple inboxes
- Important messages buried in promotional emails
- Difficulty identifying urgent vs. routine requests
- 2-3 hours daily spent managing email

**What You'll Build:**
An intelligent email assistant that:
- Categorizes emails by priority (High/Medium/Low)
- Identifies action items and deadlines
- Provides daily email briefings
- Flags potential issues or opportunities

## Part 1: Agent Design and Planning (30 minutes)

### Step 1: Define Your Email Priorities

Before building your agent, establish clear criteria for email importance:

**High Priority Emails Include:**
- [ ] Messages from your direct manager or CEO
- [ ] Customer complaints or urgent requests
- [ ] Time-sensitive project communications
- [ ] Meeting invitations for this week
- [ ] Security alerts or system notifications

**Medium Priority Emails Include:**
- [ ] Internal team communications
- [ ] Vendor or partner correspondence
- [ ] Non-urgent project updates
- [ ] Meeting requests for next week
- [ ] Industry news from trusted sources

**Low Priority Emails Include:**
- [ ] Marketing newsletters and promotions
- [ ] Social media notifications
- [ ] Automated reports and summaries
- [ ] Conference and event invitations
- [ ] General company announcements

### Step 2: Map Your Current Email Sources

Document your email landscape:

```yaml
Primary Inboxes:
  Work Email: ___________________
  Personal Email: _______________
  Other: _______________________

Key Senders to Monitor:
  Boss/Manager: _________________
  Direct Reports: _______________
  Important Clients: ____________
  Key Vendors: __________________

Email Volume:
  Daily Average: ________________
  Peak Days: ____________________
  Busiest Time: _________________
```

### Step 3: Design Your Agent Personality

Your agent should reflect your communication style:

**Agent Name:** ________________________
**Professional Tone:** Formal / Business Casual / Friendly
**Communication Style:** Concise / Detailed / Balanced
**Notification Preference:** Instant / Hourly / Daily Summary

## Part 2: Agent Creation in AgentKit (45 minutes)

### Step 1: Create New Agent

1. **Log into AgentKit Dashboard**
   - Navigate to your AgentKit workspace
   - Click "Create New Agent"
   - Select "Start from Scratch"

2. **Basic Agent Information**
   ```yaml
   Agent Name: Email Priority Assistant
   Description: Intelligent email categorization and briefing system
   Category: Productivity
   Department: Personal/Administrative
   ```

### Step 2: Configure Agent Identity

**Agent Role Definition:**
```markdown
# Agent Identity
Role: Executive Email Assistant
Reporting To: [Your Name]
Primary Function: Email intelligence and prioritization

# Personality Traits
- Professional and efficient
- Focuses on urgency and business impact
- Provides clear, actionable insights
- Respects confidentiality and privacy

# Communication Style
- Concise but thorough summaries
- Uses bullet points for clarity
- Highlights deadlines and action items
- Maintains consistent tone
```

### Step 3: Write Core Instructions

Copy this template and customize for your needs:

```markdown
## Your Primary Responsibilities

1. **Email Categorization**
   - Analyze all incoming emails in my inbox
   - Assign priority levels (HIGH/MEDIUM/LOW)
   - Identify action items and deadlines
   - Flag emails requiring immediate attention

2. **Priority Criteria**

   HIGH Priority (Immediate Attention):
   - Emails from: [your manager's email], [key client emails]
   - Subject contains: "URGENT", "ASAP", "Emergency", "Problem"
   - Customer complaints or negative feedback
   - Meeting invitations for today/tomorrow
   - Security or system alerts

   MEDIUM Priority (Same Day Response):
   - Team communications requiring input
   - Project updates affecting deadlines
   - Vendor communications about active projects
   - Meeting requests for this week
   - Contract or legal documents

   LOW Priority (When Time Permits):
   - Newsletters, marketing emails
   - Social media notifications
   - General company announcements
   - Conference invitations
   - Automated reports

3. **Daily Summary Format**

   Generate a morning briefing with:
   - High priority items requiring immediate action
   - Medium priority items for today's agenda
   - Action items with deadlines
   - Meeting invitations to respond to
   - Key information I should know about

## Processing Guidelines

- Never forward or reply to emails without explicit instruction
- Summarize email content, don't include full text
- Identify the main ask or action item in each email
- Note if sender is internal vs. external
- Highlight any deadlines or time-sensitive elements
- Flag emails that might need legal or HR review

## Output Format

For each email, provide:
**From:** Sender name and relationship (boss, client, team, vendor)
**Priority:** HIGH/MEDIUM/LOW
**Summary:** One sentence describing the email's purpose
**Action Required:** What I need to do (Reply, Schedule, Review, etc.)
**Deadline:** Any mentioned timeframes
**Notes:** Important context or flags
```

### Step 4: Configure Email Access

**Email Integration Setup:**
1. **Connect Your Email Provider**
   - For Gmail: OAuth authentication
   - For Outlook: Microsoft 365 integration
   - Grant read-only permissions initially

2. **Set Monitoring Parameters**
   ```yaml
   Monitoring Scope:
     - Inbox only (not sent items, drafts)
     - Last 24 hours for daily briefings
     - All unread emails for real-time alerts

   Exclusions:
     - Promotional/Social tabs (Gmail)
     - Junk/Spam folders
     - Deleted items
   ```

3. **Security Settings**
   ```yaml
   Permissions:
     - Read email content: Yes
     - Access attachments: No (initially)
     - Send emails: No
     - Modify emails: No

   Privacy:
     - Log interactions: Yes
     - Store email content: 7 days maximum
     - Encrypt stored data: Yes
   ```

## Part 3: Testing and Validation (45 minutes)

### Step 1: Initial Test with Sample Emails

Create test scenarios using your actual emails:

**Test Case 1: High Priority Detection**
1. Find an email from your manager or important client
2. Run agent on this email
3. Verify it categorizes as HIGH priority
4. Check if action items are identified correctly

**Test Case 2: Low Priority Filtering**
1. Find a newsletter or promotional email
2. Run agent on this email
3. Verify it categorizes as LOW priority
4. Ensure it's summarized briefly

**Test Case 3: Meeting Invitation Handling**
1. Find a meeting invitation email
2. Run agent on this email
3. Check priority assignment based on timing
4. Verify action items (Accept/Decline/Reschedule)

### Step 2: Run Daily Briefing Test

1. **Generate Morning Summary**
   - Let agent analyze your inbox from past 24 hours
   - Review the summary format and content
   - Check if priorities align with your expectations

2. **Evaluate Summary Quality**
   ```yaml
   Quality Checklist:
     - Are high priority items actually urgent? ___
     - Are action items clearly identified? ___
     - Is the summary length appropriate? ___
     - Does the tone match your preferences? ___
     - Are deadlines accurately captured? ___
   ```

### Step 3: Iteration and Refinement

Based on test results, refine your agent:

**Common Adjustments:**

1. **Priority Criteria Refinement**
   ```markdown
   If agent marked newsletter as HIGH:
   Add to LOW priority criteria: "emails from newsletter domains"

   If agent missed urgent customer email:
   Add to HIGH priority criteria: specific customer domains
   ```

2. **Summary Length Optimization**
   ```markdown
   Too verbose: "Provide one-sentence summaries maximum"
   Too brief: "Include key details and context"
   ```

3. **Action Item Clarity**
   ```markdown
   Add instruction: "For each action item, specify:
   - What needs to be done
   - Who should do it (me, delegate, or team)
   - When it should be completed"
   ```

## Part 4: Production Deployment (30 minutes)

### Step 1: Schedule Automated Processing

**Daily Briefing Schedule:**
```yaml
Trigger: Every weekday at 7:30 AM
Action: Generate email priority briefing
Delivery: Send summary to your preferred method
Duration: Continuous (review monthly)
```

**Real-Time Monitoring:**
```yaml
Trigger: High priority emails detected
Action: Immediate notification
Delivery: Push notification or SMS
Threshold: Only emails scoring 8+ priority points
```

### Step 2: Set Up Monitoring Dashboard

Track your agent's performance:
```yaml
Daily Metrics:
  - Total emails processed
  - Priority distribution (H/M/L)
  - Action items identified
  - Response time

Weekly Metrics:
  - Priority accuracy rate
  - Time saved on email management
  - Action item completion rate
  - User satisfaction score
```

### Step 3: Create Feedback Loop

**Weekly Agent Review Process:**
1. **Monday morning**: Review previous week's performance
2. **Check accuracy**: Were priority assignments correct?
3. **Note patterns**: What types of emails were misclassified?
4. **Update instructions**: Refine criteria based on learnings
5. **Test changes**: Verify improvements with sample emails

## Part 5: Success Measurement (15 minutes)

### Track Your Improvements

**Before Agent (Baseline Week):**
```yaml
Time Spent on Email Daily: _______ hours
High-importance emails missed: _______ per week
Average response time to urgent emails: _______ hours
Stress level with email management (1-10): _______
```

**After Agent (Week 2-3):**
```yaml
Time Spent on Email Daily: _______ hours
High-importance emails missed: _______ per week
Average response time to urgent emails: _______ hours
Stress level with email management (1-10): _______
```

**Calculate ROI:**
```
Time saved per day: _______ minutes
Monthly time savings: _______ hours
Value of time saved: $_______ (hourly rate × hours)
Agent cost: $_______ per month
Monthly ROI: _______ % ((value - cost) / cost × 100)
```

## Troubleshooting Common Issues

### Issue 1: Agent Misclassifies Email Priorities

**Symptoms:**
- Important emails marked as low priority
- Spam emails marked as high priority
- Inconsistent categorization

**Solutions:**
1. **Add Specific Examples**
   ```markdown
   Add to instructions:
   "Examples of HIGH priority:
   - Email from john.doe@company.com about project deadlines
   - Customer complaints containing words 'unhappy', 'cancel', 'refund'"
   ```

2. **Refine Sender Rules**
   ```markdown
   Create whitelist: "Always HIGH priority from these domains: company.com, keyclient.com"
   Create blacklist: "Always LOW priority from these domains: newsletter.com, promo.email"
   ```

### Issue 2: Summaries Are Too Long or Too Short

**Too Long (>100 words per email):**
```markdown
Add constraint: "Limit summaries to 25 words maximum per email"
```

**Too Short (missing context):**
```markdown
Add requirement: "Include WHO (sender), WHAT (main request), WHEN (any deadlines)"
```

### Issue 3: Missing Action Items

**Solutions:**
1. **Enhance Action Detection**
   ```markdown
   "Identify action items by looking for:
   - Questions requiring responses
   - Requests for information or documents
   - Meeting scheduling needs
   - Approval or decision requests
   - Follow-up commitments"
   ```

2. **Add Action Categories**
   ```markdown
   "Categorize actions as:
   - REPLY (needs email response)
   - SCHEDULE (needs calendar action)
   - RESEARCH (needs information gathering)
   - DELEGATE (needs assignment to team member)"
   ```

## Next Steps and Extensions

### Immediate Improvements (This Week)
- [ ] Fine-tune priority criteria based on first week's performance
- [ ] Add integration with calendar for meeting conflict detection
- [ ] Set up mobile notifications for high-priority emails

### Advanced Features (Next Month)
- [ ] Integration with task management system (Asana, Monday, etc.)
- [ ] Automatic response drafting for common inquiries
- [ ] Customer sentiment analysis for support emails
- [ ] Meeting scheduling assistance

### Integration Preparation (Module 7)
- [ ] Document successful email processing patterns for n8n workflows
- [ ] Identify email triggers for broader automation workflows
- [ ] Plan customer service automation expansion

## Lab Completion Checklist

- [ ] Agent successfully created and configured
- [ ] Email integration working properly
- [ ] Priority classification functioning accurately
- [ ] Daily briefing format meets your needs
- [ ] Testing completed with real emails
- [ ] Performance monitoring established
- [ ] Feedback loop created for continuous improvement
- [ ] Initial ROI measurement completed

**Estimated Time Savings:** _______ hours per week
**Agent Accuracy Rate:** _______ %
**User Satisfaction:** _______ / 10

---

**Congratulations!** You've built your first intelligent agent. This email assistant will serve as the foundation for more complex automation as you progress through the course. In Lab 2, we'll build on this success by creating a business process automation agent that handles complete workflows from start to finish.