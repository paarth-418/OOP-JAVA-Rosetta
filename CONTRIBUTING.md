# Contributing to OOP + JAVA Rosetta Encyclopedia

Thank you for interest in improving this learning resource! This document outlines how to contribute effectively.

## 🎯 Our Mission

The **OOP + JAVA Rosetta Encyclopedia** is a mental-model-first reference for understanding object-oriented programming and Java. We prioritize:

- **Conceptual clarity** over surface-level explanations
- **Deep understanding** through progressive complexity
- **Pedagogical rigor** (learning objectives, practice, reinforcement)
- **Professional presentation** that respects the reader's time

---

## 📋 Types of Contributions

### 1. **Content Improvements** 📝
- Clarifying existing explanations
- Adding code examples (implementation details)
- Expanding mental models with better analogies
- Writing practice exercises
- Adding section summaries and learning objectives

### 2. **LaTeX & Design** 🎨
- Improving formatting consistency
- Enhancing visual hierarchy
- Creating new explanation boxes (diagrams, tables)
- Optimizing typography and readability
- Cleaning up commented code

### 3. **Expert Review** 👨‍🎓
- Reviewing content for technical accuracy
- Suggesting industry best practices
- Adding real-world design pattern examples
- Validating code samples
- Improving pedagogical effectiveness

### 4. **Structure & Organization** 🏗️
- Planning missing chapters
- Creating roadmaps
- Organizing content into logical flow
- Building exercises and assessments

---

## ✅ Contribution Standards

### Content Standards

Every section must have:

1. **Learning Objective** (at the top)
   ```latex
   \textbf{After this section, you should understand:}
   \begin{itemize}
   \item [::] What X is
   \item [::] Why X matters
   \item [::] How to use X
   \end{itemize}
   ```

2. **Core Explanation** (conceptual foundation)
   - Use \mintinline{} for inline code, \begin{minted}{} for blocks
   - Employ mental models for difficult concepts
   - Progress from "why" → "what" → "how"

3. **Practical Examples** (implementation-focused)
   - Real, runnable Java code
   - Multiple examples when possible
   - Annotated with explanations

4. **Common Pitfalls** (trap boxes)
   ```latex
   \begin{trap}
   \emph{Beginners often}:
   % Mistake here
   This is wrong because...
   \end{trap}
   ```

5. **Section Summary** (retention reinforcement)
   ```latex
   \textbf{Key Takeaways:}
   \begin{itemize}
   \item [*] Point 1
   \item [*] Point 2
   \end{itemize}
   ```

6. **Exercises** (practice problems)
   - Minimum 2-3 per section
   - Start easy, progress to challenging
   - Include solutions in appendix

### LaTeX Standards

#### Visual Hierarchy
Use tcolorbox types consistently:
- **`\begin{rosettarule}`** — Core principles and guidelines
- **`\begin{idea}`** — Deep insights and "aha moments"
- **`\begin{mentalmodel}`** — Analogies and conceptual frameworks
- **`\begin{trap}`** — Common mistakes and misconceptions
- **`\begin{compressionbox}`** — Summaries and synthesis

#### Code Blocks
```latex
% Inline code
\mintinline{java}{variableName}

% Code blocks with line numbers
\begin{minted}{java}
public class Example {
    // Code here
}
\end{minted}
```

#### Formatting Rules
- Use `\textbf{}` for emphasis, not `\textit{}` for definitions
- Use `\textcolor{RosettaOrange}{}` for important keywords
- Maintain 1-inch margins and 11pt font
- Keep line length readable (avoid long wrapped lines)

#### Clean Code
- Remove commented-out sections (explain them in git history instead)
- Document all custom commands
- Keep packages organized and justified
- Comment non-obvious LaTeX choices

---

## 🚀 How to Contribute

### Step 1: Choose Your Contribution

**Small fixes** (typos, clarifications, minor examples):
- Fork the repo
- Create a branch: `git checkout -b fix/issue-description`
- Make changes
- Submit a pull request with description

**Major additions** (new sections, chapters, exercises):
- First, **open an issue** with your proposal
- Discuss approach with maintainers
- Get approval before investing time
- Then proceed with branch and PR

### Step 2: Fork and Setup

```bash
git clone https://github.com/YOUR-USERNAME/OOP-JAVA-Rosetta.git
cd OOP-JAVA-Rosetta
git checkout -b contribution/your-contribution-name
```

### Step 3: Make Your Changes

**For content contributions:**
- Edit `java.tex` or create a new `.tex` file if starting a new chapter
- Follow content and LaTeX standards above
- Test compilation: `pdflatex java.tex` or `xelatex` or [Compile Commands](./javaMaterialCompileCommands.md)

**For design contributions:**
- Update the relevant section in `java.tex`
- Test visual output (view PDF)
- Ensure colors match the Rosetta palette

### Step 4: Commit with Clarity

```bash
# Good commit messages
git commit -m "Add exercises for Chapter 1: Why OOP Exists"
git commit -m "Clarify mental model for object responsibility"
git commit -m "Fix LaTeX formatting in section 2.3"

# Bad commit messages
git commit -m "Fix stuff"
git commit -m "Update"
```

### Step 5: Submit Pull Request

In your PR description, include:
- **What**: What did you change and why?
- **Type**: Content, LaTeX, exercises, review feedback?
- **Testing**: How did you verify (compiled PDF, clarity check, etc.)?
- **Standards**: Does it follow contribution standards?

**Example PR description:**
```markdown
## What
Added 5 practice exercises for "Why OOP Exists" chapter.

## Type
Content addition + exercises

## Changes
- Added 3 conceptual exercises (understanding mental models)
- Added 2 code-writing exercises (translating concepts to Java)
- Added solution sketches in appendix

## Testing
- Verified PDF compiles without errors
- Reviewed exercises for clarity and progression
- Checked LaTeX formatting against standards

## Standards Checklist
- [x] Follows content standards (learning objectives, examples, traps)
- [x] Uses correct tcolorbox types
- [x] Code examples are runnable
- [x] Exercises progress in difficulty
```

---

## 📊 Current Roadmap & Needs

See **[ROADMAP.md](./ROADMAP.md)** for complete roadmap.

---

## 🎓 Review Process

### For Contributors
1. **Submit PR** with detailed description
2. **Maintainer review** (content + LaTeX + pedagogy)
3. **Request changes** or approve
4. **Merge** once standards are met

### For Reviewers
Evaluate based on:
- ✅ **Accuracy**: Is the content technically correct?
- ✅ **Clarity**: Is it understandable to the target audience?
- ✅ **Consistency**: Does it match existing style and standards?
- ✅ **Completeness**: Does it cover learning objectives, examples, exercises?
- ✅ **Pedagogy**: Does it teach effectively?

---

## 💬 Getting Help

- **Questions about structure?** Open an issue tagged `question`
- **Need feedback on draft?** Open a draft PR
- **Want to discuss an idea?** Open an issue tagged `discussion`
- **Found an error?** Open an issue with `bug` label

---

## 📜 License

By contributing, you agree that your work will be licensed under the same license as this project (to be determined).

---

## 🙏 Thank You!

We appreciate educators, experts, and learners who invest in making this resource better. Your contributions make OOP more accessible and understandable for everyone.

---

**Ready to contribute?** Check the [ROADMAP.md](./ROADMAP.md) for open positions and comment on an issue to claim a task!
