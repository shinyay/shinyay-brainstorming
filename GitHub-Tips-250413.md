# GitHub Copilot Tips & Subscription Plans

---

## 1. Preparation & Context Setting

### a. Open Related Files
- **Tip:** Keep related files open in your editor for richer context.
- **Detail:** GitHub Copilot uses the contents of open files to generate more precise suggestions. You can even attach files using the context variable `#file:`.

### b. Use Appropriate Comments
- **Tip:** Add comprehensive comments at the top of files and before functions.
- **Detail:** Describing the overall process—including inputs, outputs, and purpose—improves the clarity and relevance of suggestions.

### c. Employ Meaningful Naming
- **Tip:** Use descriptive names for functions, variables, and parameters.
- **Detail:** Meaningful naming improves readability and guides Copilot to suggest code that aligns with your intended functionality.

### d. Specify Library Versions When Needed
- **Tip:** State specific versions for key libraries (e.g., Python or Node modules).
- **Detail:** This minimizes compatibility issues and ensures that the generated code aligns with the version-specific syntax or features.

### e. Reset Context for Changed Tasks
- **Tip:** Start a new chat session using the `/clear` command when switching contexts.
- **Detail:** Copilot Chat uses the ongoing conversation context—refreshing it prevents outdated context from influencing suggestions.

---

## 2. Practical Shortcuts & Command Usage

### a. Code Completion Acceptance & Rejection
- **Shortcut:**
  - **Accept:** Press `Tab`.
  - **Reject:** Press `Esc`.
- **Detail:** Quickly incorporate or dismiss Copilot’s code suggestions with these keystrokes.

### b. Navigating Through Suggestions
- **Shortcut:**
  - **Next Suggestion:** `Alt + ]` (or `option + ]` on Mac)
  - **Previous Suggestion:** `Alt + [` (or `option + [` on Mac)
- **Detail:** Easily cycle through multiple suggestions to pick the best match.

### c. Accepting Code by Word
- **Shortcut:** Press `Ctrl + →` (or `⌘ + →` on Mac).
- **Detail:** This allows you to accept suggestions incrementally rather than the entire line.

### d. Multiple Suggestions Panel
- **Shortcut:** Press `Ctrl + Enter` (or `⌘ + Enter` on Mac).
- **Detail:** Reveals additional code snippet options for more flexible selection.

### e. In-Line Chat & Focus Navigation
- **Shortcut:**
  - **Start Inline Chat:** `Ctrl + I` (or `⌘ + i` on Mac)
  - **Move Focus to Copilot Chat:** `Ctrl + Alt + i` (or `⌘ + Ctrl + i` on Mac)
- **Detail:** Enhances your interactive development experience directly within your editor.

---

## 3. Copilot Chat & Agent Function Features

### a. Agent Commands in Copilot Chat
- **Usage:** Prefix your queries to scope them:
  - `@workspace`: For queries related to workspace files.
  - `@terminal`: For tasks concerning the terminal.
  - `@vscode`: For Visual Studio Code functionalities.

### b. Slash Commands
#### Workspace Commands:
- **`/explain`:** Explains what a selected block of code does.
- **`/fix`:** Suggests improvements or corrections (e.g., fixing typos).
- **`/tests`:** Generates unit tests (the article uses Jest as an example).
- **`/new`:** Creates a new workspace based on natural language instructions.

#### Editor & Terminal Commands:
- **Editor (`/search`):** Searches for files within the workspace (for VS Code).
- **Terminal (`/explain`):** Explains commands executed in the terminal.

#### Global Chat Commands:
- **`/help`:** Displays guidance for using Copilot Chat.
- **`/clear`:** Resets the chat session for new contexts.

### c. Context Variables
- **`#codebase`:** Provides an overview of the entire workspace code.
- **`#selection`:** Explains or expands on selected code segments.

---

## 4. GitHub Copilot Subscription Plans

### Individuals

- **Free Plan ($0/month):**  
  - **Limits:**
    - Up to 50 chat/Agent mode requests per month.
    - Up to 2,000 code completion suggestions per month.
  - **Access:**
    - Includes models such as Claude 3.5 Sonnet and GPT-4o.

- **Pro Plan ($10/month or $100/year):**  
  - **Enhancements over Free:**
    - Unlimited chat/Agent mode requests using GPT-4o.
    - Unlimited code completions.
    - Access to additional models like Claude 3.7 Sonnet and o1 for code review.
    - Premium requests on the latest models increased up to 6× that of the Free plan (additional purchases available).

- **Pro+ Plan ($39/month or $390/year):**  
  - **Extra Benefits:**
    - Includes all Pro features.
    - Access to GPT-4.5 and all other available models.
    - Premium requests capacity increased up to 30× that of the Free plan (additional purchases available).

### Business / Enterprise

- **Business Plan ($19/month per user):**
  - **Features:**
    - Unlimited chat/Agent mode requests using GPT-4o.
    - Unlimited code completions.
    - Access to code reviews with models like Claude 3.5/3.7 Sonnet and o1.
    - Monthly cap of 300 premium requests per user (with additional purchase options).
    - Additional tools for user management, usage metrics, intellectual property protection, and data privacy safeguards.

- **Enterprise Plan ($39/month per user):**
  - **Expanded From Business:**
    - Includes all features of the Business plan.
    - Extends access to GPT-4.5 and all other models.
    - Premium request capacity increased by a factor of 3.33 compared to the Business plan (with additional purchase options).

---

## 5. GitHub-Specific Enhancements

### a. Commit Message Generation
- **Tip:** Use Copilot to auto-generate commit messages for your code changes.
- **Detail:** By clicking the dedicated star icon (or similar UI element), Copilot reviews your changes and generates commit messages that accurately describe them.

### b. Exploring GitHub Spark
- **Tool:** GitHub Spark (currently in technical preview).
- **Detail:** Enables users to build and share micro-applications using natural language inputs, making app development accessible even without extensive coding experience.

---

## 6. Additional (Extra) Tips Not Covered in the Article

### a. Regularly Update Copilot & Your IDE
- **Tip:** Keep GitHub Copilot and your code editor updated to leverage the latest features and improvements.

### b. Integrate Linters & Code Formatters
- **Tip:** Use Copilot alongside linters (ESLint, Pylint) and formatters (Prettier, Black) to maintain code quality and style consistency.

### c. Experiment with Custom Prompts
- **Tip:** Try different ways of phrasing comments or instructions to elicit more accurate or creative code suggestions.

### d. Use Copilot as a Virtual Pair Programmer
- **Tip:** Consider Copilot as a collaborative partner. Discuss potential solutions out loud or document your thought process in comments, then seek alternative approaches using Copilot.

### e. Tailor Copilot Settings
- **Tip:** Adjust configuration settings to match your coding style and workflow, such as suggestion frequency and context length.

### f. Combine with Version Control Reviews
- **Tip:** Complement Copilot-generated code with thorough code reviews to catch nuances and ensure robust logic.

### g. Document Your Copilot Use Cases
- **Tip:** Maintain documentation on how you integrate Copilot into your workflow—this helps refine practices and share best practices with your team.

---
