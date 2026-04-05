# Module 1 — From Idea to Shipped Product

**Course:** [Claude Code in Practice](https://maven.com/boring-bot/claude-code-in-practice)
**Instructor:** Hamza Farooq · Traversaal.ai

---

## Getting Started

### Step 1 — Clone this repo

Open your terminal and run:

```bash
git clone https://github.com/hamzafarooq/claude-code-starter.git
cd claude-code-starter/module-1
```

### Step 2 — Install Claude Code

```bash
npm install -g @anthropic/claude-code
```

No Node.js? Download the LTS version from [nodejs.org](https://nodejs.org), then re-run the command above.

Verify it worked:
```bash
claude --version
```

### Step 3 — Set up your API key

1. Go to [console.anthropic.com](https://console.anthropic.com) → **API Keys** → **Create Key**
2. Copy the key (starts with `sk-ant-...`)
3. Set it in your terminal:

```bash
export ANTHROPIC_API_KEY=sk-ant-your-key-here
```

To make it permanent:
```bash
echo 'export ANTHROPIC_API_KEY=sk-ant-your-key-here' >> ~/.zshrc
source ~/.zshrc
```

### Step 4 — Start Claude Code

From inside the `module-1` folder:
```bash
claude
```

You're ready. Now work through the three assignments below.

---

## Assignment 1 — Set Up Your CLAUDE.md

`CLAUDE.md` is the most important file in your workspace. Claude reads it automatically at the start of every session. It tells Claude who you are, what your project is, and how to work with you — so you don't have to repeat yourself every time.

**Think of it as a standing briefing memo you write once.**

### What a good CLAUDE.md covers

1. **Who you are** — your role, what you care about, what you don't need explained
2. **What your project is** — one sentence, current phase, key stakeholders
3. **How Claude should respond** — tone, length, format preferences
4. **Your conventions** — where files live, how you write user stories, what sections every PRD needs

### Your task

Open Claude Code in this folder and run:

```
I'm a product manager. Help me create a CLAUDE.md file for my project. Ask me the questions you need to write a good one.
```

Claude will ask you a few questions and generate the file for you. Answer honestly — this file will shape every session going forward.

A starter template is included in this folder: [CLAUDE.md](CLAUDE.md). You can edit it directly instead if you prefer.

### How to verify it's working

After saving your `CLAUDE.md`, start a new session and ask:

```
What do you know about this project based on what you've read?
```

Claude should accurately describe your project and role. If it doesn't, open `CLAUDE.md` and fill in the placeholder sections.

---

## Assignment 2 — Install Your Skills

Skills are reusable behaviors stored in `.claude/skills/`. You trigger them with a `/skill-name` command. Instead of typing the same long prompt every time, you type one word.

Two skills are already included in this folder:
- `/prd-generator` — generates a full structured PRD from a brief description
- `/user-story-writer` — converts rough feature ideas into user stories with acceptance criteria

### Your task

**1. Test the PRD generator:**
```
/prd-generator
```
Follow the prompts. Give Claude a real feature idea — something your team is actually working on or considering.

**2. Test the user story writer:**
```
/user-story-writer
```
Describe the same feature informally. See how Claude structures it into stories.

**3. Review the skill files:**

Open [.claude/skills/prd-generator/SKILL.md](.claude/skills/prd-generator/SKILL.md) and read it. This is exactly what Claude follows when you run `/prd-generator`. You can edit it to match your team's PRD format.

### How skills are structured

```
module-1/
├── CLAUDE.md
└── .claude/
    └── skills/
        ├── prd-generator/
        │   └── SKILL.md
        └── user-story-writer/
            └── SKILL.md
```

> **Mac tip:** Folders starting with `.` are hidden by default. Press `Cmd + Shift + .` in Finder to show them.

---

## Assignment 3 — From Idea to PRD to MVP

Now put it all together. You'll take a real product idea through the full workflow: from rough concept to a structured PRD to a working prototype.

### Part A — Pick your idea

Choose a product or feature idea. It can be:
- Something your team is currently planning
- A problem you've noticed in your own work
- Anything you'd actually want to exist

Keep it small enough to ship in a week. Examples from class:
- A tool that rewrites AI-generated text to sound more human
- An SEO content generator for blog posts
- A meeting notes → Jira ticket converter

### Part B — Generate your PRD

Run `/prd-generator` and fill in the details for your idea. When Claude finishes, ask:

```
Save this PRD to docs/prd.md
```

Then review it and ask:
```
What are the three riskiest assumptions in this PRD?
```

### Part C — Break it into stories

Run `/user-story-writer` and describe the must-have features from your PRD. Ask Claude to prioritize them:

```
Which of these stories should be in the first sprint?
```

### Part D — Build the MVP

Tell Claude what you want to build:

```
Based on this PRD, help me build the simplest possible version of this product. Ask me what tools and constraints I'm working with.
```

Claude will ask clarifying questions and then start building with you. You don't need to write any code.

### What to submit

Share a link to your:
1. `docs/prd.md` — your completed PRD
2. The working MVP (a URL, a file, or a screenshot)

Post it in the course Slack channel.

---

## Reference — Useful Prompts for PMs

| What you want | What to type |
|---|---|
| Generate a full PRD | `/prd-generator` |
| Write user stories | `/user-story-writer` |
| Find gaps in a spec | `"Review docs/prd.md and tell me what's missing"` |
| Prep for engineering | `"What questions will engineers ask about this PRD?"` |
| Create a sprint plan | `"Turn the must-have stories into a 2-week sprint plan"` |
| Write for execs | `"Rewrite this as 3 bullets for a VP with 10 seconds"` |
| Check for edge cases | `"What edge cases am I missing in this flow?"` |

---

## Troubleshooting

**"command not found: claude"**
Run `npm install -g @anthropic/claude-code` again. Check Node.js is installed: `node --version`.

**Claude isn't reading my CLAUDE.md**
The file must be named exactly `CLAUDE.md` (all caps) in the same folder where you ran `claude`.

**Skill not triggering**
Check that the path is `.claude/skills/<name>/SKILL.md` and the frontmatter `name:` matches what you typed after `/`.

**Claude responses are too long**
Add to your CLAUDE.md: `"Keep all responses under 200 words unless I ask for more."`

---

*[Claude Code in Practice](https://maven.com/boring-bot/claude-code-in-practice) · Taught by Hamza Farooq · Traversaal.ai*
