## Question 1

`--global` means the Git configuration applies to all repositories for my user account on this computer. If I leave out `--global`, the setting applies only to the current repository.

## Question 2

The `.git` directory appeared when I ran `git init`. It contains Git's internal information, including the repository's history, configuration, and information Git uses to track files.

## Question 3

Git was offering to track approximately 1,100 files and folders. Most of these were files inside `.venv/`, which were not something I wrote and should not be tracked.

## Question 4

After creating `.gitignore`, the files inside `.venv/`, along with other ignored files such as Python cache files, disappeared from the `git status` output. Git now ignores those files.

## Question 5

`.gitignore` should be committed because it is part of the project's configuration and tells Git which files should be ignored. It should not be ignored itself because other people who clone the repository need the same rules.

## Question 6

`README.md` moved from the untracked/working-tree section into the staged section after I ran `git add README.md`. In the three-places model, the file moved from the working directory to the staging area.

## Question 7

Git created the commit with the message "Initial commit". It reported that 3 files changed, with 162 insertions.

## Question 8

The first seven characters of the commit hash are a shortened version of the commit's unique SHA-1 identifier. They can be used to refer to and identify that specific commit.

## Question 9

The four steps are edit, stage, commit, and repeat. First I make a change to a file, then use `git add` to stage it, `git commit` to save it in the repository history, and then repeat the process for future changes.

## Question 10

`README.md` has a special name because GitHub automatically displays it on the repository's front page. It acts as an introduction to the project and gives readers information about the repository and its contents.

## Question 11

`gh auth login` authenticated my GitHub account through the browser and stored the authentication credentials locally. This means Git can use those credentials when pushing to GitHub instead of asking me for a password each time.

## Question 12

The `README.md` file is shown on the GitHub repository's front page because GitHub automatically renders a README as the repository's introduction. It displays the Markdown as formatted text rather than showing the raw Markdown syntax.

## Question 13

No, pushing did not change my local Git history. `git push` copied my existing commits to GitHub, while the commits and their hashes remained the same locally.

## Question 14

A private repository exists on GitHub but its contents can only be accessed by people who have permission. A repository that does not exist on GitHub cannot be accessed there at all, because there is no remote repository containing the project.