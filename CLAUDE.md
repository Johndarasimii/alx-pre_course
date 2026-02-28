# CLAUDE.md

## Repository Overview

This is the **ALX Pre-Course** repository for `Johndarasimii`. It is a learning
project from ALX School covering the fundamentals of Git, Bash scripting, and C
programming. The repository itself is the artifact — the work demonstrated here
is practicing version control workflows rather than shipping application code.

---

## Repository Structure

```
alx-pre_course/
├── README.md               # Root project readme ("My first readme")
└── 0x01-git/               # Git fundamentals project
    ├── README.md           # Project-level readme ("my second README.md")
    ├── .gitignore          # Ignores editor tilde-backup files (~)
    ├── up_to_date          # Contains the string "git pull"
    ├── bash/               # Bash script exercises
    │   ├── 98              # Empty placeholder file
    │   ├── ALX             # Empty placeholder file
    │   ├── alx             # Bash script: prints "ALX School is so cool!"
    │   └── school          # Bash script: prints "The school is open!"
    └── c/
        └── c_is_fun.c      # C source file placeholder
```

---

## Tech Stack & Language Conventions

### Bash scripts (`0x01-git/bash/`)
- Files use `#!/bin/bash` shebang on the first line.
- Scripts print simple strings to stdout (no arguments, no error handling needed
  at this level).
- No file extensions are used for executable scripts (ALX convention).

### C files (`0x01-git/c/`)
- Standard C source files (`.c` extension).
- ALX style: Betty coding style is the standard for ALX C projects (though not
  yet enforced at this precourse stage).

### `.gitignore`
- Currently contains a single entry: `~` (ignores vim/emacs tilde backup files).

---

## Git Workflow & Conventions

The commit history reflects the ALX Git learning curriculum. Key patterns to
preserve:

1. **Branching**: Work is done on `master`. Feature/personal branches are merged
   back with a merge commit (see commit `307d437`).
2. **Commit messages**: Short, imperative-style messages in English (e.g.,
   `"Hot fix"`, `"my last task"`).
3. **Merges**: Non-fast-forward merges are used to preserve branch history.
4. **No force-push**: The history is the record of learning; do not rewrite it.

### Development Branch for AI Contributions
When making AI-assisted changes, use the branch:
```
claude/add-claude-documentation-ZEWbr
```
Push with:
```bash
git push -u origin claude/add-claude-documentation-ZEWbr
```

---

## File & Naming Conventions

| Context          | Convention                                      |
|------------------|-------------------------------------------------|
| Bash scripts     | No extension, `chmod +x`, `#!/bin/bash` shebang |
| C source files   | `.c` extension, Betty style                     |
| README files     | `README.md` in every project directory          |
| Directory names  | `0xNN-topic` format (e.g., `0x01-git`)          |

---

## Common Tasks

### View project structure
```bash
find . -not -path './.git/*' | sort
```

### Check a bash script is executable and well-formed
```bash
bash -n 0x01-git/bash/<script>   # syntax check
```

### Run a bash script
```bash
bash 0x01-git/bash/alx
```

### Compile a C file
```bash
gcc -Wall -Werror -Wextra -pedantic 0x01-git/c/c_is_fun.c -o c_is_fun
```

---

## Important Notes for AI Assistants

1. **No build system**: There is no `Makefile`, `package.json`, or other build
   tooling. Do not introduce one unless explicitly requested.
2. **No tests**: There is no test suite. Correctness is verified by manual
   inspection or ALX auto-grader (not available locally).
3. **Minimal changes**: This is a precourse learning repo. Keep additions small
   and focused. Do not refactor existing files unless instructed.
4. **Preserve history**: Never amend or rebase existing commits. Always create
   new commits.
5. **ALX conventions**: File names, directory naming (`0xNN-topic`), and script
   style follow ALX School standards. Match these when adding new files.
6. **Author**: John Oladipo (`johndarasimi82@gmail.com`). Commits on the main
   learning path were made in November 2022.
