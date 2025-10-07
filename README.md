# Objective
Practice a real DevOps Git workflow: branch → change → PR → review → update → merge.

# Prerequisites
- You have access to this repo.
- Know your roll number and full name.

# Files to touch
- **Create:** `<roll-number>.txt` (put your full name inside)  
- **Edit:** `students.txt` (add your entry)

# Naming Rules
- **Branch name:** `task-<roll-number>`  
- **PR title:** `Add roll-<roll-number> – <Your Name>`  
- **students.txt entry format:** `YYYYMMDD_HHMM - Roll-number – Your Name`  
  *(Date and time of your commit, local timezone)*

# Steps
1. Create a new branch from `main` named `task-<roll-number>`.
2. Add your file: create `<roll-number>.txt` with your full name as the only content.
3. Update `students.txt` and add your line in the required format.
4. Commit your changes with a clear message describing what you did.
5. Push your branch to this repository.
6. Open a Pull Request (PR) to `main`:
   - **Title:** per naming rules  
   - **Description:** optional notes about your changes
7. Wait for review. You’ll get comments requesting changes (yes, on purpose).
8. Apply requested changes on the same branch and push again. Reply to each comment explaining what you changed.
9. Ensure checks pass and the PR is up to date with `main` (resolve conflicts if GitHub tells you).
10. Merge the PR after approval (use **Squash and merge** if available), then delete your branch.

# Verification on `main`
1. Your `<roll-number>.txt` exists with your name.
2. Your `students.txt` entry is present and correctly formatted.

# Acceptance Criteria
1. Correct branch/PR naming and file names.
2. Only the two intended changes are included.
3. `students.txt` entry is formatted and sorted correctly.
4. All review comments addressed (with replies).
5. PR merged cleanly; branch deleted.

# Common Gotchas
- Don’t edit files other than your two targets.
- Keep `students.txt` sorted—no “I’ll fix it later.” Later is how bugs are born.
- If a conflict appears, use the GitHub conflict editor to fix it on your branch, then re-request review.
- Make commits **atomic**: one logical change per commit (e.g., create file + update students.txt can be separate commits if desired).

