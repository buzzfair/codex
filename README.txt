SUBAGENT TEMPLATES FOR WEBSITE PROJECTS
========================================

These Claude Code subagent definitions can help you overhaul a professional
website. Each agent is specialized for a specific domain, keeping context
focused and outputs more useful.


HOW TO USE
==========

STEP 1: FIND OR CREATE THE .claude DIRECTORY
---------------------------------------------

The .claude directory must be in your PROJECT ROOT (the main folder of your
project, where your code lives).

IMPORTANT: The folder name starts with a dot (.claude), which makes it a
hidden folder. You'll need to show hidden files to see it.


On Mac:

1. Open Finder and navigate to your project folder

2. Press Cmd + Shift + . (Command + Shift + Period) to show hidden files

3. Look for a .claude folder. If it doesn't exist, create it:
   - Right-click in the folder and select "New Folder"
   - Name it .claude (include the dot at the beginning)
   - Press Enter (you may see a warning about the dot—click "OK")


On Windows:

1. Open File Explorer and navigate to your project folder

2. Click "View" in the menu bar, then check "Hidden items"

3. Look for a .claude folder. If it doesn't exist, create it:
   - Right-click in the folder and select "New" > "Folder"
   - Name it .claude (include the dot at the beginning)
   - Press Enter


STEP 2: COPY THE AGENTS FOLDER
------------------------------

Copy the entire "agents" folder from this download into your .claude directory.

Your project structure should look like this:

    your-project/                    <-- This is your project root
    |
    +-- .claude/                     <-- Hidden folder (create if needed)
    |   |
    |   +-- agents/                  <-- Copy this folder here
    |       |
    |       +-- creative-director.md
    |       +-- website-copywriter.md
    |       +-- brand-editor.md
    |       +-- ui-designer.md
    |       +-- seo-expert.md
    |       +-- accessibility-consultant.md
    |       +-- thought-leadership-copywriter.md
    |
    +-- src/                         <-- Your other project files
    +-- index.html
    +-- ...


STEP 3: CUSTOMIZE THE AGENTS
----------------------------

Open each .md file in the agents folder and fill in the [FILL IN] sections
with your specific context (brand colors, voice guidelines, etc.).

You can open .md files with any text editor (Notepad, TextEdit, VS Code, etc.)


STEP 4: USE WITH CLAUDE CODE
----------------------------

Claude Code will automatically detect and use these agents when you run it
in your project directory.


THE AGENTS
==========

CREATIVE DIRECTOR
  When to use: Visual aesthetics, design coherence, brand alignment
  Model: opus

WEBSITE COPYWRITER
  When to use: Landing pages, CTAs, product descriptions
  Model: sonnet

BRAND EDITOR
  When to use: Voice consistency, style alignment, light edits
  Model: sonnet

UI DESIGNER
  When to use: Component styling, CSS implementation, visual consistency
  Model: sonnet

SEO EXPERT
  When to use: Metadata, headings, schema markup, search optimization
  Model: sonnet

ACCESSIBILITY CONSULTANT
  When to use: WCAG compliance, keyboard nav, screen readers
  Model: sonnet

THOUGHT LEADERSHIP COPYWRITER
  When to use: Long-form articles, research, outlines
  Model: opus


TIPS FOR CUSTOMIZATION
======================

1. BE SPECIFIC ABOUT YOUR CONTEXT
   The more specific your brand voice, colors, and design principles, the
   better the results.

2. INCLUDE REFERENCE MATERIALS
   Link to your best existing work so agents can pattern-match.

3. UPDATE AS YOU GO
   If an agent keeps making the same mistake, add a specific instruction
   to prevent it.

4. CHOOSE THE RIGHT MODEL
   Use "opus" for complex creative work, "sonnet" for straightforward tasks.


QUESTIONS?
==========

Find me at karen@goodcontent.cc

Or subscribe to Wondering About AI for more on AI tools and workflows:
https://wonderingaboutai.substack.com
