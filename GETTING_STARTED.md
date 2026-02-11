# Getting Started with GitHub (For This Project)

This guide is minimal and embodied—you'll learn by doing, not by studying.

## Core Metaphor

Think of Git as **temporal navigation**:
- **Repository** - a coherent container for your project
- **Commit** - a snapshot of a moment in development (like cellular division)
- **Branch** - parallel timeline for experiments
- **Remote** - the shared space (GitHub) where others can see/fork your work

## What You Need

1. A GitHub account (github.com - sign up is simple)
2. Git installed on your computer (likely already there on Mac)

Check if you have git:
```bash
git --version
```

If not installed, download from: git-scm.com

## First Session (Tonight - 10 minutes)

### 1. Initialize the repository
```bash
cd path/to/cellular-calendar
git init
git add .
git commit -m "Initial commit: cellular calendar with membranes and connections"
```

This creates your first snapshot.

### 2. Create GitHub repository
- Go to github.com
- Click the + icon → "New repository"
- Name it: `cellular-calendar`
- Make it public
- **Don't** add README, license, or .gitignore (we already have them)
- Click "Create repository"

### 3. Connect local to GitHub
GitHub will show you commands. They look like:
```bash
git remote add origin https://github.com/YOUR_USERNAME/cellular-calendar.git
git branch -M main
git push -u origin main
```

Copy and paste these into your terminal.

**Done.** Your work is now on GitHub.

## Tomorrow's Session

We can:
- Add 3D navigation feature
- Make a commit that shows the evolution
- Write commit messages that tell the story

## Essential Commands (Reference)

You'll use these 90% of the time:

```bash
git status              # See what's changed
git add .               # Stage all changes
git commit -m "message" # Create snapshot with description
git push                # Send to GitHub
```

## Philosophy

- **Commit when something feels complete** - not on a schedule
- **Commit messages are mini-stories** - "Add semantic clustering to cells" not "update file"
- **Push when you want to share** - local commits are private until pushed
- **Branches are for experiments** - main branch is your "canonical timeline"

## If You Get Stuck

Most "mistakes" in Git are reversible. The system is designed for safety.

Common confusion: 
- `git add` stages changes (prepares them)
- `git commit` records them (takes the snapshot)
- `git push` shares them (sends to GitHub)

Think: prepare → record → share

---

*This is enough to start. The rest reveals itself through use.*
