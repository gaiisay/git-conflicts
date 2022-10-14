# Git Conflicts Template

This template has a few conflicts to help you practice resolving them.

> ❗️ **Important:** Follow these instructions carefully step by step.

> 💡 This repo has to be imported into your own GitHub account using the import feature to keep all the commits of this template repo. The normal GitHub Template feature flattens the history of the template repo and you will not be able to see the conflicts.

## Getting Ready

1. [command+click here to create a new repository on GitHub.com using the import repository feature](https://github.com/new/import).
2. Use this URL to import the template:

```
https://github.com/JessicaLoers/web-git-conflicts-template
```

3. Create it as `git-conflics` in your own account. Click on "Begin import" and wait for the import to finish.
4. In your new Repository open pull requests for the `pirate`, `full-date` and `styling` branches.  
   _It's easiest to do this by command-clicking on the "Compare & pull request" buttons that appear after you have created the repository on GitHub._
5. Clone your repository to your computer.

All three branches should now show conflicts in the Pull Request interface.

## Resolving Conflicts

### 1. `pirate` Branch (using `merge` on the command line)

Switch to the `pirate` branch locally and merge `main` into it.

#### Resolve the Conflict

Git now shows:

```
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
```

Resolve the conflict by logically combining the changes from both branches:

- `pirate` translated the introduction to pirate speak
- `main` removed a redundant half sentence "and how to build a shelter"

Keep the translation from `pirate` and remove the redundant half sentence: "and how 't build a shelter", remove "," ,add "and ".
At the end the sentence should be: "ye will also learn how t' build a fire and how t' make a trap". 

#### Push the Changes

Push your new changes to the `pirate` branch and look at the Pull Request.

#### Merge using the Pull Request

Merge the `pirate` branch into `main` using the Pull Request interface and delete the `pirate` branch.

### 2. `full-date` Branch (using Resolve Conflicts on GitHub)

Go to the Pull Request for the `full-date` branch and click on the "Resolve conflicts" button above the disabled "Merge pull request" button.

#### Resolve the Conflict

Resolve the conflict by logically combining the changes from both branches:

- `full-date` changed the code to show the full date
- `main` refactored the code to only on line

Keep the changes from `full-date` as-is since the refactor to one line (on the `main` branch) was not necessary. (Accept the current change.)

Mark the conflict as resolved by clicking "Mark as resolved" and then commit it with the "Commit merge" button.

#### Merge using the Pull Request

Merge the `full-date` branch into `main` using the Pull Request interface and delete the `full-date` branch.

### 3. `styling` Branch (using `merge`)

❗️ Go to the `main` branch locally and pull any changes from the remote before starting.

Repeat the steps of part 1 but for the `styling` branch.

To resolve the conflicts, keep the changes from the `styling` branch that introduce custom properties to the CSS but set the `--max-width` property to `68ch` (the new value from the `main` branch).

#### Push the Changes

Push your new changes to the `styling` branch and look at the Pull Request.

#### Merge using the Pull Request

Merge the `styling` branch into `main` using the Pull Request interface and delete the `styling` branch.

---

> 👏 **Congratulations! You have successfully resolved all conflicts and all changes are in `main`.**
