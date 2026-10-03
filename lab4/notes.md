Q1. Including --global saves the Git username and email as our computer user account's default settings, applying them across every repository we work on. Omitting --global configures those details exclusively for your active project.

Q2. The .git folder shows up in ls -a instead of ls because its leading dot marks it as a hidden directory. It houses Git's internal engine, including configuration settings, commit history, and reference pointers.

Q3. Git was proposing to track files and folders in your directory. Based on my output showing 3 files changed, Git tracked only the 3 specific files (such as README.md, .gitignore, and your main script) while leaving out untracked items like .venv.

Q4. Once .gitignore was added, Git stopped tracking .venv/ and its contents entirely. The .venv folder disappeared from git status, while .gitignore itself appeared as an untracked file ready to be staged.

Q5 .gitignore should be committed rather than ignoring it. Saving it in the repository ensures that everyone collaborating on the codebase shares the exact same rules for ignored files.

Q6. README.md shifted from "Untracked files" over to "Changes to be committed." Under Git's three-stage architecture, git add README.md moved the file from the working directory into the staging area (index).

Q7. [master (root-commit) dc5db85 ] Initial commit 3 files changed, 5 insertions(+)

Q8. The sequence dc5db85 represents the first seven characters of an abbreviated SHA-1 commit hash. This hash acts as a unique ID, making it straightforward to pinpoint and reference that specific snapshot.

Q9. The standard development loop follows four steps: make code edits then inspect changes via git status → stage updates using git add → save a snapshot with git commit. This loop is repeated whenever I make changes that I want to save in Git history.

Q10. GitHub automatically renders any root README.md right on the project's primary landing page. This makes it the ideal landing document to brief visitors on what the project does without requiring them to dig through individual files.

Q11. gh auth login authenticated my GitHub account and configured Git to use my GitHub credentials for HTTPS operations. This means Git can authenticate my pushes without asking me for my GitHub password each time.

Q12. The README.md file is showing on the front page of the GitHub repository. GitHub automatically displays a root README.md as the repository’s introduction and documentation.

Q13. No, pushing did not change my local history. It only copied my existing local commits to the GitHub repository; the commits and their history remained the same locally.

Q14. A private repository exists on GitHub, but only the owner and people who have been given access can view or work with it. If a repository does not exist on GitHub, there is no online copy of the project or its Git history to access.