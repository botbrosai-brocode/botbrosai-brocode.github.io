# Pull Request Practices

> You love to write quality code right? Here's a list of practices to follow on how to write a great PR :smile: 

## Overview

**Pull requests** let you tell others about changes you've pushed to a remote repository. Once a pull request is sent, interested parties can review the set of changes, discuss potential modifications, and even push follow-up commits if necessary. 

<hr>

## Practices

Here's a list of pointers on how to write and discuss **pull requests**.

#### Two Approvals
* Allows the team to prevent merging a PR unless it's approved.
* Helps to spread the knowledge of codebase, encourage cross-pollination of team practices between members
* A lot easier to do than to accidentally deploy a mistake to production

#### Create Early, Update Often

* New task/feature = open up a PR as early as possible
* Helps others to see how your work is progressing. It also offers hints to junior developers.
* Serves as your start and save point during a project

#### Inform them of what you're trying to do

* Use the description box, use its purpose
* Gives the team the idea of what you're trying to do
* Answers your own and the team's questions. It leaves a trail that you can go back in time and see
why you implemented something a certain way and roughly the route you took

#### Commit Small, Review Faster

* One of the top ways to speed up the team's review time
* They are so small that it's so easy to understand the context and the reason behind the PR
* Breaking down the problem into tiny multiple parts is better than spending a bit more time
researching for the whole one
* Try and find a natural "break point" of modular code and split it into two, or even three PRs
and make that clear in your comments and descriptions

#### Write useful descriptions and titles

* Add issue/ticket numbers to commit/PR titles
* Give a brief description to your commit/PR
* Include pointers/details in bullet (unordered list) form

#### Discuss

* Use the comment section for discussion
* Note that the comment section should not be used to explain code
* Helps the reviewer to navigate the pull request

#### Make it visual

* Add some screenshots for your front-end changes
* You can also add GIFs of the interactions

<hr>

## BotBros Pull Request Template

```markdown
## Summary

Include a summary about the feature you're requesting to merge.

## Branch, Route and Directory

**Branch:** *feature/SP-001-SS*  

**Routes: (Temporarily)**  

* List your routes and functions like the example below
* _/api/v1/positions_ - `GET` - index()

**Directories**:  

* Same with routes, list the directories affected in _italics_

## Key Tasks/Features of the Branch

- [x] List your key tasks as to do list within the pull request

## Note to Reviewers / Testers

* Put pointers in unlisted bullet format
```

## Interested in writing the perfect pull request? Learn more!

* [Written Unwritten Guide for Pull Requests](https://www.atlassian.com/blog/git/written-unwritten-guide-pull-requests)
