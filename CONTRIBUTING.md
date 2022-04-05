# Contributing

You can help to improve the Thoth Tech company handbook by sending pull requests
to this repository. Thank you for your interest and help!

Feel free to make a proposal, we can discuss anything and if we don't agree
we'll feel free not to merge it and we'll thank you for caring about it.
We want to create a welcoming environment for everyone who is interested in
contributing.

## Local development

### Install prerequisites

#### macOS

1. Install [Homebrew](https://brew.sh/), which is a
   package manager for macOS that allows you to easily install programs and
   tools through the Terminal. Visit their website for installation
   instructions.
1. Follow the [official instructions to install nvm](https://github.com/nvm-sh/nvm#installing-and-updating),
   a Node version manager. Then, run the following to install and use the
   repository's Node version:

   ```sh
   nvm install
   nvm use
   ```

   The required Node version should be automatically detected from the `.nvmrc`
   file. This can be confirmed by running `nvm which`.

1. Install all dependencies
   ```sh
   npm install
   ```

#### Windows (using WSL2)

1. Set up Windows Subsystem for Linux (WSL) and the Linux distribution. WSL allows Linux distributions to run on the Windows OS. Visit this [website](https://docs.microsoft.com/en-us/windows/wsl/install) for more information.

   ```powershell
   wsl --install
   ```

1. Follow instructions for [Linux](#linux)

#### Linux

1. Install curl

   ```sh
   sudo apt-get install curl
   ```

1. Follow the [official instructions to install nvm](https://github.com/nvm-sh/nvm#installing-and-updating),
   a Node version manager. Then, run the following to install and use the
   repository's Node version:

   ```sh
   nvm install
   nvm use
   ```

   The required Node version should be automatically detected from the `.nvmrc`
   file. This can be confirmed by running `nvm which`.

1. Install all dependencies
   ```sh
   npm install
   ```

### Formatting

Documentation formatting is done with `prettier`. The following command can be
run to format all Markdown files across the entire repo:

```sh
npm run format
```

## Contributing guidelines

Contributing formatting guidelines, including git workflow and commit formatting requirements can be found in our [git contribution guide](docs/processes/quality-assurance/git-contribution-guide.md).
