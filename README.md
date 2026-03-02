# Subagent Templates for Website Projects

These Claude Code subagent definitions can help you overhaul a professional website. Each agent is specialized for a specific domain, keeping context focused and outputs more useful.

## How to Use

### Step 1: Find or create the .claude directory

The `.claude` directory must be in your **project root** (the main folder of your project, where your code lives).

**The folder name starts with a dot (`.claude`), which makes it a hidden folder.** You'll need to show hidden files to see it.

#### On Mac:

1. Open Finder and navigate to your project folder
2. Press `Cmd + Shift + .` (Command + Shift + Period) to show hidden files
3. Look for a `.claude` folder. If it doesn't exist, create it:
   - Right-click in the folder and select "New Folder"
   - Name it `.claude` (include the dot at the beginning)
   - Press Enter (you may see a warning about the dot—click "OK")

#### On Windows:

1. Open File Explorer and navigate to your project folder
2. Click "View" in the menu bar, then check "Hidden items"
3. Look for a `.claude` folder. If it doesn't exist, create it:
   - Right-click in the folder and select "New" > "Folder"
   - Name it `.claude` (include the dot at the beginning)
   - Press Enter

### Step 2: Copy the agents folder

Copy the entire `agents` folder from this download into your `.claude` directory.

Your project structure should look like this:

```
your-project/                    <-- This is your project root
├── .claude/                     <-- Hidden folder (create if needed)
│   └── agents/                  <-- Copy this folder here
│       ├── creative-director.md
│       ├── website-copywriter.md
│       ├── brand-editor.md
│       ├── ui-designer.md
│       ├── seo-expert.md
│       ├── accessibility-consultant.md
│       └── thought-leadership-copywriter.md
├── src/                         <-- Your other project files
├── index.html
└── ...
```

### Step 3: Customize the agents

Open each `.md` file in the `agents` folder and fill in the `[FILL IN]` sections with your specific context (brand colors, voice guidelines, etc.).

### Step 4: Use with Claude Code

Claude Code will automatically detect and use these agents when you run it in your project directory.

## The Agents

| Agent | When to Use | Model |
|-------|-------------|-------|
| **Creative Director** | Visual aesthetics, design coherence, brand alignment | opus |
| **Website Copywriter** | Landing pages, CTAs, product descriptions | sonnet |
| **Brand Editor** | Voice consistency, style alignment, light edits | sonnet |
| **UI Designer** | Component styling, CSS implementation, visual consistency | sonnet |
| **SEO Expert** | Metadata, headings, schema markup, search optimization | sonnet |
| **Accessibility Consultant** | WCAG compliance, keyboard nav, screen readers | sonnet |
| **Thought Leadership Copywriter** | Long-form articles, research, outlines | opus |

## Tips for Customization

1. **Be specific about your context.** The more specific your brand voice, colors, and design principles, the better the results.

2. **Include reference materials.** Link to your best existing work so agents can pattern-match.

3. **Update as you go.** If an agent keeps making the same mistake, add a specific instruction to prevent it.

4. **Choose the right model.** `opus` for complex creative work, `sonnet` for straightforward tasks.

## Questions?

Find me at karen@goodcontent.cc or subscribe to [Wondering About AI](https://wonderingaboutai.substack.com) for more on AI tools and workflows.
