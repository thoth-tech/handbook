# Setup Prettier and Vale for VS Code

Everyone at Thoth Tech should be using both [Prettier](https://prettier.io/), as well as
[Vale](https://marketplace.visualstudio.com/items?itemName=errata-ai.vale-server). These allow for
Pull Requests to run smoothly and allow Thoth Tech to have a consistent format, free from grammar
and spelling issues.

# Prettier

Prettier is a formatter used across Thoth Tech to make sure that all our documents are formatted
consistently. This makes sure that the print width and text wrapping are used for all documents and
code.

## Installing Prettier

To install Prettier do the following:

1. In Visual Studio code go to `Extensions` page
1. Search for `Prettier`
1. Select Install

![Prettier Install Page](images/prettier-install.png)

## Setting prettier as default formatter

1. Go to `Manager > Settings`
1. Search for `Default Formatter`
1. Under `Editor: Default Formatter` select Prettier - Code Formatter

![Prettier Install Page](images/prettier-default-formatter.png)

## Setting prettier to format on save (Optional but recommended)

1. Go to `Manager > Settings`
1. Search for `Format On Save`
1. Under `Editor: Format On Save` tick the checkbox

![Prettier Format On Save](images/prettier-on-save.png)

# Vale

Vale is a spell checking program that allows editors to see spelling and grammar mistakes. Vale is
also set to prevent long sentences so we can keep our documents succinct.

## Installing Vale

1. Open a new Command Line and run '`choco install vale`' (You must run as administrator so either
   append `sudo` for Linux or open you command line as an administrator for windows).
1. In Visual Studio code go to `Extensions` page.
1. Search for `Vale`
1. Select Install.

![Vale Install Page](images/vale-install-page.png)

See here for the [full Vale install documentation](https://vale.sh/docs/vale-cli/installation/)

## Final Steps

Finally its good to make sure that everything is setup and working correctly to do this:

1. Open a new Terminal and enter `npm install`
1. After the `npm` install finishes close down Visual Studio Code completely
1. optionally you can also do a restart

## Potential Issue fixes

1. If you face issues, go back through this guide and make sure all the settings that were changed
   have saved
1. If prettier doesn't seem to be working, try to create a file named `.prettierrc` in your current
   folder and copy the contents from the same `.prettierrc` file in main the repository

![Prettier Fix](images/prettier-fix.png)
