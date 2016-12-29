# GitHub-Workflows

**Shaun Harker 2016-12-29-1351**

I describe two workflows for collaborating using GitHub. I have prepared them for my team but they may be more generally useful so I share them here. (Note, these ideas are not new and this work is completely redundant. The value for my team is it is very specific.)

Roughly speaking, the first way is arguably the "easy but not best" way to do it, and the latter way is the "harder but better" way to do it. (Note: opinions vary.)

* [Branching Workflow:](./Branching-Workflow/GitHub-Branching-Workflow.html) (click for 10-page tutorial with pictures)
  * One repository which everyone reads and writes from
  * There is a `master` branch which is the main version
  * Every collaborator makes their own development branch, e.g. `alice-dev`, `bob-dev`, etc...
  * Collaborators pull other's work into their development branch from `master`, not directly from other development branches. All shared work must pass through `master`.
  * Collaborators share their work by submitting to `master` via a "Pull Request" (PR).
  * This workflow can be managed **without a command line** using only GUI tools.
  * It is more appropriate for smaller writing projects.


* [Forking Workflow:](./Forking-Workflow/GitHub-Forking-Workflow.html) (click for 30-page tutorial with pictures)
  * One collaborator has the "main repository" (e.g. whoever is best with `git`) and no one else has write permissions to it.
  * All other collaborators have their own forked versions of this main repository, which no one else has write permissions to.
  * The main repository's `master` branch is considered the main version of the project. Apart from that branches are managed however people choose.
  * Collaborators pull other's work from the main repositoriy's `master` branch.
  * Collaborators share their work by submitting Pull Requests to the `master` branch of the main repository.
  * This workflow requires command line interfaces to be handled.
  * It is more appropriate for coding projects, or when all team members are good with command-line `git`.
