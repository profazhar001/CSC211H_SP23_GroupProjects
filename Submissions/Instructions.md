# Instructions for Setup, Work, and Submission
This document will outline the steps that you will need to take to get started work on and submit your project. It is
focused on the technical aspects of the project (git/GitHub), and does not cover the actual project itself.
For information on the project itself, please see **ADD LINK HERE**.

## Goal
You and your teammates will be developing this project together, and as such, will need to be using git and GitHub
to collaborate. This project will be a good opportunity to practice using these tools to solve real world problems.

**Please read all the steps before starting any actions.**

## Setup
Of course before writing any code, your team will need a repository to work in.
There are a couple options for getting set up, but this is probably the simplest:
1. One team member forks this repository.
2. The forked repository will now be your team's repository and home for the project.

You could potentially just make a new repository,
however because you will be eventually submitting to this repo, it is marginally simpler to just fork it.

### Should I add my teammates as collaborators?
While it might seem like the obvious next step is to add your teammates as collaborators to your repo,
this is one of the decisions that you will need to make as a team.

*Here are the pros and cons of adding your teammates as collaborators:*

**Pros:**
* Everybody can push to the repo.
* You don't have to use pull requests.
* Everybody doesn't have to fork the new repo.

**Cons:**
* Everybody can push to the repo.
* You don't have to use pull requests.

There is a reason why GitHub has a pull request system. Not adding collaborators to your repo will force you to use it.
You may find it useful to have your teammates review your code via pull requests before merging it into the main branch.
Also, generally speaking, the more people that have full access to a repo, the more likely it is that somebody will
make a mistake using git that could cause problems for the whole team.

But as you can imagine, having to review every additional commit will slow things down. Balancing development speed
and safety is one of the many challenges real developers face every day.



## Working
Now that your team has a repo of its own, you can start writing code. Be sure that all your changes are only
sent to your team's fork, and not to this repo.

Depending on whether you added your teammates as collaborators or not based on the notes above,
you will need to use git a little differently.

**So it's clear:** *If you decide to add your teammates as collaborators*, everybody can clone your team's main fork,
and then just push changes to the team fork. *If you decide **not** to add your teammates as collaborators*, then each
teammate will need to fork the team fork, and then each teammate will push their own changes to their own fork,
and then submit their own changes via pull request to the team's main fork. One teammate, who is the owner of the
team's main fork, will be able to simply push to their own fork as they please.

## Submission
Once you have completed your project, you will need to submit it to this repo. If you originally forked this repo,
this will be as simple as making a pull request from your team's fork to this repo. There should be **ONE** directory
added to `Submissions/` in your pull request (though you can have subdirectories within your team's directory as you please).
The name of the directory should be your team name, and it should contain a `README.md` file that contains the
following information:

* Your team name
* A link to your team's fork
* A list of your team members, their GitHub IDs, and their BMCC ID's
* A list of your team members' contributions to the project

You can add anything else you want to the `README.md` file, but the above information is required.
Your directory should also only include your *src* files `*.cpp, *.h` and your `README.md`
it should **NOT** include any of the following:
* `.git` directory
* `.idea/.solution/etc..` directory (anything made by IDE's)
* `.exe` files (or anything else that is executable)

##  Notes:
If you have forgotten or do not know some of the commands I have referenced in this document, here is a short list of them and their usages.
For more details, visit [git_scm](https://git-scm.com/) or Google (git is probably the most used software by developers, so there are plenty of resources online).
```
git clone <link_to_repo>
# clones repository to your shell's working dir

git add <file(s) with changes>
# stages changes

git commit -m <message>
# commits staged changes

git fetch <remote>
# fetches all remote branches (does not affect your local branches)

git merge <branch>
# incorporates commits from <branch> into your current branch

git pull <remote>
# fetches all remotes and merges them into your local branches
# basically equal to git fetch <remote> followed by git merge origin/<current-branch>

git push <remote> <branch>
# pushes changes from current branch, moves remote HEAD to latest commit
```

For forking and pull requests, do so in your browser in GitHub.
