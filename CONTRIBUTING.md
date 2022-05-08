# Contributing

You can help to improve the Thoth Tech company handbook by sending pull requests
to this repository. Thank you for your interest and help!

Feel free to make a proposal, we can discuss anything and if we don't agree
we'll feel free not to merge it and we'll thank you for caring about it. We want
to create a welcoming environment for everyone who is interested in
contributing.

## Documentation testing

We treat documentation like code. Therefore, we use processes similar to those
used for code to maintain standards and quality of documentation.

We have tests:

- To lint the words and structure of the documentation.

### Run tests locally

You can run these tests on your local computer. This has the advantage of
speeding up the feedback loop. You can know of any problems with the changes in
your branch without waiting for a CI pipeline to run.

To run the tests locally, it's important to:

- [Install the tools](#installation)
- Run [linters](#lint-checks) the same way they are run in CI pipelines. It's
  important to use same configuration we use in CI pipelines, which can be
  different than the default configuration of the tool.

### Local linters

To help adhere to the
[documentation style guidelines](/docs/documetation/writing-style-guide.md), and
improve the content added to documentation,
[install documentation linters](#install-linters) and
[integrate them with your code editor](#configure-editors).

At Thoth Tech, we mostly use:

- [Prettier](#prettier)
- [Vale](#vale)

#### Prettier

[Prettier](https://prettier.io/) checks that Markdown syntax follows the
[CommonMark](https://commonmark.org/) specifications.

#### Vale

[Vale](https://docs.errata.ai/vale/about/) is a grammar, style, and word usage
linter for the English language. Vale's configuration is stored in the
[`.vale.ini`](https://github.com/thoth-tech/handbook/blob/main/.vale.ini) file
located in the root directory.

Vale supports creating [custom tests](https://docs.errata.ai/vale/styles) that
extend any of several types of checks, which we store in the `.vale/thothtech/`
directory in the documentation directory.

##### Vale result types

Vale returns three types of results:

- **Error** - For words or phrases with ambiguous meanings.
- **Warning** - For writing style preferences.
- **Suggestion** - For basic writing tenets and best practices.

##### Vale readability score

In
[`ReadingLevel.yml`](https://github.com/thoth-tech/handbook/blob/main/docs/.vale/thothtech/ReadingLevel.yml),
we have implemented
[the Flesch-Kincaid grade level test](https://readable.com/readability/flesch-reading-ease-flesch-kincaid-grade-level/)
to determine the readability of our documentation.

As a general guideline, the lower the score, the more readable the
documentation. For example, a page that scores `12` before a set of changes, and
`9` after, indicates an iterative improvement to readability. The score is not
an exact science, but is meant to help indicate the general complexity level of
the page.

The readability score is calculated based on the number of words per sentence,
and the number of syllables per word. For more information, see
[the Vale documentation](https://docs.errata.ai/vale/styles#metric).

#### Installation

##### Install prerequisites

###### macOS

1. Install [Homebrew](https://brew.sh/), which is a package manager for macOS
   that allows you to easily install programs and tools through the Terminal.
   Visit their website for installation instructions.
1. Follow the
   [official instructions to install nvm](https://github.com/nvm-sh/nvm#installing-and-updating),
   a Node version manager. Then, run the following to install and use the
   repository's Node version:

   ```shell
   nvm install
   nvm use
   ```

   The required Node version should be automatically detected from the `.nvmrc`
   file. This can be confirmed by running `nvm which`.

1. Install all dependencies

   ```shell
   npm install
   ```

###### Windows (using WSL2)

1. Set up Windows Subsystem for Linux (WSL) and the Linux distribution. WSL
   allows Linux distributions to run on the Windows OS. Visit this
   [website](https://docs.microsoft.com/en-us/windows/wsl/install) for more
   information.

   ```powershell
   wsl --install
   ```

1. Follow instructions for [Linux](#linux)

###### Linux

1. Install curl

   ```shell
   sudo apt-get install curl
   ```

1. Follow the
   [official instructions to install nvm](https://github.com/nvm-sh/nvm#installing-and-updating),
   a Node version manager. Then, run the following to install and use the
   repository's Node version:

   ```shell
   nvm install
   nvm use
   ```

   The required Node version should be automatically detected from the `.nvmrc`
   file. This can be confirmed by running `nvm which`.

#### Install linters

1. Install `prettier`:

   ```shell
   npm install
   ```

1. Install [`vale`](https://github.com/errata-ai/vale/releases). To install for:

   - macOS using `brew`, run: `brew install vale`.
   - Linux, use your distribution's package manager or a
     [released binary](https://github.com/errata-ai/vale/releases).

These tools can be [integrated with your code editor](#configure-editors).

### Configure editors

Using linters in your editor is more convenient than having to run the commands
from the command line.

To configure `prettier` in your editor, install one of the following as
appropriate:

- Visual Studio Code
  [`esbenp.prettier-vscode` extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode).

To configure Vale in your editor, install one of the following as appropriate:

- Visual Studio Code
  [`errata-ai.vale-server` extension](https://marketplace.visualstudio.com/items?itemName=errata-ai.vale-server).

### Lint checks

The following commands can be run to format all Markdown files across the entire
repository:

```shell
# Format markdown style (fixing markdown style issues)
npm run format

# Lint markdown style and prose (reporting issues)
npm run lint

# Lint markdown style only
npm run format:check

# Lint prose only
npm run prose:check
```

## Contributing guidelines

Contributing formatting guidelines, including git workflow and commit formatting
requirements can be found in our
[git contribution guide](docs/processes/quality-assurance/git-contribution-guide.md).
