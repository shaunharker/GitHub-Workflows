# GitHub-Workflows

**Shaun Harker 2016-12-29**  <https://shaunharker.github.io/GitHub-Workflows/>

## Summary

In this GitHub project I provide [tutorials](https://shaunharker.github.io/GitHub-Workflows/) on `git` and `GitHub` in order to lower the barrier of entry for academics to use these tools for collaborative writing (particularly, with latex).

Notably, see <https://github.com/HoTT/book> for a successful example of collaborative writing using `git`.

Advantages include:

* Overcoming the "only-one-editor-at-a-time" problem, which puts people under time pressure to make changes so they can pass it along
* Being able to track contributions and progress
* Line-by-line comparisons of changes
* Well-polished GitHub functionality for commenting on changes, bringing up issues, and discussing directions

A key hurdle in convincing people to use version control for collaboration is the relative inaccessibility of these tools to non-developers.

My goal with this repository is to address this by providing two possible workflows, along with tutorials, for how to use `git` and `GitHub` in order to collaborate on writing.

## Workflows 

The first workflow, which I refer to as the _branching workflow_, is very simplified and can be accomplished without a command line and instead using only GUI (graphical user interface, i.e. point-and-click) tools. Despite being simplified it still gives almost all of the many benefits. It also provides a stepping stone along the learning curve. Command-line users can ignore the GUI and participate easily as well.

The second workflow, the _forking workflow_, uses more concepts and requires the command line. There is better protection against mistakes and also more flexibility. The great advantage to this kind of workflow is that it allows for a much larger group of collaborators without running risks. This is the workflow used by software develpers on GitHub in order to allow strangers to make contributions.

## Terminology: Branches and Forks
These terminologies arise from the `git` concepts of "branch" and "fork". 

A single repository can have many so-called _branches_, and depending on which branch is "checked out" one has what is in principle a wholly independent version of the code. These branches can be merged in order to independent develop something without breaking another version until the changes are fully ready. In principle all branches are technically equivalent, but in practice there is a special branch named `master` which is understood to be the main branch.

_Forks_, on the other hand, refer to wholly different repositories. A forked repository is a copy of a repository one person makes of another person's repository. The idea is that will make a private copy, do their development, and then eventually come back and submit their proposed changes. In principle all forks are technically equivalent, but in practice there is a special fork, called the main repository, which is understood to be the main fork (i.e. the first version, so it wasn't created by actually forking; although sometimes a fork later becomes the main repo when the project originator hands off maintenance duties).

## Pull Requests

In both workflows the key concept is that there is a `master` "branch" of a main repository (i.e. "fork") and the ultimate goal is to copy it and then improve it. Contributors recommend their changes via issuing _Pull Requests_ (PRs), which the project maintainers inspect and either approve or request fixes. In the branching workflow, there is only one repository but many "branches" within it. In the forking workflow, there are many repositories mirroring a main repository. 

## Tutorials

With this background (or perhaps even without it), hopefully the [tutorials](https://shaunharker.github.io/GitHub-Workflows/) can be understood. And of course, there is always Google.



