# 🧭 My Git Mastery Challenge Journey

## 👩‍🎓 Student Information
- **Name:** Srija Ganja  
- **Student ID:** 23A91A0517  
- **Repository:** [https://github.com/ganjasrija/git-solved-23A91A0517.git](https://github.com/ganjasrija/git-solved-23A91A0517.git)  
- **Date Started:** October 27, 2025  
- **Date Completed:** October 29, 2025  

---

## 🧩 Task Summary
Cloned the instructor’s repository with pre-built conflicts and resolved all merge conflicts across multiple branches (`dev` and `conflict-simulator`) using proper Git workflows.  
Practiced advanced Git operations such as branching, stashing, cherry-picking, rebasing, resetting, and tagging to achieve a clean, stable, and well-documented repository.

---

## ⚙️ Commands Used

| Command | Times Used | Purpose |
|----------|-------------|----------|
| git clone | 1 | Clone instructor’s repository |
| git checkout | 25+ | Switch between branches |
| git branch | 10+ | View and manage branches |
| git merge | 2 | Merge dev and conflict-simulator into main |
| git add | 40+ | Stage resolved and modified files |
| git commit | 20+ | Commit resolved changes and new features |
| git push | 10+ | Push updates to my repository |
| git fetch | 1 | Fetch updates from instructor |
| git pull | 1 | Pull updates with merge strategy |
| git stash | 1 | Save temporary in-progress work |
| git cherry-pick | 2 | Copy specific commits between branches |
| git rebase | 1 | Synchronize feature branch with updated main |
| git reset | 3 | Demonstrate soft, mixed, and hard resets |
| git revert | 1 | Safely undo a bad commit |
| git tag | 2 | Create and push release tags |
| git status | 50+ | Check repository state frequently |
| git log | 30+ | View commit history |
| git diff | 20+ | Compare differences during conflict resolution |
| git reflog | 1 | Track branch history and recovery |

---

## ⚔️ Conflicts Resolved

### 🔹 Merge 1: main + dev (6 files)

**1. config/app-config.yaml**  
- Issue: Development used port 3000, production used 8080  
- Resolution: Unified environment-based configuration  
- Strategy: Kept production as default; added development override via `NODE_ENV`  
- Difficulty: Medium | Time: 15 min  

**2. config/database-config.json**  
- Issue: Different database hosts and SSL settings  
- Resolution: Created profiles for both environments  
- Strategy: Structured JSON to handle both modes cleanly  
- Difficulty: Medium | Time: 10 min  

**3. scripts/deploy.sh**  
- Issue: Conflicting deployment methods (Docker vs Production)  
- Resolution: Introduced `DEPLOY_ENV` variable for conditional logic  
- Strategy: Retained production flow, enabled optional Docker build  
- Difficulty: Hard | Time: 20 min  

**4. scripts/monitor.js**  
- Issue: Different monitoring logic and log formats  
- Resolution: Unified monitoring with config-driven intervals  
- Strategy: Used `process.env.NODE_ENV` to control behavior  
- Difficulty: Medium | Time: 15 min  

**5. docs/architecture.md**  
- Issue: Contradicting architecture documentation  
- Resolution: Merged descriptions into one overview  
- Strategy: Organized content by environment  
- Difficulty: Easy | Time: 10 min  

**6. README.md**  
- Issue: Different features and versioning  
- Resolution: Combined lists with environment labels  
- Strategy: Unified structure with sectioned docs  
- Difficulty: Easy | Time: 10 min  

---

### 🔹 Merge 2: main + conflict-simulator (5 files)

**1. README.md**  
- Issue: AI/ML section conflicted with existing content  
- Resolution: Added “Experimental Features” section  
- Strategy: Kept main stable docs intact  
- Difficulty: Medium | Time: 15 min  

**2. docs/architecture.md**  
- Issue: Standard vs AI-enhanced architecture  
- Resolution: Hybrid architecture combining both  
- Strategy: AI enhancements made optional  
- Difficulty: Medium | Time: 10 min  

**3. config/app-config.yaml**  
- Issue: Missing AI/ML flags  
- Resolution: Added `AI_MODE=false` default  
- Strategy: Maintained backward compatibility  
- Difficulty: Easy | Time: 10 min  

**4. scripts/deploy.sh**  
- Issue: AI init logic vs production deploy  
- Resolution: Enabled AI startup only when flag true  
- Strategy: Protected production deployments  
- Difficulty: Hard | Time: 20 min  

**5. scripts/monitor.js**  
- Issue: AI predictive monitoring vs standard logging  
- Resolution: Combined both, defaulted to standard logs  
- Strategy: Use AI logic in experimental mode  
- Difficulty: Medium | Time: 15 min  

---

## 🧠 Most Challenging Parts

1. **Understanding Conflict Markers:** Initially confusing (`<<<<<<<`, `=======`, `>>>>>>>`), later learned HEAD represents current branch.  
2. **deploy.sh Logic:** Merging production and AI logic safely was challenging.  
3. **Choosing What to Keep:** Required analyzing both branches carefully.  
4. **Rebasing Practice:** Learned how rebase rewrites history vs merge.

---

## 📚 Key Learnings

### 🔧 Technical Skills
- Mastered conflict resolution and branch management.  
- Practiced rebase, stash, cherry-pick, reset, and revert.  
- Used `git diff`, `git log`, and `git reflog` effectively.  

### 🪜 Best Practices
- Always review both sides before resolving.  
- Write meaningful commit messages.  
- Check `git status` often.  
- Tag stable points for traceability.  

### 🧩 Workflow Insights
- Conflicts are a normal part of collaboration — not errors.  
- A clean commit history shows professionalism.  
- Tags and documentation improve project traceability.  

---

## 💬 Reflection
This Git Mastery Challenge strengthened my understanding of real-world version control.  
I learned that merge conflicts are just Git asking for clarity — not problems.  
From resolving conflicts to using rebase, revert, and reset, each step built my confidence.  
Now, I can collaborate safely and effectively in any Git-based project.
