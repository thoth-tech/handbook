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

### Installation

We use [prettier](#prettier) and [Vale](#vale) to check the documentation.

#### Install prerequisites

##### macOS

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

##### Windows (using WSL2)

1. Set up Windows Subsystem for Linux (WSL) and the Linux distribution. WSL
   allows Linux distributions to run on the Windows OS. Visit this
   [website](https://docs.microsoft.com/en-us/windows/wsl/install) for more
   information.

   ```powershell
   wsl --install
   ```

1. Follow instructions for [Linux](#linux)

##### Linux

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
