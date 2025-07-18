# Getting Started with Cursor

Cursor is an AI-powered code editor built on top of VS Code, designed to enhance your coding experience with intelligent assistance. This guide will help you get up and running quickly.

## Installation

1. **Download Cursor**: Visit [cursor.com](https://cursor.com) and download the appropriate version for your operating system.
2. **Install**: Follow the standard installation process for your platform
3. **Sign up**: Create an account to access AI features and sync your settings

## Key Features

### 1. AI Chat Assistant
- **Access**: Use `Cmd+L` (Mac) or `Ctrl+L` (Windows/Linux) to open the chat panel or click the Toggle AI Pane in top right corner. <br/><br/>
<div align="center">
    <img src="assets/ai_pane2.svg" height=""><br/>
    <em>Location of chat panel</em> <br/><br/>
</div>

- **Ask questions**: Get help with code explanations, debugging, and implementation suggestions
- **Context-aware**: The AI understands your current codebase and can provide relevant assistance
    - Enable Codebase Indexing in settings to give AI the full context of the project

### 2. Code Generation with Tab
- **Inline suggestions**: Start typing and press `Tab` to accept AI-generated code completions
- **Smart completions**: The AI suggests context-appropriate code based on your project
- **Multi-line generation**: Generate entire functions, classes, or code blocks


### 3. Agent Mode
- **Access**: Use `Cmd+L` (Mac) or `Ctr+L` (Windows/Linux) to open chat and switch to Agent mode in bottom left of chat window.
- **Create with natural language**: Prompt what to create or changes to make in natural language and Agent will execute changes.
- **File-wide changes**: Make complex modifcations across multiple files simultaneously using Agent mode.

### 4. Inline Edits
- **Access**: Use `Cmd+K` (Mac) or `Ctrl+K` (Windows/Linux) to open inline editor.
- **Modify with natural language**: Select chunk of code or edit with natrual language. Describe changes and AI will execute.


### 5. Codebase Understanding
- **@Symbols**: Method to referencing code, files, documentation using the `@` symbol
    - Can reference:
    - `@Files & folders` - Add specific files and folders to context
    - `@Code` -  Add certain lines of code to context
    - `@Docs` - Add documentation from outside sources into context
    - `@Git` - Add Git history, recent commits, etc. into context
    - `@Past Chats` - Add past Cursor chats into context
    - `@Cursor Rules` - Add rules into context
    - `@Web` - Add web searches into context
- **Context inclusion**: The AI can analyze your entire codebase for better suggestions
- **Documentation generation**: Ask the AI to create documentation for your code

## Getting Started Workflow

### 1. First Time Setup
#### Install cursor command
 - Open command palette `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux) and search for `Install 'cursor' command`
```bash
# Open your project in Cursor
cursor /path/to/your/project

# Or create a new project
mkdir my-new-project
cd my-new-project
cursor .
```

### 2. Basic Usage Examples

#### Ask for Help
- Open chat (`Cmd+L` for Mac or `Ctrl+L` for Windows/Linux) and ask questions like: "How does this function work?" while having a file(s) open
-  Understand new codebases by opening codebase and ask questions like: "Summarize the purpose of this codebase"
- Reference specific files: "Explain the logic in @example.py"
- Get debugging help: "Why is this code throwing an error?"

#### Generate Code
- Start typing a function signature and press `Tab` to auto-complete
- Use Inline editor (`Cmd+K` for Mac or `Ctrl+K` for Windows/Linux) to say: "Add error handling to this function"
- Ask Agent in chat: "Write a function to validate email addresses"

#### Refactor Code
- Select code and use Inline Editor: "Refactor this to use modern JavaScript syntax"
- Ask in chat: "How can I optimize this database query?"
- Get suggestions: "What's a better way to structure this component?"

## Best Practices

### 1. Effective Prompting
- **Be specific**: Instead of "fix this", say "fix the null pointer exception in the getUserData function"
- **Provide context**: Mention the programming language, framework, or specific requirements
- **Use examples**: Show the AI what you want with concrete examples

### 2. Leveraging Context
- **Reference files**: Use `@filename` to include specific files in your conversation
- **Context 
- **Mention symbols**: Reference functions, classes, or variables with `@symbolName`
- **Describe your goal**: Explain what you're trying to achieve, not just what's broken
<br/><br/>
<div align="center">
    <img src="assets/context.png" height="100"><br/>
    <em>Adding context to chat</em> <br/><br/>
</div>

### 3. Creating Rules
- **Review suggestions**: Always create a set of rules to define tech stack, unit testing, and coding patterns
- **Test thoroughly**: Run tests and verify functionality after AI assistance
- **Maintain style**: Ensure AI suggestions match your project's coding standards
<video width="640" height="360" controls>
  <source src="assets/rules.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
