# Contributing Guidelines

Thanks for your interest in contributing to `packit-service-centosmsg`.

The following is a set of guidelines for contributing to `packit-service-centosmsg`.
Use your best judgement, and feel free to propose changes to this document in a pull request.

By contributing to this project you agree to the Developer Certificate of Origin (DCO). This document is a simple statement that you, as a contributor, have the legal right to submit the contribution. See the [DCO](DCO) file for details.

## Reporting Bugs

Before creating a bug report, please check a [list of known issues](https://github.com/packit-service/packit-service-centosmsg/issues) to see
if the problem has already been reported (or fixed in a master branch).

If you're unable to find an open issue addressing the problem, [open a new one](https://github.com/packit-service/packit-service-centosmsg/issues/new).
Be sure to include a **descriptive title and a clear description**.

If possible, add a **code sample** or an **executable test case** demonstrating the expected behavior that is not occurring.

**Note:** If you find a **Closed** issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.
You can also comment on the closed issue to indicate that upstream should provide a new release with a fix.

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues.
When you are creating an enhancement issue, **use a clear and descriptive title** and **provide a clear description of the suggested enhancement** in as many details as possible.

## Guidelines for Developers

If you would like to contribute code to the `packit-service-centosmsg` project, this section is for you!

### Is this your first contribution?

Please take a few minutes to read GitHub's guide on [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/).
It's a quick read, and it's a great way to introduce yourself to how things work behind the scenes in open-source projects.

### Dependencies

If you are introducing a new dependency, please make sure it's added to:

- [setup.cfg](setup.cfg)

### How to contribute code to packit

1. Create a fork of the `packit-service-centosmsg` repository.
2. Create a new branch just for the bug/feature you are working on.
3. Once you have completed your work, create a Pull Request, ensuring that it meets the requirements listed below.

### Requirements for Pull Requests

- Please create Pull Requests against the `master` branch.
- Please make sure that your code complies with [PEP8](https://www.python.org/dev/peps/pep-0008/).
- One line should not contain more than 100 characters.
- Make sure that new code is covered by a test case (new or existing one).
- We don't like [spaghetti code](https://en.wikipedia.org/wiki/Spaghetti_code).
- The tests have to pass.

### Checkers/linters/formatters & pre-commit

To make sure our code is compliant with the above requirements, we use:

- [black code formatter](https://github.com/ambv/black)
- [Flake8 code linter](http://flake8.pycqa.org)
- [mypy static type checker](http://mypy-lang.org)

There's a [pre-commit](https://pre-commit.com) config file in [.pre-commit-config.yaml](.pre-commit-config.yaml).
To [utilize pre-commit](https://pre-commit.com/#usage), install pre-commit with `pip3 install pre-commit` and then either

- `pre-commit install` - to install pre-commit into your [git hooks](https://githooks.com). pre-commit will from now on run all the checkers/linters/formatters on every commit. If you later want to commit without running it, just run `git commit` with `-n/--no-verify`.
- Or if you want to manually run all the checkers/linters/formatters, run `pre-commit run --all-files`.

#### Changelog

When you are contributing to changelog, please follow these suggestions:

- The changelog is meant to be read by everyone. Imagine that an average user
  will read it and should understand the changes.
- Every line should be a complete sentence. Either tell what is the change that the tool is doing or describe it precisely:
  - Bad: `Use search method in label regex`
  - Good: `Packit now uses search method when...`
- And finally, with the changelogs we are essentially selling our projects:
  think about a situation that you met someone at a conference and you are
  trying to convince the person to use the project and that the changelog
  should help with that.

Thank you for your interest!
packit team.
