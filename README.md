# Contributing in cryptodemonz repos

In modern-day applications, it is crucial to keep a clean workflow. It helps the development process by allowing lead developers to quickly review your commits, make optimal adjustments and merge them to production as soon as possible.

Thus, we have compiled a small but informative contributing guide that will apply to every repository. It is for our core developers, contractors and any external contributors. Any unique exception will be described in the repository-specific guide if there is any notable exception.

## Workflow

**The contribution workflow is following:**

If you have permission from lead developers to maintain the repository, you can be called a "core developer", and you will be granted rights to commit directly and create your workflow/custom contributing guidelines.

For other contributors, you SHOULD follow the given rules:

  1) **Fork the repository**
  
  If you dont know the difference between cloning and forking, please catch up with github basics, it is very important to understand what you do and why do you. 
  
  2) **Always stay updated by fetching upstream**
  
  ```
  cd <forked repo>
  git remote add upstream <original repo>
  git fetch upstream
  git pull --rebase upstream <default branch>
  ```
  
  3) **If there is an issue open, use it's id (#0000) and create new branch, for example: `chore/update-truffle-deployment-#0000`, otherwise use default branch**
  
  Branching out in custom one is very strightforward:
  ```
  git checkout -b <new branch name>
  ```
  
  4) **Commit changes and open pull request, describing the changes accordingly (see guide below)**
  
  ```
  git commit -am "feat: add new feature"
  git push <remote name> <branch name>
  ```

## How to write good commit messages

For commit messages, we strongly advise using the semantic way. It is a standard for writing commit messages in a clean and efficiently filterable way:

  - `feat` is a new feature for the user, not for the build script
  - `fix` commit related to some fix
  - `docs` update in README, CONTRIBUTING, or code documentation
  - `style` for example, change spaces to tabs
  - `refactor` modifying code without changing its logic but making it more optimised.
  - `test` adding test cases
  - `chore` updating build, deployment scripts or dependencies
  - `mixed` commit that fits in several categories
  - `none` commit, that either doesn't fit in given categories or is too small to be described
  
 Here are the several examples:
 
 `feat: add new button`
 `refactor: remove unused functions`
 `mixed: fix #0000 and add build script`
 
 *It is important to keep messages in infinitive sense, for example `feat: added new layout` is bad, instead use `feat: add new layout`. Also it's important to keep messages very short. If there is anything that you want to describe, add comment to commit afterwards*
 
## How to write good PR

Other than respecting the rules mentioned above, here are some tips and PR message templates to make our job easier:

 - Addressing <issue id, example: #0001> 
    - If you aren't addressing any open issues, add a title that describes your changes, for example: fixing the XYZ bug for better performance.

 - Why did you decide to add this feature or fix this bug? Describe your changes.

 - Reference other issues, was this mentioned before? Are you sure that PR that addresses this wasn't rejected already? 

 - Anything else you want to change, any question, or issue that you detected but can't fix.>

## Other tips that might come handy
 - Write tests. Tests are very important.
 - Never push huge commits, always keep them short, with proper semantic messages
 - If you aren't sure, ask in our discord, we might help you
 - Respect styling and modern code writing standards. All tho, this will be mentioned in each repository under CONTRIBUTING.md
 - Write docs, or NETSPEC comments. Explain your stuff, it's important that you explain your stuff.

## Easy win

If you respect our guidlines, we will make sure to respect your work as well. Make things easier for us, and we will do same. 

For any question, either open issue in this repo, or contact us in [Discord](https://discord.gg/xhsr8gwtgY) (Open a ticket, or ask how ticket system works, never spam public chat)
