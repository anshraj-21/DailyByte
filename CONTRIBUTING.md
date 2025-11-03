# 🤝 Contributing to DailyByte

Thank you for your interest in contributing to **DailyByte**! This document provides comprehensive guidelines to help you submit your solutions effectively.

---

## 📋 Table of Contents

1. [Code of Conduct](#-code-of-conduct)
2. [Getting Started](#-getting-started)
3. [Submission Guidelines](#-submission-guidelines)
4. [Naming Conventions](#-naming-conventions)
5. [AI Usage Policy](#-ai-usage-policy)
6. [Code Quality Standards](#-code-quality-standards)
7. [Pull Request Process](#-pull-request-process)
8. [Review Process](#-review-process)
9. [Common Mistakes to Avoid](#-common-mistakes-to-avoid)

---

## 🌟 Code of Conduct

By participating in DailyByte, you agree to:

- ✅ **Be respectful** to all community members
- ✅ **Write original code** without plagiarism
- ✅ **Learn from mistakes** and help others learn
- ✅ **Follow submission guidelines** strictly
- ❌ **Never use AI tools** for generating solutions
- ❌ **Never copy code** from others or the internet
- ❌ **Never submit** code that you don't understand

### ⚠️ Violations will result in:
- First offense: Warning and PR rejection
- Second offense: Temporary ban from submissions
- Third offense: Permanent exclusion from the program

---

## 🚀 Getting Started

### Prerequisites

Before contributing, ensure you have:

- A GitHub account
- Git installed on your machine
- Basic understanding of Git commands
- A code editor (VS Code, PyCharm, etc.)
- Your ERP ID ready

### Initial Setup

1. **Fork the Repository**
   ```bash
   # Click the 'Fork' button on GitHub
   ```

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/DailyByte.git
   cd DailyByte
   ```

3. **Set Upstream Remote**
   ```bash
   git remote add upstream https://github.com/Sayan-dev731/DailyByte.git
   ```

4. **Verify Remotes**
   ```bash
   git remote -v
   # Should show both 'origin' and 'upstream'
   ```

---

## 📝 Submission Guidelines

### Step-by-Step Process

#### 1️⃣ Sync Your Fork (Before Every New Solution)

```bash
# Fetch latest changes
git fetch upstream

# Switch to main branch
git checkout main

# Merge upstream changes
git merge upstream/main

# Push to your fork
git push origin main
```

#### 2️⃣ Create a New Branch

```bash
# Use the format: solution/MM-DD-YYYY
git checkout -b solution/11-02-2025
```

#### 3️⃣ Navigate to the Solution Folder

Each daily question has a dedicated solutions folder:

```bash
cd Daily-Solutions/11-02-2025/
```

If the folder doesn't exist, create it:

```bash
mkdir Daily-Solutions/11-02-2025
cd Daily-Solutions/11-02-2025/
```

#### 4️⃣ Create Your Solution File

Use the naming convention: **`githubusername_ERPID.extension`**

**Examples:**
- Python: `johndoe_2021001.py`
- JavaScript: `janedoe_2021002.js`
- Java: `alexsmith_2021003.java`
- C++: `emilybrown_2021004.cpp`

```bash
# Create your solution file
touch githubusername_ERPID.py
```

#### 5️⃣ Write Your Solution

Include the following in your solution file:

```python
"""
Problem: [Problem Name]
Date: [MM-DD-YYYY]
Author: [Your Name]
GitHub: [Your GitHub Username]
ERP ID: [Your ERP ID]

Approach:
[Explain your approach in 2-3 sentences]

Time Complexity: O(?)
Space Complexity: O(?)
"""

# Your code here
def solution():
    pass

# Test cases
if __name__ == "__main__":
    # Test with provided examples
    pass
```

#### 6️⃣ Test Your Solution

Before committing, ensure your solution:
- ✅ Passes all provided test cases
- ✅ Handles edge cases
- ✅ Runs without errors
- ✅ Follows the problem constraints

#### 7️⃣ Stage and Commit

```bash
# Add your file
git add Daily-Solutions/11-02-2025/githubusername_ERPID.py

# Commit with a clear message
git commit -m "Add solution for 11-02-2025 - [Your Name]"
```

#### 8️⃣ Push to Your Fork

```bash
# Push your branch
git push origin solution/11-02-2025
```

#### 9️⃣ Create a Pull Request

1. Go to your fork on GitHub
2. Click **"Compare & pull request"**
3. Use this PR title format: `Solution: [Problem Name] - [Your Name] (ERP: [ERP ID])`
4. Fill in the PR template (see below)

---

## 🏷️ Naming Conventions

### Branch Names
```
solution/MM-DD-YYYY
```
**Examples:**
- `solution/11-02-2025`
- `solution/12-25-2025`

### Solution File Names
```
githubusername_ERPID.extension
```

**Valid Examples:**
- ✅ `sayandev731_2024001.py`
- ✅ `john_doe_2024002.js`
- ✅ `alice-smith_2024003.java`

**Invalid Examples:**
- ❌ `solution.py` (missing username and ERP ID)
- ❌ `SayanDev.py` (missing ERP ID)
- ❌ `2024001.py` (missing username)
- ❌ `sayan dev 2024001.py` (spaces not allowed)

### Supported File Extensions

| Language | Extension |
|----------|-----------|
| Python | `.py` |
| JavaScript | `.js` |
| TypeScript | `.ts` |
| Java | `.java` |
| C++ | `.cpp` |
| C | `.c` |
| Go | `.go` |
| Rust | `.rs` |
| Ruby | `.rb` |
| PHP | `.php` |

---

## 🚫 AI Usage Policy

### ⚠️ **STRICTLY PROHIBITED**

The use of **ANY AI-powered tools** to generate, complete, or assist in writing solutions is **ABSOLUTELY FORBIDDEN**.

#### Prohibited Tools Include (but not limited to):
- ❌ ChatGPT / GPT-4 / GPT-3.5
- ❌ GitHub Copilot
- ❌ Amazon CodeWhisperer
- ❌ Tabnine AI
- ❌ Codeium
- ❌ Claude AI
- ❌ Bard / Gemini
- ❌ Any other AI code generation tools

### 🕵️ AI Detection

We use multiple methods to detect AI-generated code:
- Code pattern analysis
- Style consistency checks
- Complexity analysis
- Manual review by experienced developers

### ⚖️ Consequences of AI Usage

If we detect AI-generated code:

1. **First Violation:**
   - ❌ PR will be **rejected immediately**
   - ⚠️ Official warning issued
   - 📝 Recorded in your contribution history

2. **Second Violation:**
   - ❌ PR will be **rejected immediately**
   - 🚫 **Temporary ban** for 2 weeks
   - 📧 Notification to program coordinators

3. **Third Violation:**
   - ❌ **Permanent exclusion** from DailyByte
   - 🚫 **Blacklisted** from future participation
   - 📧 Report to academic institution (if applicable)

### ✅ What IS Allowed

- ✅ Reading documentation
- ✅ Searching for algorithm concepts
- ✅ Reviewing data structure tutorials
- ✅ Understanding time/space complexity
- ✅ Discussing approaches with peers (without sharing code)
- ✅ Using IDE features (syntax highlighting, auto-complete of keywords)

### ❌ What is NOT Allowed

- ❌ Pasting the problem into AI tools
- ❌ Asking AI to write any part of your solution
- ❌ Using AI to debug or optimize your code
- ❌ Copying code snippets from AI-generated sources
- ❌ Using AI to explain code that you then replicate

### 💡 Why This Policy Exists

The goal of DailyByte is to:
- Build YOUR problem-solving skills
- Develop YOUR coding abilities
- Prepare YOU for real technical interviews
- Help YOU learn to think algorithmically

**Using AI defeats the entire purpose of this program.**

---

## ✨ Code Quality Standards

### Required Elements

Every solution must include:

1. **Header Comment Block**
   ```python
   """
   Problem: [Problem Name]
   Date: [MM-DD-YYYY]
   Author: [Your Name]
   GitHub: [Your GitHub Username]
   ERP ID: [Your ERP ID]
   
   Approach:
   [Explain your approach]
   
   Time Complexity: O(?)
   Space Complexity: O(?)
   """
   ```

2. **Clean, Readable Code**
   - Use meaningful variable names
   - Add inline comments for complex logic
   - Follow language-specific style guides

3. **Test Cases**
   ```python
   # Include test cases at the end
   if __name__ == "__main__":
       # Test Example 1
       # Test Example 2
       # Test edge cases
   ```

4. **Error Handling** (where applicable)
   ```python
   def solution(input_data):
       if not input_data:
           return None  # or appropriate default
       # Your logic
   ```

### Code Style Guidelines

#### Python (PEP 8)
```python
# Good
def convert_to_spooky_case(variable_name: str) -> str:

# Bad
def f(s):

```

#### JavaScript (Airbnb Style)
```javascript
// Good
function convertToSpookyCase(variableName) {
}

// Bad
function f(s){}
```

---

## 🔄 Pull Request Process

### PR Title Format

```
Solution: [Problem Name] - [Your Name] (ERP: [ERP ID])
```

**Example:**
```
Solution: Spooky Case - Sayan Karmakar (ERP: 2024001)
```

### PR Description Template

When creating your PR, use this template:

```markdown
## 📋 Solution Details

**Problem:** [Problem Name]
**Date:** [MM-DD-YYYY]
**Author:** [Your Full Name]
**GitHub:** @[your-username]
**ERP ID:** [Your ERP ID]

## 🧠 Approach

[Explain your approach in 3-5 sentences. What algorithm or data structure did you use? Why?]

## ⏱️ Complexity Analysis

- **Time Complexity:** O(?)
- **Space Complexity:** O(?)

## ✅ Test Results

- [x] Example 1: Passed
- [x] Example 2: Passed
- [x] Example 3: Passed
- [x] Edge Cases: Passed

## 🎯 Challenges Faced

[Optional: Mention any challenges you faced and how you overcame them]

## 📚 Learning Outcomes

[Optional: What did you learn from solving this problem?]

---

## ✍️ Declaration

I hereby declare that:
- ✅ This solution is entirely my own original work
- ✅ I have NOT used any AI tools to generate or assist with this code
- ✅ I understand the logic and can explain every line of this code
- ✅ I have tested this solution thoroughly
- ✅ I have followed all contribution guidelines

**Signature:** [Your Name]
**Date:** [Current Date]
```

### PR Checklist

Before submitting, ensure:

- [ ] File name follows convention: `githubusername_ERPID.extension`
- [ ] File is in correct folder: `Daily-Solutions/MM-DD-YYYY/`
- [ ] Code includes header comment with all required information
- [ ] Solution passes all test cases
- [ ] Code is well-commented and readable
- [ ] Time and space complexity is analyzed
- [ ] No AI tools were used
- [ ] Declaration statement is included in PR description
- [ ] Branch name follows convention: `solution/MM-DD-YYYY`

---

## 🔍 Review Process

### Timeline

1. **Submission:** You create a PR
2. **Initial Review:** Within 24-48 hours
3. **Feedback:** If changes are needed, you'll receive comments
4. **Re-submission:** You make changes and push updates
5. **Final Review:** Within 24 hours of re-submission
6. **Merge:** If approved, your PR is merged

### What Reviewers Check

✅ **Correctness**
- Does the solution solve the problem?
- Does it pass all test cases?
- Are edge cases handled?

✅ **Code Quality**
- Is the code readable?
- Are variables meaningfully named?
- Is the logic clear?

✅ **Originality**
- Is this original work?
- Are there signs of AI usage?
- Is the coding style consistent?

✅ **Documentation**
- Is there a proper header comment?
- Are complex parts explained?
- Is complexity analysis correct?

✅ **Compliance**
- Correct file name?
- Correct folder location?
- All guidelines followed?

### Possible Outcomes

#### ✅ Approved and Merged
Your solution meets all criteria. Congratulations! 🎉

#### 📝 Changes Requested
Minor improvements needed:
- Add more comments
- Fix a bug
- Improve variable names
- Add test cases

**Action:** Make the requested changes and push to the same branch

#### ❌ Rejected
Your PR may be rejected for:
- AI-generated code detected
- Plagiarized code
- Incorrect file name or location
- Solution doesn't work
- Severe quality issues

**Action:** Start over with a new solution (if eligible)

---

## ⚠️ Common Mistakes to Avoid

### 1. Wrong File Naming
❌ `solution.py`
✅ `johndoe_2024001.py`

### 2. Wrong Folder Location
❌ `Daily-Solutions/solution.py`
✅ `Daily-Solutions/11-02-2025/johndoe_2024001.py`

### 3. Missing Header Comments
❌ No comments at all
✅ Complete header with all information

### 4. Not Testing Code
❌ Submitting without running
✅ Testing with all examples and edge cases

### 5. Unreadable Code
❌ Single-letter variables, no spacing
✅ Clear variable names, proper formatting

### 6. Wrong Branch Name
❌ `main`, `master`, `my-solution`
✅ `solution/11-02-2025`

### 7. Copy-Pasting from Internet
❌ Copying code from GeeksforGeeks, LeetCode, etc.
✅ Writing your own solution after understanding the concept

### 8. Using AI Tools
❌ Any AI assistance
✅ Your own brain power 🧠

---

## 💬 Getting Help

If you're stuck or have questions:

### ✅ Allowed
- Ask about **concepts** and **approaches**
- Discuss **algorithm choices**
- Get help with **understanding the problem**
- Ask about **debugging strategies**

### ❌ Not Allowed
- Asking someone to **write code for you**
- Sharing your **code for review** before submission
- Asking AI to **explain or generate solutions**

### Where to Ask
- Open an **Issue** on GitHub with your question
- Ask in community **discussion forums**
- Contact program **coordinators**

---

## 🎯 Best Practices

1. **Read the problem carefully** - Understand all constraints
2. **Plan before coding** - Think about the approach first
3. **Start simple** - Get a working solution first, optimize later
4. **Test frequently** - Test after writing each function
5. **Comment as you go** - Don't leave comments for later
6. **Learn from mistakes** - Review rejected PRs to improve
7. **Help others** - Share knowledge (not code!)
8. **Be consistent** - Participate regularly
9. **Stay honest** - Always submit original work
10. **Enjoy the process** - Learning is the goal, not just solving

---

## 📊 Contribution Statistics

Track your progress:
- Number of problems solved
- PR acceptance rate
- Code quality scores
- Consistency streak

Top contributors will be recognized in the community!

---

## 🙏 Acknowledgments

Thank you for being part of the DailyByte community! Your dedication to learning and honest effort is what makes this program valuable.

**Remember:** The struggle is part of the learning process. Every mistake is a lesson, and every solution you write makes you a better programmer.

---

## 📞 Questions or Concerns?

If you have questions about these guidelines:
- Open an issue on GitHub
- Contact repository maintainers
- Check the FAQ in the main README

---

**Happy Coding! 💻**

*Last Updated: November 2025*

---

## 📄 License

By contributing to DailyByte, you agree that your contributions will be licensed under the same license as the project.
