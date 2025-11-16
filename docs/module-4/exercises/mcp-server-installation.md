# MCP Server Installation Lab
## Hands-On Practice: Your First MCP Setup

### Welcome to Your First MCP Installation

This lab is designed to give you practical experience installing MCP servers. We'll start simple and gradually build up your skills. By the end, you'll have working MCP connections and the confidence to install more on your own.

### Lab Overview

**Time Required**: 90-120 minutes
**Difficulty Level**: Beginner to Intermediate
**Skills Learned**: MCP installation, authentication, basic testing, troubleshooting

---

## Pre-Lab Setup

### ✅ **Before You Begin**

**Check Your System**:
1. **Claude Desktop**: Version 1.2 or higher installed
2. **Internet**: Stable broadband connection
3. **Accounts**: Access to a Google account you can use for testing
4. **Files**: A few test documents on your computer
5. **Time**: Set aside 2 hours without interruptions

**Create a Lab Workspace**:
1. **Create a folder** on your Desktop called "MCP_Lab"
2. **Add some test files**:
   - A simple text document called "test_document.txt"
   - A small spreadsheet with sample data
   - A few other files you don't mind Claude accessing

**Safety First**:
- **Use a non-critical Google account** if possible
- **Don't connect** your primary business email initially
- **Have backups** of any important data

---

## Lab Exercise 1: File System MCP Installation
**Goal**: Set up your first MCP server for local file access
**Time**: 20-30 minutes
**Difficulty**: ⭐⭐ (Beginner)

### **Step 1: Access MCP Settings (5 minutes)**

1. **Open Claude Desktop**
2. **Find MCP settings** (look for):
   - Gear icon → "MCP Servers"
   - Menu → "Integrations"
   - Settings → "Tools & Extensions"
3. **Take a screenshot** of the MCP settings page for your lab report

### **Step 2: Install File System MCP (10 minutes)**

1. **Click "Add New MCP Server"**
2. **Select "File System Server"** from the list
3. **Choose installation path**:
   - Browse to your "MCP_Lab" folder
   - Grant access to this folder only
4. **Set permissions**: Start with "Read-Only"
5. **Click "Install"**
6. **Wait for installation** to complete

### **Step 3: Test Basic Functionality (15 minutes)**

1. **Return to Claude chat**
2. **Test Commands**:

```
Command 1: "What files are in my MCP_Lab folder?"
Expected Result: List of files you created
Record what happens: ________________

Command 2: "Read the content of test_document.txt"
Expected Result: Content of your text file
Record what happens: ________________

Command 3: "Create a new file called 'mcp_test.txt' with the content 'File System MCP is working!'"
Expected Result: Error (read-only mode)
Record what happens: ________________
```

### **Step 4: Upgrade to Read/Write (Optional)**

1. **Go back to MCP settings**
2. **Edit File System MCP configuration**
3. **Change permissions** to "Read/Write"
4. **Test the file creation command** again
5. **Verify** the new file was created in your MCP_Lab folder

### **🎯 Lab Exercise 1 Checkpoint**

Before moving on, ensure:
- ✅ Claude can list files in your lab folder
- ✅ Claude can read file contents
- ✅ You understand the difference between read-only and read/write permissions
- ✅ You can modify MCP settings

**If something isn't working**: Check the troubleshooting section at the end of this lab.

---

## Lab Exercise 2: Gmail MCP Installation
**Goal**: Connect Claude to your email account
**Time**: 30-45 minutes
**Difficulty**: ⭐⭐⭐ (Intermediate)

### **Step 1: Prepare Your Gmail Account (10 minutes)**

1. **Sign in to Gmail** (use test account if available)
2. **Send yourself 2-3 test emails** with different subjects:
   - "MCP Test Email 1"
   - "Important: Lab Exercise"
   - "Regular: Daily Update"
3. **Create a label** called "MCP_Testing"

### **Step 2: Install Gmail MCP (15 minutes)**

1. **In Claude Desktop MCP settings**
2. **Click "Add New MCP Server"**
3. **Select "Gmail Server"**
4. **Click "Install"**

### **Step 3: Google Authentication (10 minutes)**

1. **Browser will open automatically**
2. **Sign in** to your Google account
3. **Review permissions** carefully:
   - "Read emails"
   - "Compose and send emails"
   - "Manage labels and organization"
4. **Click "Allow"** if you're comfortable
5. **Wait for confirmation** in Claude Desktop

### **Step 4: Configure Email Settings (5 minutes)**

1. **Set default mode** to "Draft Only" (Claude creates drafts, doesn't send)
2. **Choose folder access**:
   - Start with "Inbox Only"
   - Add "MCP_Testing" label
3. **Save configuration**

### **Step 5: Test Email Integration (15 minutes)**

```
Test 1: "How many unread emails do I have?"
Expected: Number of unread emails
Actual result: ________________

Test 2: "What are the subjects of my last 3 emails?"
Expected: List of email subjects
Actual result: ________________

Test 3: "Draft a reply to the 'MCP Test Email 1' saying 'This is a test reply from Claude MCP'"
Expected: Draft created in Gmail
Check Gmail: Draft created? Yes/No ________________

Test 4: "Create an email draft to myself with subject 'MCP Lab Success' and body 'Gmail MCP is working correctly'"
Expected: New draft email
Check Gmail: Draft exists? Yes/No ________________
```

### **🎯 Lab Exercise 2 Checkpoint**

Before continuing:
- ✅ Claude can read your email count
- ✅ Claude can describe recent emails
- ✅ Claude can create email drafts (verify in Gmail)
- ✅ You understand the security implications

---

## Lab Exercise 3: Google Sheets MCP Installation
**Goal**: Enable Claude to work with spreadsheets
**Time**: 20-30 minutes
**Difficulty**: ⭐⭐⭐ (Intermediate)

### **Step 1: Create a Test Spreadsheet (10 minutes)**

1. **Go to Google Sheets**
2. **Create a new spreadsheet** called "MCP Lab Data"
3. **Add sample data**:

```
   A          B          C
1  Product    Sales      Month
2  Widget A   1500       Jan
3  Widget B   2300       Jan
4  Widget C   800        Jan
5  Widget A   1800       Feb
6  Widget B   2100       Feb
7  Widget C   950        Feb
```

4. **Save the spreadsheet**

### **Step 2: Install Google Sheets MCP (10 minutes)**

1. **MCP settings** → **"Add New MCP"**
2. **Select "Google Sheets Server"**
3. **Install and authenticate** (same process as Gmail)
4. **Set permissions**:
   - **Read access**: All spreadsheets
   - **Write access**: Only the "MCP Lab Data" spreadsheet

### **Step 3: Test Spreadsheet Integration (15 minutes)**

```
Test 1: "List my recent Google Sheets"
Expected: List including "MCP Lab Data"
Result: ________________

Test 2: "What data is in the 'MCP Lab Data' spreadsheet?"
Expected: Description of your sample data
Result: ________________

Test 3: "Calculate the total sales for Widget A"
Expected: 3300 (1500 + 1800)
Result: ________________

Test 4: "Add a new row with Widget D, 1200 sales, March"
Expected: New row added to spreadsheet
Check Google Sheets: Row added? Yes/No ________________

Test 5: "Create a summary showing total sales by product"
Expected: Analysis of sales data
Result: ________________
```

### **🎯 Lab Exercise 3 Checkpoint**

Verify that:
- ✅ Claude can find your spreadsheets
- ✅ Claude can read and understand data
- ✅ Claude can perform calculations
- ✅ Claude can add new data
- ✅ Claude can create analysis summaries

---

## Lab Exercise 4: Multi-MCP Integration Test
**Goal**: Use multiple MCPs together in a workflow
**Time**: 15-20 minutes
**Difficulty**: ⭐⭐⭐⭐ (Advanced)

### **Integration Workflow Test**

Now let's test using multiple MCPs in a single workflow:

```
Complex Task: "Create a sales report by reading data from my 'MCP Lab Data' spreadsheet, save it as a text file in my MCP_Lab folder, and draft an email to myself with the report as the email body."

Expected Steps:
1. Claude reads spreadsheet data
2. Claude analyzes and formats the data
3. Claude creates a text file with the report
4. Claude drafts an email with the report

Document what happens at each step:

Step 1 (Read spreadsheet): ________________

Step 2 (Analyze data): ________________

Step 3 (Create file): ________________

Step 4 (Draft email): ________________
```

### **Troubleshooting Multi-MCP Issues**

If the integration doesn't work smoothly:
1. **Test each MCP individually** first
2. **Check permissions** for all involved MCPs
3. **Try the workflow in smaller steps**
4. **Note any error messages**

---

## Lab Exercise 5: Configuration and Security Review
**Goal**: Understand and manage your MCP security
**Time**: 10-15 minutes

### **Security Audit Checklist**

Review your installed MCPs:

1. **File System MCP**:
   - **Folders it can access**: ________________
   - **Permission level**: ________________
   - **Security comfort level (1-10)**: ________________

2. **Gmail MCP**:
   - **Account connected**: ________________
   - **Permissions granted**: ________________
   - **Can send emails directly**: Yes/No ________________
   - **Security comfort level (1-10)**: ________________

3. **Google Sheets MCP**:
   - **Spreadsheets it can access**: ________________
   - **Can modify data**: Yes/No ________________
   - **Security comfort level (1-10)**: ________________

### **Permission Adjustment Exercise**

1. **Practice changing permissions**:
   - Make File System MCP read-only
   - Change Gmail MCP to "read-only" mode
   - Test that changes take effect

2. **Practice disconnecting MCPs**:
   - Temporarily disable one MCP
   - Verify it no longer works in Claude
   - Re-enable it

---

## Troubleshooting Common Issues

### **Problem: MCP Not Appearing in Claude**

**Symptoms**: Installed MCP doesn't show up in Claude's available tools

**Solutions to try**:
1. **Restart Claude Desktop** completely
2. **Check Claude Desktop version** (must be 1.2+)
3. **Verify installation** in MCP settings
4. **Check system resources** (close other applications)
5. **Reinstall the MCP server**

### **Problem: Authentication Failures**

**Symptoms**: "Access Denied" or "Permission Error" messages

**For Google Services**:
1. **Check Google account security settings**
2. **Try incognito browser** for authentication
3. **Clear browser cookies** for Google
4. **Verify account has necessary permissions**

### **Problem: Partial Functionality**

**Symptoms**: MCP connects but some features don't work

**Diagnostic steps**:
1. **Test with simple commands** first
2. **Check specific error messages**
3. **Verify permissions** match what you're trying to do
4. **Test with different data** to isolate the issue

---

## Lab Report Template

### **MCP Installation Lab Report**

**Student Name**: ________________
**Date**: ________________
**Total Time Spent**: ________________

#### **Exercise 1: File System MCP**
- **Installation successful**: Yes/No
- **Basic file reading worked**: Yes/No
- **File creation worked**: Yes/No
- **Main challenges**: ________________

#### **Exercise 2: Gmail MCP**
- **Authentication successful**: Yes/No
- **Email reading worked**: Yes/No
- **Email drafting worked**: Yes/No
- **Main challenges**: ________________

#### **Exercise 3: Google Sheets MCP**
- **Installation successful**: Yes/No
- **Data reading worked**: Yes/No
- **Data writing worked**: Yes/No
- **Main challenges**: ________________

#### **Exercise 4: Multi-MCP Integration**
- **Complex workflow successful**: Yes/No
- **Which part was most difficult**: ________________
- **What worked best**: ________________

#### **Exercise 5: Security Review**
- **Understanding of permissions**: Good/Fair/Poor
- **Comfort with security settings**: High/Medium/Low
- **Changes made to default settings**: ________________

#### **Overall Experience**
- **Most surprising discovery**: ________________
- **Biggest challenge**: ________________
- **Most excited about**: ________________
- **Questions remaining**: ________________

#### **Next Steps**
- **Which MCP will you use most**: ________________
- **What other MCPs interest you**: ________________
- **Specific workflow you want to automate**: ________________

---

## Bonus Challenges

### **Challenge 1: Custom Workflow Creation**
Design a workflow that uses all three MCPs for a task relevant to your work:
- Example: "Weekly report generation" or "Client communication automation"

### **Challenge 2: Permission Experimentation**
Try different permission combinations to understand security implications:
- Ultra-restrictive setup
- Balanced setup
- Maximum convenience setup

### **Challenge 3: Error Recovery**
Intentionally break your configuration and practice fixing it:
- Corrupt the configuration file
- Revoke permissions
- Practice restoration procedures

---

## Lab Completion Checklist

### **Before You Finish**

- ✅ **Successfully installed 3 MCP servers**
- ✅ **Tested basic functionality** of each MCP
- ✅ **Completed integration workflow** using multiple MCPs
- ✅ **Understand security implications** of each connection
- ✅ **Know how to modify or disconnect** MCPs
- ✅ **Can troubleshoot basic issues** independently
- ✅ **Completed lab report** with specific examples

### **Skills Gained**
After completing this lab, you should be able to:
- Install MCP servers using the GUI method
- Configure authentication for cloud services
- Set appropriate permission levels for different use cases
- Test MCP functionality systematically
- Troubleshoot common installation issues
- Understand the security implications of MCP connections
- Design workflows that use multiple MCPs together

---

## Next Steps After the Lab

### **Immediate Actions**
1. **Keep practicing** with your installed MCPs daily
2. **Start with simple tasks** that replace manual work
3. **Document successful workflows** for future reference

### **This Week**
1. **Install one additional MCP** that matches your work needs
2. **Create a real workflow** that saves you time
3. **Share your success** with a colleague

### **This Month**
1. **Explore advanced MCP features** and configurations
2. **Connect to business-specific tools** (if applicable)
3. **Develop confidence** with more complex integrations

**Ready for the next section?** Move on to [4.5 Claude Desktop Configuration](../sections/4-5-claude-desktop-config.md) to optimize your setup for maximum performance.