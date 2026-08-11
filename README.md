
### **How does Cowork work?**
1. Describe your task
2. Claude plans and breakdown
3. Executes in Sanbox VM
4. Delivers output

### Key Behaviors:
- **Direct local file access:** reads and writes to your folders
- **Sub-agent coordination:** breaks complex work into parallel tasks
- **Professional outputs:** Excel, PowerPoint, Word, PDFs and more
- **Scheduled tasks:** automate recurring work without manual prompts

### Cowork capabilities
- **Document Creation:** Word docs, Spreadsheets, presentations, PDFs with professional formatting 
- **Data Analysis:** Statistical analysis, visualization, data cleaning and transformation
- **R****easearch and synthesis:** Web reasearch, transcript analysis, multi-source information gathering
- **File management: **Organize folders, batch rename, process receipts, sort files
- **Code and automation:** Write scripts, build tools, automate repetitive workflows
- **Scheduled Tasks:** Create recurring automated tasks that run on a set schedule

**Note:** Cowork uses more tokens than standard chat, think of it as Claude doing deep work, not quick answers

### Claude Cowork Practical Demo: Organizing files and using excel skills
This practical demo makes files organized in different categories and calculates the total receipts in excel using Claude Cowork.
There are 2 invoices, 2 receipts and 2 agreements in Small Business folder:

![Original folder structure](https://github.com/pratikishere/claude-cowork-learning/blob/main/organising-files-screenshots/original-folder-structure.png)

The prompt (used with Opus 4.8) :
"Organise the folder into categories: receipts, invoices and agreements. Then I want you to add the total receipts and exports them in an Excel Sheet."  
Output:  

![Output folder structure](https://github.com/pratikishere/claude-cowork-learning/blob/main/organising-files-screenshots/output-folder-structure.png)

![Ouput of receipts excel](https://github.com/pratikishere/claude-cowork-learning/blob/main/organising-files-screenshots/receipts-summary.png)

As receipts have different currency the total is not correct. Claude has already mentioned in the result. We can use the following prompt to get receipts in CAD:
"Convert USD rows to CAD. Take the currency conversation value of the date mentioned."  
Output:

![Receipts excel](https://github.com/pratikishere/claude-cowork-learning/blob/main/organising-files-screenshots/receipts-summary-final.png)
