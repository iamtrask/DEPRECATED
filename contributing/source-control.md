## Branching

- Master stays protected, pull requests to master only.


- Branch names have the following tags:
    - 🐛 `bug`- fixing bugs in existing code
    - 👖 `chore`- updating tooling or cleanup
    - 📚 `docs`- adding/updating docs
    - ➕ `feature` - adding new features, work on a feature
    - 🔧 `tool` - adding modules/tools, development candy


- Branch names follow the following structure:
     - `<tag>/<feature name>--<branch changes>`

        i.e: `feature/training--restarting` or `chore/webpack--update-to-2`

## Commits

- One logical change per commit
- [Commitizen](https://github.com/commitizen/cz-cli) is a wonderful tool that helps keep commits organized. If you are frequently contributing, we highly recommend, but do not require, using it. 
