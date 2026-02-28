> [!NOTE]
> This repository once hosted the code for a shared library named [`broken-source`](https://pypi.org/project/broken-source/), alongside docker images, main website, monorepo and documentation for all projects.

As time went on, requirements changes and lessons are naturally learned - just because something has come to an end doesn't imply failure, but rather haunting on how useful it was and the legacy it leaves.

- A new repository under the same name was created to host a purely virtual workspace. This does break source install scripts, but they were going to be deprecated soon for simplicity, anyway.
- Submodules aren't as flexible as they seem, using the root repository .git for storing metadata and blobs makes them harder to move around in eventual restructuring and feel like a liability.
- Most of the code has been moved or inlined into projects that use the specific parts, or made into separate repositories (eg. [docker images](https://github.com/BrokenSource/Containers)) to be more focused and easier to maintain. Monorepos work _really well_ for when the whole acts as a single unit, an idea that diverged in my projects.
- No content seen here represents latest thoughts or practices, and certainly becomes less and less relevant as time goes on, given the constant evolution in better ways to do things.
- Content will be kept for a while for reference in porting and historical, trust reasons.

⚠️ Note that eventually (maybe in a year or two), this archived repository will be deleted along the deprecated shared library on PyPI. Nothing important will be lost, as things will adapt by then, providing a significantly better user experience and maintainability. Legacy unsupported code will not matter.
