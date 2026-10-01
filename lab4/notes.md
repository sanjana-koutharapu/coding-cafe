## Question 1

`--global` means the Git configuration applies to all repositories for my user account on this computer. If I leave out `--global`, the setting applies only to the current repository.

## Question 2

The `.git` directory appeared when I ran `git init`. It contains Git's internal information, including the repository's history, configuration, and information Git uses to track files.

## Question 3

[Put the approximate number of files/folders you saw in your ORIGINAL `git status` here.] Some of the files were existing project files, and the `.venv` files were not something I wrote and should not be tracked.

## Question 4

After creating `.gitignore`, the files inside `.venv/`, along with other ignored files such as Python cache files, disappeared from the `git status` output. Git now ignores those files.

## Question 5

`.gitignore` should be committed because it is part of the project's configuration and tells Git which files should be ignored. It should not be ignored itself because other people who clone the repository need the same rules.

## Question 6

`README.md` moved from the untracked/working-tree section into the staged section after I ran `git add README.md`. In the three-places model, the file moved from the working directory to the staging area.

## Question 7

[Use the actual output from your `git commit` command here.] Git created a commit and reported the number of files changed.

## Question 8

The first seven characters of the commit hash are a shortened version of the commit's unique SHA-1 identifier. They can be used to refer to and identify that specific commit.