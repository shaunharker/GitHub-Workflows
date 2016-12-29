# GitHub-Workflows

**Shaun Harker 2016-12-29**  <https://shaunharker.github.io/GitHub-Workflows/>

## Summary

In this GitHub project I provide [two tutorials](https://shaunharker.github.io/GitHub-Workflows/) (one is shorter, one is longer) on `git` and `GitHub` in hopes of lowering the barrier of entry for academics to use these tools for collaborative writing (particularly, with Latex). 

In particular [the shorter of the two tutorials](https://shaunharker.github.io/GitHub-Workflows/Branching-Workflow/GitHub-Branching-Workflow.html)  describes a GUI-based GitHub workflow which is completely point-and-click and does not require the command line.

Advantages of using GitHub include:

* Overcoming the "only-one-editor-at-a-time" problem, which puts people under time pressure to make changes so they can pass it along
* Being able to track contributions and progress
* Line-by-line comparisons of changes
* Well-polished GitHub functionality for commenting on changes, bringing up issues, and discussing directions


## Workflows 

A great summary of workflows with nice pictures can be found on the Atlassian site <https://www.atlassian.com/git/tutorials/comparing-workflows/>.

The tutorials I provide refer to the _feature branch workflow_, (or just _branching workflow_) and the _forking workflow_ discussed on the Atlassian site. These correspond to the shorter and longer tutorials, respectively.

The two workflows I don't discuss which are mentioned on the Atlassian link are the _centralized workflow_ and the _gitflow workflow_. The _centralized workflow_ is to be avoided because it gives up, for hardly any benefit, a key feature that contributions are presented as "Pull Requests" (PRs) and subject to maintainer review. Instead, everyone just does naked commits against the main "branch" of a single repository. That makes it way too easy to make mistakes.

Meanwhile, the _gitflow workflow_ is perhaps interesting, but it is  needlessly complex for the needs of most academic writing projects.

The _branching workflow_ is a minimal adjustment to the centralized workflow where you commit against another "branch" and request maintainer review. This adds safety, even if you do the review yourself. The additional step prevents accidentally clicking a button and mucking up the repo for everybody else. It gives the opportunity to use the tools on GitHub to make sure the changes pass a sanity test before imposing them onto the main branch (and hence onto everyone else, who expects pulling from the main branch will be safe). The branching workflow can be accomplished without a command line and instead using only GUI (graphical user interface, i.e. point-and-click) tools. Command-line user types can ignore the GUI and participate easily as well.

The _forking workflow_ has some extra advantages but requires the command line and thus is a significantly higher ask for people to learn. But there is far better protection against mistakes from coauthors and also more flexibility. The great advantage to this kind of workflow is that it allows for a much larger group of collaborators without running risks. This is the workflow used by software develpers on GitHub and it is so robust and safe that it allows strangers to make contributions to code repositories.

## Terminology: Branches and Forks

The terms _branching workflow_ and _forking workflow_ arise from the `git` concepts of "branch" and "fork". 

A single repository can have many so-called _branches_, and depending on which branch is "checked out" one has what is in principle a wholly independent version of the project. These branches can be used to develop something in isolation without breaking the main version until the changes are fully ready. Note that in principle all branches are on a technical level equivalent, but in practice there is a special branch named `master` which is understood to be the main branch.

_Forks_, on the other hand, refer to wholly different repositories, belonging to different people. A forked repository is a copy of a repository one person makes of another person's repository. The idea is that someone will make a their own personal forked copy, do their development, and then eventually come back and submit their proposed changes to the main repository. In principle all forks are on a technical level equivalent, but in practice there is an "official" (or main) repository which is understood to be the main fork (i.e. the first version, so it wasn't created by actually forking; although sometimes a fork later becomes the main repo when the project originator hands off maintenance duties).

## Pull Requests

In both branching and forking workflows the key concept is that there is a `master` "branch" of a main repository (i.e. main "fork") and the ultimate goal is to copy it (i.e. pull other author's contributions from it), improve it, and then issue a _Pull Request_ (PR). Project maintainers inspect pull requests and either approve them or request fixes. 

In the branching workflow, there is only one repository but many "branches" within it, and a pull request from a coauthor Alice will ask that the `master` branch pull from Alice's development branch `alice-dev`. 

In the forking workflow, there are many repositories mirroring a main repository, and a pull request asks that the `master` branch of the main repository will pull from one of the coauthor's branches in their forked repository. (It could be their `master` branch, but actually this can cause problems if they make commits after a pull request and don't realize they are changing the PR by doing so!)

## Tutorials

With this background (or perhaps even without it), hopefully the [tutorials](https://shaunharker.github.io/GitHub-Workflows/) can be understood. And of course, there is always Google. Since `git` and `GitHub` are extremely widely used, there is no shortage of resources.  



