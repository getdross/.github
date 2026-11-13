# Yosr Dross

Yosr Dross is a developer disk cleaner for macOS. The command is `dross`.

`dross` finds build artifacts such as `node_modules`, `target`, `.venv`, JVM (`target` with `pom.xml`, `build`, `.gradle`) and .NET (`bin`, `obj`), shows how much space they use, and moves them to the Trash. It also sizes macOS developer caches including `maven`, `gradle`, and `nuget`, and the disk used by Docker Desktop, OrbStack, Colima, and Podman. Container leftovers (dangling images, dangling build cache, stopped containers) are pruned only through each runtime's own CLI, after you pick them; dross never starts a daemon or touches a VM disk. Permanent deletion is a separate, explicit step.

v0.4.1 runs on Apple Silicon and Intel. The source is not published in this organization.

## Install

```sh
brew tap getdross/tap
brew trust getdross/tap
brew install dross
"$(brew --prefix)/bin/dross" --version
```

`brew trust` is required once on Homebrew 7. No GitHub login is required.

Website: <https://dross.yosr.ai>

Releases and archives: <https://github.com/getdross/dross>

License: [Yosr Dross License](https://dross.yosr.ai/trust/). Free to use; the source is private.

Bug reports: email (see the site).
