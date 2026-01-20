# 📊 Work Management Dashboard

Welcome to your personal work management system! This dashboard helps you navigate and understand how to effectively use your Obsidian work notes.

## 🚀 Quick Start Guide

### For New Users
1. **Start with Weekly Notes**: Every Monday, create a new note in `Weekly/` using the `Weekly_Template`
2. **Track Multi-Week Tasks**: When a task spans multiple weeks, create a dedicated task note in `Tasks/`
3. **Link Everything**: Use `[[Task Name]]` syntax to link tasks to your weekly notes

### For Existing Users
- Review your `Master_Task_List.md` weekly
- Archive completed tasks monthly
- Use project notes for complex initiatives

## 📂 Directory Structure Explained

```
Obsidian_Work_Management/
├── 📅 Daily/           # Optional daily logs (if needed)
├── 📅 Weekly/          # Your main workspace - create one every week
├── 📅 Monthly/         # Monthly reviews and goal setting
├── 🎯 Tasks/           # Individual task notes (for multi-week tasks)
├── 🚀 Projects/        # Large project overviews
├── 📁 Archive/         # Completed items
├── 📊 Master_Task_List.md    # Central task tracking
└── 📋 Templates/       # All templates
```

## 🔗 How Tasks Flow Through the System

### 1. Task Creation
```markdown
# In Tasks/ folder
[[New Task Name]] - Created in Tasks/ with Task_Template
```

### 2. Weekly Integration
```markdown
# In Weekly notes
## Active Tasks
- [ ] [[New Task Name]] - Status: In Progress
```

### 3. Monthly Review
```markdown
# In Monthly notes
## Task Completion Summary
- Completed: [[New Task Name]]
- In Progress: [[Another Task]]
```

## 💡 Best Practices

### For Multi-Week Tasks
1. **Create detailed task notes** with clear objectives and timelines
2. **Update progress weekly** in the task note, not in weekly notes
3. **Use consistent naming** for easy linking (e.g., `[[Project-A-Development]]`)

### For Weekly Planning
1. **Review previous week** before planning the next
2. **Limit to 3-5 main goals** per week
3. **Link to relevant tasks** instead of copying content

### For Monthly Reviews
1. **Aggregate weekly achievements**
2. **Identify patterns** in productivity
3. **Set realistic goals** for the coming month

## 🛠️ Advanced Features

### Using Dataview (if installed)
```dataview
TABLE status, priority, created
FROM "Tasks"
WHERE status != "completed"
SORT priority DESC
```

### Template Variables
- `{{date}}` - Current date
- `{{date:YYYY-[W]ww}}` - Week number
- `{{date:YYYY-MM}}` - Month

## 📈 Productivity Tips

1. **Weekly Review Ritual**: Every Friday, spend 15 minutes reviewing and planning
2. **Task Batching**: Group similar tasks in your weekly notes
3. **Progress Tracking**: Use checkboxes consistently
4. **Reflection**: Always include learnings in weekly reviews

---

*Last updated: {{date}}*