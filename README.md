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

The first workflow, which I refer to as the _branching workflow_, is very simplified and can be accomplished without a command line and instead using only GUI (graphical user interface, i.e. point-and-click) tools. Despite being simplified it still gives almost all of the many benefits. It also provides a stepping stone along the learning curve. Command-line users can ignore the GUI and participate easily as well.

The second workflow, the _forking workflow_, uses more concepts and requires the command line. There is better protection against mistakes and also more flexibility. The great advantage to this kind of workflow is that it allows for a much larger group of collaborators without running risks. This is the workflow used by software develpers on GitHub in order to allow strangers to make contributions.

In both workflows the key concept is that there is a `master` branch of a repository which one pulls the current state of the project from. Contributors recommend their changes via issuing _Pull Requests_ (PRs), which the project maintainers inspect and either approve or request fixes.

See the [tutorials](https://shaunharker.github.io/GitHub-Workflows/) for more details.



