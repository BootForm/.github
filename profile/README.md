# Learn to put a real website on the internet

Short, free, no-fluff guides that take you from *"I have never used GitHub"* to a live site with a
**working contact form**. That last part is where most tutorials stop, because a static site has no
backend to send one to.

Every repo below marked as a template works the same way: click **Use this template**, follow the
README, and you have a URL you can send to someone. New repos land one at a time; watch the org to
hear about each one as it ships.

---

## Vanilla HTML/JS

No build step, no framework, no terminal required.

| | |
|---|---|
| **[first-website](https://github.com/BootForm/first-website)** | Your first page on the internet, in 15 minutes. Browser only, nothing to install. |
| **[one-page-site](https://github.com/BootForm/one-page-site)** | A single-page site you wouldn't be embarrassed by, on your own domain. |
| **[multi-step-form](https://github.com/BootForm/multi-step-form)** | A 5-step intake questionnaire (with a review step before it sends) that stays on one page the whole way through. |

## VitePress

More setup than the plain HTML templates (a terminal and Node.js), and more site for it: real
pages, a generated post list, tags, and RSS where a template calls for them. Two ways in.

### With Claude Code: install the skills and ask

```
/plugin marketplace add BootForm/site-skills
/plugin install vitepress@site-skills
/plugin install bootform@site-skills
```

Then start from a template and grow it, one command at a time:

```
/vitepress:portfolio-site   I'm Maya, a product designer in Portland
/vitepress:add-section      three-tier pricing and an FAQ on the home page
/vitepress:add-collection   books, with the author and year on each card
/vitepress:theme            dark green, with a serif font for headings
/vitepress:icons            icons for pool, gym and parking, and my Instagram in the header
/bootform:add-contact-form
```

Start a site with `/vitepress:marketing-site`, `/vitepress:portfolio-site`, `/vitepress:blog-site`
or `/vitepress:villa-site`. The full list is in [site-skills](https://github.com/BootForm/site-skills).

### By hand: use a template

Click **Use this template** on one of these and follow its README.

| | |
|---|---|
| **[vitepress-marketing](https://github.com/BootForm/vitepress-marketing)** | VitePress as a proper marketing site with a blog. Not a docs site wearing a hat. |
| **[vitepress-blog](https://github.com/BootForm/vitepress-blog)** | A real blog engine: generated post list, tags, RSS, authors. Everything VitePress doesn't ship by default. |
| **[vitepress-portfolio](https://github.com/BootForm/vitepress-portfolio)** | Projects, case studies, and a hire-me form that actually works. |
| **[vitepress-villa](https://github.com/BootForm/vitepress-villa)** | A villa or holiday rental site: rooms, a gallery, a local-guide journal, and a booking enquiry form. |

Then add page sections from **[site-sections](https://bootform.github.io/site-sections/)**:
heroes, features, pricing, FAQs, footers and more, written to survive VitePress's own styles.

**More frameworks land here over time** (Astro and React are next in line), each getting its own
section once there's more than one template in it.

## Common

Not templates to clone; reference material and tools that work no matter which framework (or
none) you're building with.

| | |
|---|---|
| **[form-styles](https://bootform.github.io/form-styles/)** | Live, copy-paste Tailwind styling for forms: input types, validation, error and success states, dark mode, and full sections that pair a form with a map or contact info. |
| **[contact-form-recipes](https://github.com/BootForm/contact-form-recipes)** | Copy-paste forms for Astro, Hugo, Jekyll, Eleventy, Svelte and VitePress. Vanilla JS, React, Vue and Angular are already covered in the [docs site's framework guides](https://bootform.com/docs/framework-vanilla-js). |
| **[site-sections](https://bootform.github.io/site-sections/)** | 27 copy-paste page sections (heroes, features, testimonials, pricing, FAQs, footers) with live previews at desktop and phone width, in Tailwind CSS v4. Built for VitePress, fine anywhere Tailwind runs. |
| **[site-skills](https://github.com/BootForm/site-skills)** | A Claude Code plugin marketplace: `/vitepress:...` commands that start a site from one of the templates above and grow it (sections, new kinds of content, theme, icons), and `/bootform:...` commands that make its form work, with no account needed until you claim it. |

---

## Building with an AI agent?

Every template ships an `AGENTS.md`, so Claude Code, Cursor, Copilot or whatever you use reads the
conventions instead of guessing at them. Ask for a marketing site and you get a marketing site,
not a documentation site with the words changed. If you're using Claude Code, the **site-skills** commands
above do the whole thing for you.

## While you wait

The BootForm documentation is already live and free to read, including framework guides for
[vanilla JS](https://bootform.com/docs/framework-vanilla-js),
[React](https://bootform.com/docs/framework-react),
[Vue](https://bootform.com/docs/framework-vue) and
[Angular](https://bootform.com/docs/framework-angular):

### 📖 **[bootform.com/docs](https://bootform.com/docs/)**

## Who's behind this

We make **[BootForm](https://bootform.com)**, a form backend for sites that don't have one. Helping
people past that step is our day job, which is why these guides spend real time on it.

They're free, and they stay free, whether or not you ever use it.
