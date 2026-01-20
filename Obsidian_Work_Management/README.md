# 📓 Obsidian Work Management System

Welcome to your structured work note system. This setup is designed to handle tasks that span multiple weeks while keeping your daily and monthly records clean.

## 📂 Directory Structure

```
Obsidian_Work_Management/
├── 📅 Daily/                    # Optional daily logs
├── 📅 Weekly/                  # Main workspace - weekly reviews
├── 📅 Monthly/                 # Monthly summaries and goals
├── 🎯 Tasks/                   # Individual task notes (multi-week)
├── 🚀 Projects/                # Large project overviews
├── 📁 Archive/                 # Completed items
├── 📊 Master_Task_List.md      # Central task tracking
├── 📊 Dashboard.md             # System overview and guide
└── 📋 Templates/               # All templates
```

## 🛠️ Core Templates

- **`Weekly_Template.md`**: Weekly planning and review
- **`Monthly_Template.md`**: Monthly goals and summaries  
- **`Task_Template.md`**: Multi-week task management
- **`Project_Template.md`**: Large project coordination
- **`Daily_Template.md`**: Optional daily logging

## 🔄 Multi-Week Task Management

### The Linking Strategy
1. **Create Task Note**: Create detailed task in `Tasks/` folder
2. **Link in Weekly**: Reference task in weekly notes using `[[Task-Name]]`
3. **Update Progress**: Modify task note directly, weekly notes auto-update
4. **Track Completion**: Move completed tasks to Archive

### Example Flow
```markdown
# Weekly/2026-W01.md
## Active Tasks
- [ ] [[Develop-New-Feature]] - Status: Planning
- [ ] [[Setup-Infrastructure]] - Status: In Progress

# Tasks/Develop-New-Feature.md
## Progress
- Week 1: Research completed
- Week 2: Implementation started
```

## 🎯 Key Features

### ✅ Task-Centric Design
- Long-running tasks have dedicated notes with full history
- Progress updates happen once, visible everywhere through links
- Tasks can be referenced across multiple weeks/months

### ✅ Time-Centric Views
- Weekly notes focus on current week's priorities
- Monthly notes aggregate achievements and set high-level goals
- Clean separation between planning and detailed tracking

### ✅ Scalable Structure
- Clear directory organization
- Consistent naming conventions
- Easy to archive completed work

## � Getting Started

### Step 1: Setup
1. Set your Obsidian Template folder to `Obsidian_Work_Management/Templates`
2. Install recommended plugins: **Periodic Notes**, **Calendar**, **Dataview**

### Step 2: Create Your First Weekly Note
1. Use `Weekly_Template.md` to create `Weekly/2026-W04.md`
2. Add 3 main goals for the week
3. Link any existing multi-week tasks

### Step 3: Start a Multi-Week Task
1. Create task note in `Tasks/` using `Task_Template.md`
2. Link it in your weekly note under "Active Tasks"
3. Update progress directly in the task note

### Step 4: Monthly Review
1. At month end, create monthly note using `Monthly_Template.md`
2. Review all weekly notes from the month
3. Update `Master_Task_List.md` with completed items

## 📈 Advanced Usage

### Using Dataview Queries
```dataview
TABLE status, priority, created
FROM "Tasks"
WHERE status != "completed"
SORT priority DESC
```

### Tag Strategy
- Use tags like `#project-a`, `#high-priority`, `#q1-2026`
- Combine with status: `#in-progress`, `#blocked`, `#review`

### Linking Best Practices
- Use descriptive task names: `[[Website-Performance-Optimization]]`
- Create project hubs in `Projects/` for complex initiatives
- Cross-reference related tasks and projects

## � Example Files

Check these example files to see the system in action:
- `Weekly/2026-W04.md` - Sample weekly review
- `Tasks/Setup-Obsidian-Work-System.md` - Completed task example
- `Examples.md` - Detailed usage scenarios

---

**Ready to transform your work note management? Start with your first weekly note today!**
