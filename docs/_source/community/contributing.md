
# Contributor Documentation

Thank you for investing your time in contributing to the project! Any contribution you make will be reflected in the most recent version of [Argilla](https://github.com/argilla-io/argilla) 🤩.

> Please read the [Code of Conduct](https://github.com/argilla-io/argilla/blob/develop/CODE_OF_CONDUCT.md) to keep the community approachable and respectable.

If you're a new contributor, we recommend you start reading the [New Contributor Guide](#new-contributor-guide), if it's not your case, feel free to jump to the section you need.


## New Contributor Guide

If you're a new contributor, read the [README](https://github.com/argilla-io/argilla/blob/develop/README.md) to get an overview of the project. In addition, here are some resources to help you get started with open-source contributions:

* **Slack**: You are welcome to join the [Argilla Slack community](https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g), where you can keep in touch with other users, contributors and the Argilla team. In the following [section](#first-contact-in-slack), you can find more information on how to get started in Slack.
* **Git**: This is a very useful tool to keep track of the changes in your files. Using the command-line interface (CLI), you can make your contributions easily. For that, you need to have it [installed and updated](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) on your computer.
* **GitHub**: It is a platform and cloud-based service that uses git and allows developers to collaborate on projects. To contribute to Argilla, you'll need to create an account. Check the [Contributor Workflow with Git and Github](#contributor-workflow-with-git-and-github) for more info.
* **Developer Documentation**: To collaborate, you'll need to set up an efficient environment. Check the [developer documentation](/community/developer_docs.md) to know how to do it.
* **Schedule a meeting with our developer advocate**: If you have more questions, do not hesitate to contact to our developer advocate and [schedule a meeting](https://calendly.com/argilla-office-hours/30min).


## First Contact in Slack

Slack is a very useful tool for more casual conversations and to answer day-to-day questions. Click [here](https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g) to join our Slack community effortlessly.

The following screens will be displayed, choose how you wish to join and enter the code sent to you via email.

![argilla-slack](../_static/images/community/contributing/argilla-slack.png)

Once you have joined the community, you'll be added to some channels by default, but below we show you all the community channels you can join:

* **00-announcements**: 📣 Stay up-to-date on official Argilla
* **01-introductions**:  👋 Say hi! to the community Fun facts are appreciated.
* **02-support-and-questions**: 🙋‍♀️ Need help with Argilla or NLP? We are always here.
* **03-discoveries-and-news**: 📚 Looking for resources and news related to everything NLP?
* **04-contributors**: 🏗️ A channel for contributions and contributors.
* **05-beta-testing**: 🚧 For access to the latest features and help us with testing the newest features.
* **06-general**: 🐒 This channel is for... well, everything else.
* **07-events-and-job-offers**: 👔 Would you like to share info about events, job offers or meetups?

So now there is only one thing left to do, introduce yourself and talk to the community. You'll be always welcome! 🤗👋


## Contributor Workflow with Git and GitHub

If you're working with Argilla and suddenly a new idea comes to your mind or you find an issue that can be improved, it's time to actively participate and contribute to the project! The main steps will be the following:

<!-- no toc -->
1. [Report an issue](#report-an-issue)
2. [Work with a fork](#work-with-a-fork)
3. [Create a new branch](#create-a-new-branch)
4. [Make changes and push them](#make-changes-and-push-them)
5. [Create a pull request](#create-a-pull-request)
6. [Review your pull request](#review-your-pull-request)
7. [Your PR is merged!](#your-pr-is-merged)


### Report an issue

If you spot a problem, [search if an issue already exists](https://github.com/argilla-io/argilla/issues?q=is%3Aissue). You can use the `Label` filter. If that is the case, participate in the conversation. If it does not exist, create an issue by clicking on `New Issue`.

![issues-page](../_static/images/community/contributing/issues-page.PNG)

This will show various templates, choose the one that best suits your issue.

![templates-issues](../_static/images/community/contributing/templates-issues.PNG)

Below, you can see an example of the `Feature request` template. Once you choose one, you will need to fill in it following the guidelines. Try to be as clear as possible. In addition, you can assign yourself to the issue and add or choose the right labels. Finally, click on `Submit new issue`.

![issue-feature-template](../_static/images/community/contributing/issue-feature-template.PNG)


### Work with a fork

#### Fork the Argilla repository

After having reported the issue, you can start working on it. For that, you will need to create a fork of the project. To do that, click on the `Fork` button.

![fork-bar](../_static/images/community/contributing/fork-bar.PNG)

Now, fill in the information. Remember to uncheck the `Copy develop branch only` if you are going to work in or from another branch (for instance, to fix documentation the `main` branch is used). Then, click on `Create fork`.

![create-fork](../_static/images/community/contributing/create-fork.PNG)

Now, you will be redirected to your fork. You can see that you are in your fork because the name of the repository will be your `username/argilla`, and it will indicate `forked from argilla-io/argilla`.


#### Clone your forked repository

In order to make the required adjustments, clone the forked repository to your local machine. Choose the destination folder and run the following command:

```sh
git clone https://github.com/[your-github-username]/argilla.git
cd argilla
```

To keep your fork’s main/develop branch up to date with our repo, add it as an upstream remote branch. For more info, check the [documentation](/community/developer_docs.md).

```sh
git remote add upstream https://github.com/argilla-io/argilla.git
```


### Create a new branch

For each issue you're addressing, it's advisable to create a new branch. GitHub offers a straightforward method to streamline this process.

> ⚠️ Never work directly on the `main` or `develop` branch. Always create a new branch for your changes.

Navigate to your issue and on the right column, select `Create a branch`.

![create-branch-issue](../_static/images/community/contributing/create-branch.PNG)

After the new window pops up, the branch will be named after the issue, include a prefix such as feature/, bug/, or docs/ to facilitate quick recognition of the issue type. In the `Repository destination`, pick your fork ( [your-github-username]/argilla), and then select `Change branch source` to specify the source branch for creating the new one. Complete the process by clicking `Create branch`.

> 🤔 Remember that the `main` branch is only used to work with the documentation. For any other changes, use the `develop` branch.

![create-branch](../_static/images/community/contributing/create-branch-together.png)

Now, locally change to the new branch you just created.

```sh
git fetch origin
git checkout [branch-name]
```


### Make changes and push them

Make the changes you want in your local repository, and test that everything works and you are following the guidelines. Check the [documentation](/community/developer_docs.md) for more information about the development.

Once you have finished, you can check the status of your repository and synchronize with the upstreaming repo with the following command:

```sh
# Check the status of your repository
git status

# Synchronize with the upstreaming repo
git checkout [branch-name]
git rebase [default-branch]
```

If everything is right, we need to commit and push the changes to your fork. For that, run the following commands:

```sh
# Add the changes to the staging area
git add filename

# Commit the changes by writing a proper message
git commit -m "commit-message"

# Push the changes to your fork
git push origin [branch-name]
```

When pushing, you will be asked to enter your GitHub login credentials. Once the push is complete, all local commits will be on your GitHub repository.


### Create a pull request

Come back to GitHub, navigate to the original repository where you created your fork, and click on `Compare & pull request`.

![compare-and-pr](../_static/images/community/contributing/compare-pull-request.PNG)

First, click on `compare across forks` and select the right repositories and branches.

> In the base repository, keep in mind to select either `main` or `develop` based on the modifications made. In the head repository, indicate your forked repository and the branch corresponding to the issue.

![compare-across-forks](../_static/images/community/contributing/compare-across-forks.PNG)

Then, fill in the pull request template. In the title, add the feat, bug or docs prefix depending on the type of modification. A general template will be shown, please click on `Preview` and choose the corresponding pull request template. In addition, on the right side, you can select a reviewer (for instance, if you discussed the issue with a member of the Argilla team) and assign the pull request to yourself.

![pr](../_static/images/community/contributing/pull-request.PNG)

Below, we chose the feature template. Now, fill in it carefully and follow the guidelines. Remember to link the original issue. Finally, enable the checkbox to allow maintainer edits so the branch can be updated for a merge and click on `Create pull request`.

![pr-feature-template](../_static/images/community/contributing/pull-request-feature.PNG)


### Review your pull request

Once you submit your PR, a team member will review your proposal. We may ask questions, request additional information or ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request) or pull request comments.

You can apply the changes directly through the UI (check the files changed and click on the right-corner three dots, see image below) or from your fork, and then commit them to your branch. The PR will be updated automatically and the suggestions will appear as outdated.

![edit-file-from-UI](../_static/images/community/contributing/edit-file.PNG)

> If you run into any merge issues, check out this [git tutorial](https://github.com/skills/resolve-merge-conflicts) to help you resolve merge conflicts and other issues.


### Your PR is merged!

Congratulations 🎉🎊 We thank you 🤩

Once your PR is merged, your contributions will be publicly visible on the [Argilla GitHub](https://github.com/argilla-io/argilla#contributors).

Additionally, we will include your changes in the next release based on our [development branch](https://github.com/argilla-io/argilla/tree/develop).

We will probably contact you, but if you would like to send your personal information (LinkedIn, profile picture, GitHub) to [David](mailto:david@argilla.io), he can set everything up for receiving your JustDiggit bunds and a LinkedIn shoutout.


## Additional resources

Here are some helpful resources for your reference.

* [Configuring Slack](https://slack.com/help/articles/218080037-Getting-started-for-new-Slack-users), a guide to learn how to configure Slack.
* [Pro Git](https://git-scm.com/book/en/v2), a book to learn Git.
* [Git in VSCode](https://code.visualstudio.com/docs/sourcecontrol/overview), a guide to learn how to easily use Git in VSCode.
* [GitHub Skills](https://skills.github.com/), an interactive course to learn GitHub.
