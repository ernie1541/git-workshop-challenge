# Git Workshop Challenge

Congratulations! You've made it to the Git challenge.

Your goal is to practice the basic Git and GitHub workflow:

**Fork → Clone → Branch → Edit → Commit → Push → Pull Request**

You will make a small change to this website and submit your change through a Pull Request.

---

## Challenge

You will modify the `index.html` file with your own information.

Find:

```html
<strong>YOUR NAME</strong>
```

and replace it with your name.

Then find:

```html
<strong>YOUR ANSWER</strong>
```

and replace it with your answer to:

*What is your favorite thing about coding?*

For example:

```html
<p>
    My name is <strong>Alex</strong>.
</p>
<p class="favorite">
    My favorite thing about coding is:
    <strong>building cool projects</strong>
</p>
```

---

## Instructions

### 1. Fork this repository
Click the **Fork** button at the top-right of this GitHub repository.
This creates your own copy of the repository under your GitHub account.

### 2. Clone your fork
Go to your fork and click:
**Code → HTTPS**
Copy the URL.
Then open your terminal and run:

```bash
git clone YOUR_REPOSITORY_URL
```

Move into the repository:

```bash
cd git-workshop-challenge
```

### 3. Create a feature branch
Do NOT make your changes directly on `main`.
Create a new branch:

```bash
git checkout -b add-my-info
```

You can replace `add-my-info` with another descriptive branch name.
For example:

```bash
git checkout -b add-john-info
```

Check that you are on your new branch:

```bash
git branch
```

You should see your new branch marked with `*`.

### 4. Edit the HTML file
Open the project folder in your code editor.
Open: `index.html`

Replace `YOUR NAME` with your name.
Then replace `YOUR ANSWER` with your answer to: *What is your favorite thing about coding?*

Save the file.

### 5. Check your changes
In your terminal, run:

```bash
git status
```

You should see that `index.html` has been modified.
You can also see exactly what changed with:

```bash
git diff
```

### 6. Stage your changes
Run:

```bash
git add index.html
```

### 7. Commit your changes
Create a commit:

```bash
git commit -m "Add my information"
```

### 8. Push your branch to GitHub
Run:

```bash
git push -u origin add-my-info
```

If you used a different branch name, replace `add-my-info` with your branch name.

### 9. Create a Pull Request
Go to your fork on GitHub.
You should see an option to create a Pull Request for your recently pushed branch.

Create a Pull Request with:
*   **Base repository:** The workshop instructor's repository
*   **Base branch:** `main`
*   **Compare branch:** Your feature branch

Give your Pull Request a title such as: `Add John Doe's information`

Then click: **Create pull request**

---

## Final Checklist
Before submitting your Pull Request, make sure:

- [ ] I forked the repository
- [ ] I cloned my fork
- [ ] I created a feature branch
- [ ] I edited `index.html`
- [ ] I ran `git status`
- [ ] I staged my changes with `git add`
- [ ] I committed my changes
- [ ] I pushed my branch to GitHub
- [ ] I created a Pull Request to the instructor's main branch

---

## Git Workflow
The workflow you just practiced is:

```text
Fork
  ↓
Clone
  ↓
Create Branch
  ↓
Make Changes
  ↓
git add
  ↓
git commit
  ↓
git push
  ↓
Pull Request
```

This is a simplified version of the workflow developers use when contributing to real projects.

---

## If You Get Stuck
Ask a workshop instructor or another attendee for help.
Common commands you may need:

```bash
git status
git branch
git diff
git add .
git commit -m "Your message"
git push
```

---

### One change I'd recommend for your workshop

Since you're specifically teaching **Git**, I would **not have them create a brand-new HTML file from scratch**. Having them modify `index.html` keeps the challenge focused on:

> **fork → clone → branch → modify → commit → push → PR**

You could make the final challenge slightly more interesting by having the **PR itself 