# Movie Links
Pull Requests(https://drive.google.com/file/d/1o6plTwi0Nr13CdOSHsf65gpG-FgLhL_1/view?usp=sharing)
# Pull Requests, Merge Conflicts, & Linking

## 1. Pull Requests (PRs)
*   **What they are:** A proposal to merge changes from one branch into another (usually from a feature branch into `main`) on GitHub.
*   **Why use them:** They allow team members to review code, run automated tests, discuss changes, and catch bugs before combining code into the main project.
*   **Basic Workflow:**
    1. Push your feature branch to GitHub: `git push origin <branch-name>`
    2. Open a Pull Request on the GitHub website.
    3. Request reviews, address feedback, and merge the code once approved.

## 2. Handling Merge Conflicts
*   **What they are:** Occur when Git cannot automatically combine code changes because two branches edited the exact same line of a file differently.
*   **How to resolve them:**
    1. Run `git pull` or `git merge`. Git will pause and flag the conflicting files.
    2. Open the file in your code editor to find the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).
    3. Manually edit the code to keep what you want and delete the conflict markers.
    4. Stage the fixed file: `git add <filename>`
    5. Complete the process: `git commit -m "Resolve merge conflict"`

## 3. Linking Pull Requests
*   **What it is:** Connecting a Pull Request directly to a GitHub Issue so they are associated with each other.
*   **How to do it:**
    *   **Using Keywords:** Write words like `closes #123`, `fixes #456`, or `resolves #789` in your PR description or commit message. When the PR is merged, GitHub will automatically close the linked issue.
    *   **Manual Linking:** Use the "Development" sidebar on the right-hand side of the GitHub PR page to search for and attach related issues manually.
