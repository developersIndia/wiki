# Discovering Small GitHub Projects for Contributing to FOSS

There are more than [60k small FOSS projects](https://github.com/search?q=saved%3Asmall-foss&type=repositories&saved_searches=%5B%7B%22name%22%3A%22small-foss%22%2C%22query%22%3A%22template%3Afalse+archived%3Afalse+fork%3Afalse+stars%3A100..500+forks%3A%3E%3D3+is%3Apublic+topics%3A%3E%3D3+license%3A0bsd+license%3Amit+license%3Aapache-2.0+license%3Agpl+license%3AMPL-2.0%22%7D%5D&expanded_query=template%3Afalse+archived%3Afalse+fork%3Afalse+stars%3A100..500+forks%3A%3E%3D3+is%3Apublic+topics%3A%3E%3D3+license%3A0bsd+license%3Amit+license%3Aapache-2.0+license%3Agpl+license%3AMPL-2.0) on GitHub most likely open to contributions. Have you ever thought about contributing to them? If not, then you should. This guide is about helping the reader identify these projects on GitHub. The guide is meant to encourage both new and experienced contributors to find projects on GitHub that have a small impact and contribute to them in any way.

There are existing sites like [Up For Grabs](https://up-for-grabs.net/#/) and [First Timers Only](https://www.firsttimersonly.com/) that use "crowdsourcing" as a way to add & find projects and issues to contribute to but there's a big chance that authors of small projects may not be well represented in this list (marketing projects takes a lof of effort), or even worse you are missing out to work on some interesting hidden gems.


## What this guide covers?

- Understanding the importance of contributing to small projects.
- How to search projects on GitHub effectively.

## What it doesn't cover?

- How to contribute to FOSS, this guide is only about finding small projects & their impact on the FOSS ecosystem. There are thousands of guides on how to contribute to open-source projects on the internet, the things taught in those guides apply to projects of all sizes.
- Finding small projects on other platforms like GitLab, Self-hosted Git instances, etc.


## Why contribute to small projects?

### You can make a significant impact

- Due to less traffic (or activity) on small projects, your contributions are more likely to be noticed and appreciated.
- It's comparatively easier to get started on small projects because of less codebase and complexity, which ultimately lowers your overwhelmness to get started.

### This is the "Real" FOSS that needs your help

- Small FOSS is the real FOSS that needs your help. They are not backed by big companies and are not as popular as big projects. They are the ones that require your help the most.

### Fuck Around and Find Out

- Large FOSS projects that are maintained by a community usually have a set of docs to get started. Conversely, these small projects may not have those guides.
- This is a golden opportunity for folks trying to _**learn by doing**_. Throw yourself in this clueless, unknown codebase, and see if you find and learn new things. Sure you can do this with Big projects as well but hey, the more no. of contributors, the more no. of chances of code patterns plus with a small impact understanding small codebases will be easier and less time-consuming.


## How to find small projects on **`GitHub`**?

We now look at how to use GitHub search effectively to find small projects and in the end, create a workflow to do this regularly.

### Base Search Criteria

```
template:false archived:false fork:false stars:100..500 forks:>=3 is:public topics:>=3 license:0bsd license:mit license:apache-2.0 license:gpl license:MPL-2.0
```


### Judging the criteria to filter small projects

- **`stars:100..500`**
  - At first glance, filtering by stars may not be a good idea since they can possibly be [bought nowadays](https://dagster.io/blog/fake-stars), but it's a good starting point for us. Projects sitting in this category have some traction and are not completely unknown to the internet but they most likely lack marketing.
  - Reaching this milestone with the number of stars is a sign that the maintainer/author may be serious about the project and is willing to maintain it for the long run. Hence, open for contributions.
- **`archived:false`**
  - Avoid projects where the author has given up on the project or the maintainers no longer wish to continue the development.
- **`forks:>=3`**
  - A project with at least 3 forks is a good sign that the project is being used by others. You can make this criteria more strict by increasing the number of forks.
- **`template:false`**
  - Very few projects qualify as a template, so we exclude them.
- **`topics:>=3`**
  - An author willing to add topics to their project is a good sign that they are serious about making their project visible to the internet. [Topics](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics#about-topics) are a great way to categorize your project and make it discoverable.
- **`fork:false`**
  - Avoid duplicate copies of the same project. This works in conjugation with `forks>=3` filter, we need to only find the main repositories, not their forks.
  - This has a side effect of excluding forks that are now well maintained & supported by the community. But that doesn't matter in the long run, since the users of that niche project are most likely already aware of the fork. It's also possible that the author of the original project lists the fork in their README.


### How to apply and use the filter query?

GitHub is kind enough to provide us with a "Saved Searches" feature. You can save the filter query as a saved search and apply it whenever you want to find small projects. Let's see how to do that.

#### Step 1: Search for the filter query

Head over to [GitHub's search page](https://github.com/search) and copy-paste our filtering criteria in the search bar and hit enter.

```
template:false archived:false fork:false stars:100..500 forks:>=3 is:public topics:>=3 license:0bsd license:mit license:apache-2.0 license:gpl license:MPL-2.0
```

<center><img width="1088" alt="search github with small foss criteria" src="https://github.com/developersIndia/wiki/assets/34342551/ceac195e-08b2-4a18-b33c-0dd34c6cd227"></center>

#### Step 2: Save the search

Click the "Create save search" button to save the search. You can name the search anything you like. We recommend naming it something like "small-foss". Avoid using spaces in the name.

<center><img width="400" alt="save github search" src="https://github.com/developersIndia/wiki/assets/34342551/a345c0dc-5932-4bd6-a22b-6560fb9286e4"></center>

#### Step 3: Use the saved search

Once you have saved the search, you can use it anytime by referencing it via `saved:<search-name>` in the search bar.

<center><img width="369" alt="use saved github search" src="https://github.com/developersIndia/wiki/assets/34342551/7998f9dc-92d8-4e06-ab9d-bb1d408b5219"></center>

As visible from the above UI, you can choose to edit this search by clicking on "Manage saved searches" anytime.

#### Step 4: Customize the search

You can combine other filters with saved searches as well. For example, to find small FOSS Python projects, you can use the following filter query:

```
saved:small-foss language:python

# or combine multiple languages

saved:small-foss language:C++ language:Java 
```

<center><img width="325" alt="customize saved github search" src="https://github.com/developersIndia/wiki/assets/34342551/8461ad1d-82b4-4fa9-b672-8fded48b0a26"></center>

#### Step 5: Sort by recently updated

You can sort the search results by "Recently updated" to find the most active projects in this new filtered search. We could do this by adding `pushed>=YYYY-MM-DD` to the filter query but that would require us to update the date every time we want to use the search. Sorting by "Recently updated" is a better option.

<center><img width="237" alt="Sort by recently updated" src="https://github.com/developersIndia/wiki/assets/34342551/e3a6a8fc-36db-4c05-8b7b-398ef3cbaf14"></center>


> Note that we have solely relied on [GitHub's documentation](https://docs.github.com/en/search-github/searching-on-github/searching-for-repositories) to build this filter query. We recommend the reader to read the docs to modify the query as per their needs.

### What's missing?

- There's no way to tell if the project has a valid description or not. You can however search for a query [inside the description](https://docs.github.com/en/search-github/searching-on-github/searching-for-repositories#search-by-repository-name-description-or-contents-of-the-readme-file) to filter out projects. A missing description is a sign that the author may not be serious about the project.

### FAQs

#### What if I don't trust the projects I find?

- You can always check the project's README, CONTRIBUTING.md, and the issues to get a better understanding of the project and its maintainers.
- Look for authors on external platforms like LinkedIn, Twitter, etc, and see if they actively talking about the project.
- In rare cases its also possible that the authors set-up a blog, newsletter or a YouTube channel to talk about the project. This is an opportunity for you to understand the author's vision and the project's future.

#### What if my PRs are not getting merged?

- If your PRs are not getting merged, don't worry. You can always ask for feedback and improve your PRs.
- In the real world, not all PRs will get merged. That's not new and applies to all projects, big or small.
- Having said that, it's a good idea to move on to another project as soon as you feel you can't contribute anymore. There are plenty of projects out there that need your help.
- Lastly, if the project is not active, you can always fork it and maintain it yourself :)

#### What if there are no open issues on these small projects?

Here's your chance to do a **_lot_** of things.

- Install and run the project, find potholes in that process, open issue.
- Look for bugs in the code, open issue.
- Run a test suite if it's available, open issue if it fails.
- Add tests if they are missing, open PR.
- README looks outdated? Open PR and improve the documentation. Avoid fixing typos, they are not worth the Maintainer's time, unless of course, the project in itself is documentation.
- There's no CI/CD pipeline? Open a PR with a GitHub Actions workflow.
- The project is not following best practices? Open the issue and discuss.
- Lastly, become an **enabler** for the project. Evangelize the project on social media, write a blog post, etc.

## Recommended Reading

- [GitHub's documentation on Understanding the Code Search syntax](https://docs.github.com/en/search-github/github-code-search/understanding-github-code-search-syntax)

---
This wiki is maintained by [u/BhupeshV](https://www.reddit.com/user/BhupeshV/)
