# Code Reviewers

Smaller teams can work perfectly fine without code reviewers, but as
the team size grows, code reviewers work to make sure submitted code
is of a standard quality.

Code reviewers at the minimum should make sure the code works.
Non-working code will block the work of other developers and as such,
should never make it to the `main` branch.

## Workflow Overview

1. Read through the pull request.
2. Check out the pull request's branch.
3. Update the branch by merging from `main`. This can cause merge conflicts so be ready to resolve those.
4. Take a look at files that have been changed. Take a look at the [What to look for](#what-to-look-for) section.
5. Provide feedback. This can be done through
   [Github's code comment system](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request).
6. Submit your review when done.
7. If your project has automated code testing and builds, make sure those pass.
8. Finally, merge when the pull request has no remaining issues and has gained enough approvals (smaller projects can have just one code reviewer).

## What To Look For

1. Does the code work? Does it compile? Does it fulfill the intended purpose?
2. Is the change needed? What purpose does it serve?
3. Is the code easy to understand? If not, does it have comments?
4. Is there a better approach? Can readability or performance be improved? Can unnecessary code be removed?
5. Is the code consistent with the project's code style?

> Note: Be careful with performance vs readability. If performance
> isn't needed by that area of code, typically it is better to prefer
> readable code until performance is needed. Over-optimizing for
> performance can add a lot of complexity.

In addition to this, Google provides a great explanation to how code review should be conducted:
[What to look for in a code review](https://google.github.io/eng-practices/review/reviewer/looking-for.html)

> In doing a code review, you should make sure that:
> - The code is well-designed.
> - The functionality is good for the users of the code.
> - Any UI changes are sensible and look good.
> - Any parallel programming is done safely.
> - The code isn't more complex than it needs to be.
> - The developer isn't implementing things they might need in the future but don't know they need now.
> - Code has appropriate unit tests.
> - Tests are well-designed.
> - The developer used clear names for everything.
> - Comments are clear and useful, and mostly explain why instead of what.
> - Code is appropriately documented (generally in g3doc).
> - The code conforms to our style guides.

## Handling Merges

There are many, many ways of handling merges from doing it in a text
editor and having a full GUI application designed for merging.
However, here are a few tips that may help merging easier:

1. You can restart merges by Git resetting the repo.
2. Always check the final result before pushing. If it doesn't look
   right, try merging again.
3. Talk to your teammates and figure out what has been changed.
4. Rebasing can be easier than a normal merge since rebasing replays a
   single commit at a time. This allows you to resolve multiple
   smaller conflicts rather than all of them at once.

> Note: Binary files cannot be merged by Git.
> 
> In these cases, check if the program you are using has tools for
> aiding merges or if it has a way to store the file in text form
> instead.

### Unity

- Unity should serialize assets as text by default, but has
  an [option to enable it if it is not](https://docs.unity3d.com/Manual/class-EditorManager.html).

  ![Image of Unity Force Text Serialization option](/docs/collab-template/unity_force-text-serialization.png)
- For asset files, Unity has
  the [UnityYAMLMerge tool](https://docs.unity3d.com/Manual/SmartMerge.html)
  that can often automatically merge scene and other complex assets
  such as prefabs for you.

### Unreal

- Unreal can help
  you [diff blueprints](https://www.unrealengine.com/en-US/blog/diffing-blueprints)
  (but cannot directly merge them for you).