# Assessment: LIA

For this course's Learning Integration Assessment (LIA), you will use
Django to build an online shop. The project will be carried out in teams
of two, and is divided into six "milestones", each graded separately.
You will find the requirements for each milestone in the accompanying
files.

## Pull request workflow

To make collaboration smoother and encourage code review, you will share
your code with your teammate using GitHub's pull request workflow. Here
are the steps to follow once you have cloned the repository:

1. Make sure your local main branch is up to date with the remote main
   branch by running `git pull`.

2. From your local main branch, create a local feature branch with
   `git checkout -b <branch-name>`, where `<branch-name>` corresponds to
   the name of the feature you will implement.

3. Commit your changes with `git add <path>` and `git commit` (many
   times if necessary).

4. Once your code is ready, push your commits to GitHub with
   `git push -u origin <branch-name>`.

5. Using GitHub's web interface, create a pull request (Pull requests →
   New pull request → feature branch's name → Create pull request).

6. Let your teammate review your pull request. If necessary, make
   changes to your pull request by pushing new commits (repeat step #2
   and #3).

7. Let your teammate rebase and merge your pull request (Pull requests →
   pull request's name → Rebase and merge). If your pull request is
   out-of-date with main, GitHub will not let you merge it. In that
   case:

   1. Back in your terminal, switch to your local main branch with
      `git checkout main`.

   2. Sync your local main branch with the remote main branch using
      `git pull`.

   3. Switch back to your local feature branch with
      `git checkout <branch-name>`.

   4. Incorporate the latest changes from the main branch into your
      local feature branch with `git rebase main`.

   5. Fix merge conflicts, if any.

   6. Update your remote feature branch with `git push --force`.

8. Delete the remote feature branch (Code → main → view all branches →
   trash icon).

9. Back in your terminal, switch to your local main branch with
   `git checkout main`.

10. Sync your local main branch with the remote main branch using
    `git pull`.

11. Delete your local feature branch with `git branch -D <branch-name>`.

12. Repeat for every feature.

## Assessment criteria

- Program design
  - requirements are met
  - program flow is decomposed into manageable, logical pieces
  - data structures are appropriate
  - common code is unified, not duplicated
  - appropriate algorithms are used, and coded cleanly
  - interfaces are used correctly
  - code is lint-free (see `uv run ruff check`)
  - code is well-tested
  - project is well-structured
  - markup is semantic
  - no global variables

- Readability
  - constants are used instead of hard-coded values
  - complex or meaningful expressions are named
  - naming is consistent and descriptive
  - inline comments are used to explain reasoning
  - code is formatted (see `uv run ruff format`)

- Version control
  - commits contain related changes
  - messages are consistent and informative
  - changes are merged using pull requests

- Teamwork
  - workload is divided evenly (styling will not be assessed and
    therefore doesn't count toward your workload)
  - comments on pull requests are useful
  - peer assessment
