# Contributing to BootForm's repos

Thanks for helping. This guide covers every repo under [github.com/BootForm](https://github.com/BootForm) that doesn't have its own `CONTRIBUTING.md`.

## Fork it, don't "Use this template"

Most of these repos are GitHub templates, so the big green button says **Use this template**. That button is for starting your own site. It makes a brand new repo with no shared history, and GitHub can't open a pull request from it back to ours.

To contribute, **fork** the repo instead (the Fork button at the top right, or `gh repo fork BootForm/<repo> --clone`), make a branch, and open the PR from your fork.

### Already made your changes in a repo from the template?

You don't have to redo them. Fork our repo, then copy your files across:

```sh
gh repo fork BootForm/<repo> --clone
cd <repo>
git checkout -b my-change

# point at the repo you made from the template
git remote add mine https://github.com/<you>/<your-repo>.git
git fetch mine

# the two histories are unrelated, so copy files rather than merge
git checkout mine/main -- path/to/changed-file another/changed-file

git commit -m "Describe the change"
git push -u origin my-change
gh pr create --repo BootForm/<repo>
```

Leave out anything specific to your own site (your form ID, your domain, your posts).

## Before you open the PR

- **Read the repo's `AGENTS.md`.** It explains how the repo works and the mistakes it was built to avoid. It's written for AI coding agents and people alike.
- **Run the build.** For the VitePress and Node repos that's `npm install` then `npm run build`. Other repos say in their README or `AGENTS.md` how to check them.
- **Look at it at phone width (375px)**, not only on desktop, if you changed anything visible.
- **Keep the placeholder form ID.** Examples use `11111111-1111-4111-8111-111111111111`. Never commit a real form ID: whoever claims a form ID receives everything sent to it.
- **One change per PR.** Two unrelated improvements are easier to review as two PRs.

## Finding something to work on

Open issues labelled `hacktoberfest` or `good first issue` are ready to pick up; comment on one to say you're taking it. For anything bigger, open an issue first so we can agree on the approach before you spend time on it.

We aim to review PRs within two days.
