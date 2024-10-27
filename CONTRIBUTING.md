# Contributing to developersIndia wiki

First off, thanks for taking the time to contribute! 🎉 Make sure you follow
below guidelines before contributing.

## Setup

### Prerequisites

You need to have the follow tools installed:

- [`mdbook`](https://github.com/rust-lang/mdBook/releases)
<!-- - [`vale`](https://vale.sh/docs/vale-cli/installation/) -->
<!-- - [`pre-commit`][18] -->

Once installed you can verify if the software are working properly or not by
invoking the following commands;

```shell
# Verify the mdbook CLI tool is installed on your system
mdbook --version
# Example output: mdbook v0.4.21
```

### Getting Started

1. Fork the repository & clone it on your local machine:

   ```shell
   git clone github.com/developersIndia/wiki
   ```

2. Run the development server to see the changes live:

   ```shell
   mdbook serve
   ```

<!-- **1. Pre-Commit Hooks**:

We've placed some bare minimum pre-commit hooks to ensure the contributions we
receive adhere to some standard coding practices. It helps us maintain an
uniform source code across the repository. So, ensure you've `pre-commit`
installed on your local machine & run the following command:

```shell
cd wiki && pre-commit install --install-hooks
```

This will install the necessary [`git` pre-commit hooks][22] which will run
each time you attempt to commit some changes. -->

<!-- **2. mdBook**:

We statically generate the [website][23] for the wiki using a CLI tool called
[`mdbook`][16]. It's built using Rust which means its fast & very useful for
building documentation websites without much overhead.

`mdbook` requires us to create Markdown files inside the `src` directory &
nested Markdown contents can exists inside sub-folders. The CLI tool is smart
enough to use those sub-folders when building the URLs. In other words, here's
what the current structure of the project is like:

```shell
.
└── ./
    └── src/
        ├── faqs/
        │   ├── how-to-start-dsa.md
        │   └── ...
        └── common-guides/
            ├── how-to-find-a-tech-job.md
            └── ...
```

Besides, the opinionated file organisation structure, `mdbook` can also be
further configured using the `book.toml` file!

Regardless, `mdbook` is highly customization & as such we recommend going
through its [official documentation](https://rust-lang.github.io/mdBook/index.html) for more information on the same. -->

## What qualifies as a "wiki"?

### FAQs

1. Questions that are repeatedly asked on our subreddit (or discord). E.g _"How
   to prepare yourself for a product job"_ or _"How to switch from service based
   to a product-based job"_.
2. FAQs are highly valuable to the community & we expect you to constantly
   update them as time changes.
3. While adding insightful posts & comments from the community, make sure you
   follow below guidelines:
   - Follow the pattern of the existing FAQs.
   - Always make sure the content is relevant to the topic. If a category for
     FAQs doesn't exist, create a proposal with the necessary posts/comments
     that can belong to it.
   - Always make sure the content is not offensive. If moderators have removed a
     post, avoid linking any content from it.
   - Avoid linking any comments that are "reactions" to the post (E.g. _congrats
     OP_, _I'm in same situation_, etc).
   - Avoid linking any comments that are "follow-up" questions to a post. Only
     link direct answers to the post.
   - Add comments that are are insightful, these usually have a lot of upvotes
     or 1-2 paragraphs or points of detailed advice.

### Community Guides

1. Long text guides which will help developersIndia (or the tech community) in
   general. You can suggest ideas by creating a proposal. A nice example would
   be _"How to improve your productivity as a developer"_. Go very niche with
   the topic.
2. Basically these are guides that are not FAQs but are still very helpful to
   the community. Avoid proposing tutorials, like how to create a HTMX app.
3. Try to make you wiki as detailed as possible. We don't expect you to know
   everything.
4. Your intention while writing a wiki should be to think of the community as a
   whole.
5. Try to avoid any personal opinions. Try to be as close as possible towards
   facts.

## Process of contributing a wiki

1. You create a
   [wiki proposal](https://github.com/developersIndia/wiki/issues/new/choose)
   with an intention to work on it.
2. Community Members review your proposal & ask/suggest any follow ups.
3. You take your time to write this wiki. We use markdown for writing and vale
   for prose linting.
4. You create a PR mentioning the issue no.
5. One (or more) community members from our team reviews your Wiki. You fix any
   issues (grammar etc)
6. Once the PR is merged. We announce the new wiki addition on our subreddit
   (and discord).
