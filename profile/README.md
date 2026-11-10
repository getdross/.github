# dross

Developer disk cleaner for macOS.

`dross` finds build artifacts such as `node_modules`, `target`, `.venv`, JVM (`target` with `pom.xml`, `build`, `.gradle`) and .NET (`bin`, `obj`), shows how much space they use, and moves them to the Trash. It also sizes macOS developer caches including `maven`, `gradle`, and `nuget`. Permanent deletion is a separate, explicit step.

v0.3.2 runs on Apple Silicon and Intel. The source is not published in this organization.

## Install

```sh
brew tap getdross/tap
brew trust getdross/tap
brew install dross
"$(brew --prefix)/bin/dross" --version
```

`brew trust` is required once on Homebrew 7. No GitHub login is required.

Releases and archives: <https://github.com/getdross/dross>
