# SEO Hackathon 2026

## How to Participate

1. Create a comment here to "register" https://github.com/chr156r33n/seo-hackathon-2026/discussions/2
2. Think about some of the potential tools/techniques/scripts/software that'd be beneficial to SEO - DON'T START BUILDING YET if you want to submit it to the Hackathon, just to keep it in the spirit of things
3. Get yourself used to running with GitHub and AI assisted (Vibe) coding (if you're not already) - notes below
4. Stay tuned for the dates/start times and further details

## How to Submit Code

1. Fork this repository
2. Create a project folder in `/projects/your-team-name/`
3. Work on your project in your fork
4. Submit a Pull Request to merge your changes
5. Wait for approval from a designated reviewer

---

## Working with GitHub: A Guide for Non-Developers

### What is GitHub?

GitHub is a platform for storing and sharing code. Think of it like Google Drive, but specifically designed for code projects. It uses **Git**, a version control system that tracks changes to files over time.

### Key Concepts

- **Repository (Repo)**: A project folder containing all your files and their history
- **Fork**: Creating your own copy of someone else's repository
- **Branch**: A parallel version of the code where you can make changes safely
- **Commit**: Saving a snapshot of your changes with a message describing what you did
- **Pull Request (PR)**: A request to merge your changes into the main project

### Step-by-Step GitHub Workflow

#### 1. Create a GitHub Account
- Go to [github.com](https://github.com) and sign up
- Choose a username (this will be part of your profile URL)
- Verify your email address

#### 2. Fork the Repository
- Navigate to this repository's page on GitHub
- Click the **"Fork"** button in the top-right corner
- This creates a copy of the repository under your GitHub account
- You now have your own version to work with!

#### 3. Clone Your Fork (Get It on Your Computer)
- On your fork's page, click the green **"Code"** button
- Copy the HTTPS URL (looks like: `https://github.com/your-username/repo-name.git`)
- Open your terminal/command prompt
- Navigate to where you want the project: `cd ~/Desktop` (or wherever you prefer)
- Run: `git clone https://github.com/your-username/repo-name.git`
- This downloads the repository to your computer

#### 4. Create Your Project Folder
- Navigate into the cloned folder: `cd repo-name`
- Go to the projects folder: `cd projects`
- Create your team folder: `mkdir your-team-name`
- Navigate into it: `cd your-team-name`
- You're now ready to add your project files!

#### 5. Make Changes and Commit
- Add your project files to the `your-team-name` folder
- In the terminal, from the repository root, run:
  ```bash
  git add projects/your-team-name/
  git commit -m "Add project files for [your-team-name]"
  ```
- The commit message should describe what you're adding

#### 6. Push Your Changes
- Send your changes to GitHub: `git push origin main`
- If this is your first push, you might need to set upstream:
  ```bash
  git push -u origin main
  ```

#### 7. Create a Pull Request
- Go to your fork on GitHub
- You'll see a banner saying "This branch is X commits ahead" with a **"Contribute"** button
- Click **"Contribute"** → **"Open pull request"**
- Add a title and description explaining your project
- Click **"Create pull request"**
- Wait for a reviewer to approve and merge your changes

### Common Git Commands

```bash
# Check status of your files
git status

# See what changed
git diff

# Add all changes
git add .

# Commit with a message
git commit -m "Your message here"

# Push to GitHub
git push origin main

# Pull latest changes from the original repo
git pull upstream main
```

### Troubleshooting

**"Permission denied" errors?**
- Make sure you're using HTTPS (not SSH) URLs
- You may need to authenticate with a Personal Access Token

**"Repository not found"?**
- Double-check the repository URL
- Make sure you've forked the repository first

**Need to update your fork?**
- Add the original repo as "upstream": `git remote add upstream [original-repo-url]`
- Fetch updates: `git fetch upstream`
- Merge: `git merge upstream/main`
- Push: `git push origin main`

---

## Working with GitHub Using AI Coding Tools

### Using Cursor

[Cursor](https://cursor.sh) is an AI-powered code editor that integrates Git operations directly into your workflow.

#### Setup
1. Download and install Cursor from [cursor.sh](https://cursor.sh)
2. Open Cursor and sign in with your GitHub account
3. Open the repository folder: **File → Open Folder** → select your cloned repository

#### Forking and Cloning
1. In Cursor, open the Command Palette: `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
2. Type "Git: Clone" and select it
3. Paste your fork's URL: `https://github.com/your-username/repo-name.git`
4. Choose where to save it
5. Cursor will open the cloned repository automatically

#### Making Changes
1. Use Cursor's AI chat (`Cmd+L` or `Ctrl+L`) to help write code
2. Ask Cursor to create files, write functions, or fix bugs
3. Cursor can help you create your project structure:
   - "Create a folder structure for a web project in `projects/my-team/`"
   - "Add an index.html file with a basic structure"

#### Committing and Pushing
1. Open the Source Control panel (Git icon in the left sidebar, or `Ctrl+Shift+G`)
2. You'll see all your changed files
3. Stage files by clicking the `+` next to them, or stage all with `+` next to "Changes"
4. Write a commit message in the text box at the top
5. Click the checkmark (✓) to commit
6. Click the `...` menu → **Push** to send to GitHub

#### Creating a Pull Request
1. After pushing, Cursor will show a notification with a link to create a PR
2. Or use the Command Palette: "Git: Create Pull Request"
3. Or manually go to GitHub and create the PR as described in the main workflow

#### Tips for Cursor
- Use `Cmd+K` (Mac) or `Ctrl+K` (Windows/Linux) for inline AI edits
- The AI chat understands context about your entire project
- Ask Cursor to explain Git commands if you're unsure

---

### Using Claude Code (Claude Desktop / Anthropic)

Claude Code refers to using Claude AI to help with coding tasks. You can use Claude through various interfaces.

#### Setup
1. Access Claude through:
   - [Claude.ai](https://claude.ai) web interface
   - Claude Desktop app (download from Anthropic)
   - VS Code extension (if available)
2. For file operations, you'll still need a code editor or terminal

#### Workflow with Claude
1. **Planning Phase**: Ask Claude to help plan your project structure
   - "Help me design a folder structure for an SEO project"
   - "What files should I include in my hackathon project?"

2. **Code Generation**: Ask Claude to write code
   - Paste your requirements: "Create an HTML page that does X, Y, Z"
   - Claude will generate code you can copy into your files

3. **File Management**: 
   - Use your terminal or code editor to create files
   - Copy Claude's generated code into the appropriate files
   - Save files in your `projects/your-team-name/` folder

4. **Git Operations**: Use terminal commands (see main GitHub guide) or your code editor's Git integration

#### Example Claude Prompts
```
"I'm participating in an SEO hackathon. Help me create a project structure 
with an HTML file, CSS file, and a README. The project should be about 
[your topic]."

"Generate a responsive HTML page with semantic markup for SEO best practices."

"Help me write a commit message for adding my project files to the repository."
```

#### Tips for Claude
- Be specific about file locations and structure
- Ask Claude to explain any code it generates
- Use Claude to review your code before committing
- Ask for help writing good commit messages

---

### Using ChatGPT Codex / ChatGPT

ChatGPT (including Code Interpreter/Advanced Data Analysis) can help with coding tasks and understanding Git workflows.

#### Setup
1. Access ChatGPT at [chat.openai.com](https://chat.openai.com)
2. For file operations, use a code editor alongside ChatGPT
3. Consider using ChatGPT Plus for Code Interpreter features

#### Workflow with ChatGPT
1. **Understanding Git**: Ask ChatGPT to explain Git concepts
   - "Explain what forking means in GitHub"
   - "How do I create a pull request step by step?"

2. **Code Generation**: 
   - Describe what you want to build
   - ChatGPT will provide code you can copy
   - Example: "Create a landing page HTML file optimized for SEO"

3. **File Creation**:
   - Copy ChatGPT's code into files in your project folder
   - Use your code editor (VS Code, Cursor, etc.) to save files

4. **Git Commands**: Ask ChatGPT for the exact commands you need
   - "What git commands do I run to commit and push my changes?"
   - ChatGPT will give you step-by-step instructions

#### Example ChatGPT Prompts
```
"I've forked a GitHub repository. Walk me through cloning it, adding my 
project files, and creating a pull request."

"Generate HTML, CSS, and JavaScript for an SEO-optimized landing page 
about [your topic]."

"Help me write a professional README.md file for my hackathon project."
```

#### Tips for ChatGPT
- Ask for explanations if you don't understand something
- Request code in specific formats (HTML, CSS, etc.)
- Use ChatGPT to debug error messages you encounter
- Ask for best practices for your specific use case

---

## Quick Reference: Which Tool Should I Use?

- **Complete beginners**: Start with the manual GitHub workflow, use ChatGPT for explanations
- **Want AI in your editor**: Use Cursor for integrated coding and Git operations
- **Prefer web-based AI**: Use Claude or ChatGPT for code generation, then use a code editor for file management
- **Need step-by-step guidance**: Ask any AI tool to explain Git commands before running them

## Getting Help

If you run into issues:
1. Check the troubleshooting section above
2. Ask your AI coding assistant to explain the error
3. Search GitHub's documentation: [docs.github.com](https://docs.github.com)
4. Reach out to hackathon organizers or mentors
