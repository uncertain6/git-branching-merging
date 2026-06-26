# Git Branching & Merging

These are my notes while learning Git branching and merging. This repository is mainly for practice and as a quick reference.

---

## Create a Branch

```bash
git branch <branch_name>
```

Creates a new branch.

---

## Switch Branches

```bash
git switch <branch_name>
```

Older command:

```bash
git checkout <branch_name>
```

---

## Merge Branches

```bash
git merge <branch_name> -m "message"
```

Merges another branch into the branch you're currently on.

**Easy way to remember:**

* On `main` → `git merge feature1` → `feature1` → `main`
* On `feature1` → `git merge main` → `main` → `feature1`

The branch you're standing on receives the merge.

---

## Abort a Merge

```bash
git merge --abort
```

Cancels an unfinished merge.

---

## Delete a Branch

```bash
git branch -D <branch_name>
```

Deletes a branch.

---

## Things I Learned

* Branches let you work on different features without affecting each other.
* `git switch` changes branches.
* `git merge` combines one branch into the current branch.
* The current branch always receives the merge.
* If a merge goes wrong, `git merge --abort` cancels it.
