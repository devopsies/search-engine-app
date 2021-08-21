# DevSecOps Workshops: Github & Github Actions

This is a brief introduction to Github Actions, followed by a workshop. For the workshop material, visit <a href="https://github.com/mdnfiras/devsecops-github-actions" target="_blank">github.com/mdnfiras/devsecops-github-actions</a>. For a complete documentation, visit <a href="https://docs.github.com/en/actions" target="_blank">docs.github.com/en/actions</a>.

## What is Github?

Github is a provider of Internet hosting for software development and version control using Git. It offers the distributed version control and source code management functionality of Git, plus its own features.

## What is Github Actions?

GitHub Actions connects all of your tools to automate every step of your development workflow. In summary, Github Actions is a CI/CD tool, hosted on Github (no installation required, as opposed to Jenkins).

## Start using Github & Github Actions

In this workshop, we're going to pretend to we're building a product in C++: our awesome search engine. First, ask to be added as a collaborator in this repo. Then clone the repo, create and switch to a new development branch `develop-your_name` and push it. When solving any of the following issues, start from your development branch, create and switch to a new branch `optimizing search` or `optimizing pipeline` depending on the issue you're working on, then trigger a pull request (PR). The workflow we described here is a simple scenario from the famous Git workflow. Refer to <a href="https://www.atlassian.com/git/tutorials/comparing-workflows" target="_blank">www.atlassian.com/git/tutorials/comparing-workflows</a> for more information.

### First issue

You're the developer. The product you're developing (the search engine) currently do not satisfy the requirements as it becomes very slow with a large amount of input. Refer to the issue at <a href="https://github.com/mdnfiras/devsecops-github-actions/issues/1" target="_blank">github.com/mdnfiras/devsecops-github-actions/issues/1</a> for more details. If you have any question regarding this task, you can leave a comment in that same issue.

### Second issue

You're a DevOps engineer. The CI pipeline you've set up is slow. refer to the issue at <a href="https://github.com/mdnfiras/devsecops-github-actions/issues/3" target="_blank">github.com/mdnfiras/devsecops-github-actions/issues/3</a> for more details. If you have any question regarding this task, you can leave a comment in that same issue.
