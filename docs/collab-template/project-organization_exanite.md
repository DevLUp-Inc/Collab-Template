# Exanite's Project Organization

> Since I usually use Unity, this will be written based off of how I
> typically organize my projects.

I recommend dividing your project into four different sections:

1. Project assets
2. Project code
3. Third party packages
4. Prototyping

Because code typically isn't meant to be directly used by designers,
assets and code are separated out into different folders. This makes
it easy for designers to know what they can and cannot modify.

Likewise, third party packages typically shouldn't be modified and is
thus placed in its own folder. If a third party package needs to be
modified, it should be done with care since it can make updating the
package difficult.

Having a separate prototyping folder also creates a separation between
production ready assets and assets that are used for testing or are in
the middle of development. This prevents unfinished assets from
accidentally included into production builds and situations such as
using an asset and having it suddenly change or be deleted.

### Example

> You can copy-paste this into the Project Organization section of the README

This project is organized into the following sections:

1. Project - Stores any project related assets that isn't code. This includes art, music, prefabs, shaders, and much more.
2. Project.Source - Stores any project related code. This is where programmers will work.
3. Plugins - Stores 3rd party assets and code (unless the asset needs to be in a specific folder).
4. Prototype - Contains folders related to each developer's ongoing work. Each developer will have their own folder where they can store anything that isn't ready to be included in the final game.

[More Information](https://github.com/UF-GDA/CollabTemplate/docs/collab-template/project-organization_exanite.md)