# How to Change a Forked Git Repo Base

## Why would you need to change the fork for your repo?


If you forked the wrong version of the repo and have made changes. 

Your pull requests will not be approved to the main OnTrack or SplashKit repos. 

**_MAKE SURE YOU HAVE CLONED THE THOTH TECH VERSIONS OF THESE REPOS._**


# How do you check which repo you cloned?

**1. Navigate to your local repo's root directory in terminal**

**2. Enter command:**

	`git config --get remote.origin.url`

If you followed the onboarding instructions, it should return something like this:

	`https://github.com/[YOUR_GITHUB_USERNAME]/splashkit-core.git`

This link should point to the fork you made of the base repository on GitHub.
Now we'll check if you forked from the right repository...

**3. Navigate to your fork on GitHub via the GitHub web interface**

The URL should look something like this:

	`https://github.com/[YOUR_GITHUB_USERNAME]/splashkit-core`

**4. Check where it's forked from**

This is right under the repository name in the top left of the page.
It should look something like this:

	`forked from **thoth-tech**/splashkit-core`
And _should not_ look like this:

	`forked from **splashkit/splashkit-core`


# I forked from the wrong repo; how do I change it?

If you forked from the wrong repo and you haven’t made any commits, then the easiest option is to start over. If you have made commits you will need to change the fork location like this...

**1. Fork the correct repo (the Thoth Tech one) via the GitHub web interface**

**2. Navigate to the your local repo's root directory in terminal**

**3. Rename your origin to upstream**

	`git remote rename origin upstream`

**4. Add the new fork as the origin**

	`git remote add origin git@github.com/[GITHUB_USERNAME]/[YOUR_NEW_FORK_NAME]`

**5. Fetch from new origin**

	`git fetch origin`

**6. Set origin master**

	`git branch --set-upstream-to origin/master master`

**7. Push to fork**

	`git push origin`

... Done!

Your changes should now be going to the right place.

You can repeat the steps for checking which repo you cloned to confirm that it worked.
