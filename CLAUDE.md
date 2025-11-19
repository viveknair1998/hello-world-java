# CLAUDE.md - AI Assistant Guide

> **Repository**: hello-world-java
> **Owner**: boslbosl
> **Purpose**: Simple "Hello World" program in Java
> **Last Updated**: 2025-11-19

## 📋 Project Overview

This is a minimalist Java project demonstrating the classic "Hello World" program. It serves as:
- A simple Java syntax demonstration
- A template for basic Java programs
- An educational resource for beginners learning Java

**Key Characteristics:**
- Single-file Java application
- No external dependencies
- No build tools (Maven/Gradle)
- Plain `javac` compilation

## 🗂️ Repository Structure

```
hello-world-java/
├── .git/                 # Git version control directory
├── .gitignore           # Ignores compiled .class files
├── HelloWorld.java      # Main source file
├── README.md            # User-facing documentation
└── CLAUDE.md            # This file - AI assistant guide
```

### File Descriptions

#### `HelloWorld.java`
- **Lines of Code**: 5
- **Purpose**: Prints "Hello world!" to console
- **Class Name**: `HelloWorld` (must match filename)
- **Entry Point**: `public static void main(String[] args)`

#### `.gitignore`
- **Excludes**: `*.class` (compiled bytecode files)
- **Reason**: Compiled files should not be version-controlled

#### `README.md`
- **Audience**: End users and developers
- **Contains**: Source code display, compilation, and execution instructions
- **Note**: Contains a typo "Excute" instead of "Execute" (line 27)

## 🔧 Development Workflow

### Compilation

```bash
javac HelloWorld.java
```

**What Happens:**
- Java compiler (`javac`) processes the source file
- Generates `HelloWorld.class` bytecode file
- `.class` file is ignored by git

**Requirements:**
- JDK (Java Development Kit) installed
- `javac` available in PATH

### Execution

```bash
java HelloWorld
```

**Expected Output:**
```
Hello world!
```

**Technical Details:**
- JVM loads `HelloWorld.class`
- Executes `main()` method
- `System.out.println()` writes to standard output

### Testing the Program

```bash
# Compile and run in sequence
javac HelloWorld.java && java HelloWorld
```

## 🌿 Git Conventions

### Branch Structure

- **Main Branch**: `main` (or `master` - check with `git branch`)
- **Feature Branches**: Use format `claude/claude-md-<session-id>`
- **Current Branch**: `claude/claude-md-mi60itxg1efxl1nk-01L3p8FaW2G9EPef1t72YAPb`

### Commit Message Guidelines

Follow these patterns based on recent commits:
- Use present tense: "Updating README.md", "Uploading Hello World program"
- Be descriptive but concise
- Examples from history:
  - `Updating README.md`
  - `Uploading Hello World program.`
  - `README.md updated`

### Push Protocol

Always use:
```bash
git push -u origin <branch-name>
```

**Important**: Branch names must start with `claude/` and end with matching session ID to avoid 403 errors.

## 📐 Java Conventions

### Code Style Observed

1. **Indentation**: 2 spaces (not tabs)
2. **Braces**: Opening brace on same line
3. **Class Declaration**: `public class HelloWorld {`
4. **Method Declaration**: `public static void main(String[] args) {`
5. **Line Breaks**: Simple and minimal

### Class Naming Rules

- **Filename MUST match class name**: `HelloWorld.java` → `class HelloWorld`
- Use PascalCase for class names
- One public class per file

## 🤖 AI Assistant Guidelines

### When Making Code Changes

1. **Preserve Formatting**: Keep 2-space indentation
2. **Match Style**: Follow existing conventions exactly
3. **Test After Changes**: Always compile and run to verify
4. **Minimal Changes**: This is a simple project - avoid over-engineering

### Common Tasks

#### Adding Functionality
```java
// Example: Adding a method
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello world!");
  }

  // New methods here, maintaining 2-space indent
}
```

#### Modifying Output
- Change the string in `System.out.println()`
- Recompile after changes
- Verify output matches expectation

### Files to NEVER Modify

- `.git/` directory contents
- `.gitignore` (unless specifically requested)
- Compiled `.class` files (they're generated, not source)

### Files to Update Carefully

- `README.md`: User-facing documentation - changes should enhance clarity
- `HelloWorld.java`: The core program - test thoroughly after changes

### Recommended Development Flow

1. **Read** existing code
2. **Plan** changes (use TodoWrite for multi-step tasks)
3. **Edit** files
4. **Compile** with `javac`
5. **Test** with `java`
6. **Commit** with clear message
7. **Push** to appropriate branch

## 🚨 Common Issues & Solutions

### Issue: "javac: command not found"
**Solution**: JDK not installed or not in PATH
```bash
# Check Java installation
java -version
javac -version
```

### Issue: "Could not find or load main class HelloWorld"
**Causes**:
- `HelloWorld.class` not in current directory
- Filename/class name mismatch
- Need to recompile

**Solution**:
```bash
javac HelloWorld.java  # Recompile
java HelloWorld        # Run (no .class extension)
```

### Issue: Git push returns 403
**Cause**: Branch name doesn't follow required pattern
**Solution**: Use branches starting with `claude/` and ending with session ID

## 📚 Project Context

### Educational Purpose
This repository is designed for:
- Learning basic Java syntax
- Understanding compilation vs. interpretation
- Practicing git workflows
- Template for simple Java programs

### Minimal Dependencies
- **No** Maven or Gradle
- **No** external libraries
- **No** frameworks
- Pure JDK-only project

### Simplicity is Key
When working on this codebase:
- Don't add unnecessary complexity
- Keep it beginner-friendly
- Maintain the educational value
- Preserve the "hello world" essence

## 🔄 Maintenance Notes

### README.md Typo
Line 27 contains "Excute" - this could be fixed to "Execute" if requested.

### Potential Enhancements (Only if Requested)
- Add comments to Java code
- Create variants (HelloWorld2, HelloWorld3)
- Add command-line argument handling
- Include package structure example
- Add build automation (Maven/Gradle)

**Default Stance**: Keep it simple unless user requests expansion.

## 📞 Quick Reference

### Essential Commands
```bash
# Compile
javac HelloWorld.java

# Run
java HelloWorld

# Compile and run
javac HelloWorld.java && java HelloWorld

# Check git status
git status

# Commit changes
git add .
git commit -m "Description of changes"

# Push to feature branch
git push -u origin claude/claude-md-<session-id>
```

### File Checklist
- [ ] `HelloWorld.java` - Source code
- [ ] `README.md` - Documentation
- [ ] `.gitignore` - Ignore compiled files
- [ ] `CLAUDE.md` - AI assistant guide (this file)

---

**For AI Assistants**: This is a straightforward project. Focus on clarity, correctness, and maintaining the educational simplicity. Always test changes by compiling and running the program. When in doubt, keep it simple.
