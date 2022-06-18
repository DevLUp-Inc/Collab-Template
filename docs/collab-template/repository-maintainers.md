# Repository Maintainers

Repository maintainers have the role of setting up the repo and making
sure that it stays in a workable state.

## Repository Setup

1. First start by pressing the green 'Use this template' button as
   shown below and give your new repo a name. This will create a copy
   of this repo.

   ![Image of 'Use this template' button](/docs/collab-template/images/github_use-this-template.png)

2. Add your project either directly into the root folder of the repo
   OR as a subfolder.

3. Add a `.gitignore` file into your project folder. This tells Git to
   ignore certain files and folders in your project. This often is the
   difference between a 1 GB sized repo and a few MB sized repo.

   This website can help you generate a suitable `.gitignore` for your
   project: https://www.toptal.com/developers/gitignore

   ![Image of Gitignore.io](/docs/collab-template/images/gitignore-io.png)

4. In the repository [README](/README.md), fill
   the [Project Organization](/README.md#project-organization) section
   with how your project is organized. Resources are provided if you
   don't already have a plan.

5. Consider going into the repository settings and setting your pull request settings to be something similar to this:

   ![Image of Github repository pull request settings](/docs/collab-template/images/github_pull-request-settings.png)

   > Merge commits are the same as the typical merge done by Git.
   > They have the benefit of keeping branch history, but can become
   > unwieldy when there are a high number of branches
   >
   > Squash merging is when the entire pull request branch is combined
   > into a single commit.
   > This has the benefit of making the `main` branch's commit history
   > linear and very concise.
   >
   > Rebase merging is when each commit is recreated on top of the
   > `main` branch history, one at a time.
   > Similar to squash merging, this keeps the `main` branch history
   > linear. However, instead of each pull request generating one
   > commit, all of the pull request's commits are added to main.
   
   > 'Always suggest updating pull request branches' is disabled by
   > default, but having an updated branch helps code reviewers and
   > contributors test their changes on the latest version of the
   > repo. This avoids situations where the code works before merging,
   > but does not afterwards.
   
   ![Image of Github pull request update branch button](/docs/collab-template/images/github_pull-request-update-branch.png)

   > 'Automatically delete head branches' is disabled by default, but
   > enabling it keeps the Github repository clean and does not delete
   > the contributors' local branches. However, it can lead to
   > contributors forgetting to update their branch or to create a new
   > branch after the pull request has been submitted.

6. (Highly recommended) Read through the
   repository [README](/README.md) and the rest of the role specific
   documents.

7. (Optional) Add a license to the project (if open source).