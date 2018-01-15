# Contributing

Welcome! If you have not yet, checkout the [quickstart guide](./quickstart.md). The rest of this is for when you are starting to contribute code. The goal is to make contributing to the project as seemless as possible for _everyone_ by being on the same page. If you have any suggestions for rules, follow the [filing an issue guidelines](#step-1-file--claim-an-issue)

In all places, whether commenting, filing an issue, or writing documentation, follow [docker's documentation and style conventions](https://docs.docker.com/opensource/doc-style/)

## How to Contribute

### Step 1: File / Claim an Issue
- Give notification that you are working on an existing issue or file a new one with notification.
- Issues or comments on existing issues should be related to OpenMined.
- Issue titles should be concise yet descriptive.<br>
  **Example** Instead of `Newbie question, please help`, use `How do I set up git to ignore test files?`

- Phrasing should match the main purpose of the issue.<br>
  For example, if it is a bug report, the issue title should sound like a bug report
  **Example** `Option 'other' is missing from the dropdown` instead of a feature request `Add 'other' option to the dropdown`.

### Step 2: Branch (and maybe fork)

For the most part, we follow [git flow](http://nvie.com/posts/a-successful-git-branching-model/), with the exception of a few additional rules:

- If you have not contributed, fork and branch from there.
- Branch names have the following tags:
    - 🐛 `bug`- fixing bugs in existing code
    - 👖 `chore`- updating tooling or cleanup
    - 📚 `docs`- adding/updating docs
    - ➕ `feature` - adding new features, work on a feature
    - 🔧 `tool` - adding modules/tools, development candy


- Branch names follow the following structure:
     - `<tag>/<feature name>--<branch changes>`

        **Example** `feature/he--key-rotation-add` or `chore/webpack--update-to-2`

- `master` on all repos stay protected, branch from there


### Step 3: Do work and commit

- One commit per logical change
- Be descriptive (no `Update README.md`)
- Do not make unnecessary changes to the codebase (e.g. adding/removing newlines) or changes unrelated to the issue the pull request is meant to address (please open a separate PR!)
- [Commitizen](https://github.com/commitizen/cz-cli) is a wonderful tool that helps keep commits organized. If you are frequently contributing, we highly recommend using it.

### Step 4: Pull Request
- Open a pull request against `master` and request a review. All code must meet [code standards](#code), pass integration tests, and provide a meaningful contribution.
- Tag the issues that the pull request addresses by including a GitHub keyword in the description (e.g. `Closes #1`)
- Be respectful to the reviewer! We are all trying to improve OpenMined 📈
- Once your Pull Request has been accepted, you are officially a contributor! 🔥💥🎆🎉

### Code Acceptance guidelines

If you're contributing to PySyft and/or OpenMined Unity app, here's how you should make sure your code works correctly before creating the pull request:

1. Make sure you notified other contibutors that you're working on an issue by posting a comment on the github issue page. That'll help others to understand who's working on what, ask you questions about the issue later on, or ask for advice in if someone's working on a related issue.
2. If you're adding or changing some behavior of Syft, **you should first create a notebook example of the expected behavior.**. Specifically, go to `OpenMined/notebooks/tests/` and add an example to an appropriate notebook. The example works as an integration test and will fail at this point. That's OK.
3. Write an integration test in `OpenMined/integration/`. The test should fail at this point.
4. Update or write tests in OpenMined Unity app. Run tests via Window > Test Runner to make sure your new test fails.
5. First update the OpenMined Unity code and make sure tests from Pt 4 now work correctly.
6. Write the PySyft code and make sure integration tests work correctly.

To run integration tests, do this:

```bash
cd ./integration
pytest
```

Make sure no new failing tests appeared because of your code changes before submitting your pull request. If you see any failing tests, check if there's a related issue on Github, and ping us on Slack in #team_unity if there's no issue for a failing test.

## Code

You are writing code for people to read just as much as machines. Be purposeful! [Language specific conventions](./languages.md) supersede these rules.

### Filenames

Unless a specific language convention states otherwise, all file names should be lower case and hyphenated.
**Example** `this-is-a-name.js`

### Variable Naming

Naming is not an exact science, but following these principals will help.

-  **Booleans**: Prefix with `is`, `has`
- Prioritize **descriptive** names over brevity (avoid names like `a`, `b`, `x`, etc).


### Comments

_Your code should tell the story of what you are doing; your comments should tell the story of why you are doing it._ (Source: http://stackoverflow.com/a/142869)

- Use the following prefixes when commenting:
  - `// TODO` if there is still a meaningful task to be done
  - `// FIXME` if there is something that needs to be fixed before merging
  - `// HACK` if you know or believe there is a better implementation

- Do not repeat what the code is already telling you

## Documentation

Unless it is specific to development of a repo, put any documentation in the [Docs](https://github.com/OpenMined/Docs) repo. You are in that now!

For repository specific documentation please stick to the [Readme template](readme_template.md). All repos following this standard set of _required topics_ covered in the readme enable an aligned developer experience when browsing multiple repositories.

## Inspiration
https://github.com/oss-generic/process/blob/master/docs/FormatsAndConventions.md
https://github.com/nodejs/node/blob/master/CONTRIBUTING.md
