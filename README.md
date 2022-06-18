# Collab Template

> Note: It is recommended to replace this section with a description about your project.

This template aims to provide the following:

1. A simple Git workflow designed for teams.
2. Guidelines for project organization.
3. A place to consolidate project resources and documentation.

The information is broken up into different roles:

1. [Contributors]() work on code and other assets within this repo.
2. [Code Reviewers]() review pull requests and merge them.
3. [Repository Maintainers]() set up the repo and make project organization decisions.

With each role, guidelines are broken up into two sections:

1. Less strict guidelines for small or short term projects.
2. Stricter guidelines for large or long term projects.

When onboarding new members to the project, you can point them towards the respective sections and answer any additional questions they have.

## Resources

If you are ever stuck, don't hesitate to ask a teammate! In addition, here are some important links related to the project:

1. [Placeholder]() - Put your own links here!

## Workflow Overview

To put it simply, the overall workflow is to:

1. Clone the repo.
2. Create a development branch.
3. Make and commit your changes.
4. Open a pull request.
5. Switch back to `main` branch.
6. Fetch/Pull any new changes.
7. (Optional) Delete your previous local dev branch.
8. Create a new dev branch with a new name (`dev/previous-name-2`, etc).

After you have opened a pull request, a repository maintainer will review your changes and merge it into the project.

In the case of merge conflicts or any other issue, they will also work with you to resolve the issues or suggest improvements.

### Additional Workflow Tips

1. Try to keep your branches and pull requests small! Smaller branches tend to be more focused and easier to merge.
2. Always communicate with your team about what features and files you will be working on.
3. Don't let your branch get outdated. Either update your branch by merging `main` into your branch or create a pull request.

## Project Organization

> Note: You'll likely want to edit this section to better fit your project.

I (Exanite) recommend dividing your project into four different sections:

1. Project assets
2. Project code
3. Third party code
4. Prototyping

Because code typically isn't meant to be directly used by designers,
sections 1 and 2 create a separation between designers and
programmers.

Likewise, third party code typically shouldn't be modified and is thus
placed in its own folder.

Having a separate prototyping folder also creates a separation between
production ready assets and assets that are used for testing or are in
the middle of development.

### Example

With Unity, this leads to the four following folders in the Assets folder:

1. Project - Stores any project related assets that isn't code. This includes art, music, prefabs, shaders, and much more.
2. Project.Source - Stores any project related code. This is where programmers will work.
3. Plugins - Stores 3rd party assets and code (unless the asset needs to be in a specific folder).
4. Prototype - Contains folders related to each developer's ongoing work. Each developer will have their own folder where they can store anything that isn't ready to be included in the final game.

### Additional Resources

Here are some additional resources for deciding on how to organize your
project, however, note that much of this is subject to opinion and can
differ depending on the needs of your project. However, in any case,
being consistent is more important than being "correct".

https://github.com/justinwasilenko/Unity-Style-Guide
https://github.com/Allar/ue5-style-guide

## For Repository Maintainers

