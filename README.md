# Budget Tech Picks ✨💸

Your go-to source for clever, affordable tech - from hidden gems to surprisingly useful gadgets.

![GitHub Repo stars](https://img.shields.io/github/stars/circuitecho/budgettechpicks-theme?style=social)
[![Powered By](https://img.shields.io/badge/powered%20by-circuitecho-9cf?logo=github)](https://github.com/circuitecho)
[![Built for Ghost](https://img.shields.io/badge/built%20for-Ghost-FF4785?logo=ghost&logoColor=white)](https://ghost.org)
[![View Theme](https://img.shields.io/badge/theme-Casper-orange)](https://github.com/TryGhost/Casper)
[![Live Site](https://img.shields.io/badge/live-site-blue)](https://budgettechpicks.com)
![GitHub top language](https://img.shields.io/github/languages/top/circuitecho/budgettechpicks-theme)
![GitHub code size](https://img.shields.io/github/languages/code-size/circuitecho/budgettechpicks-theme)
[![MIT License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

This customized version of the **Casper** theme powers the [BudgetTechPicks.com](https://budgettechpicks.com) blog:

- 💻 Focused on budget-friendly tech picks and hidden gems
- ✍️ Clean, readable layout for long-form blog content
- 🪄 Custom tweaks for easier browsing and more engaging visuals

---

# Casper

The default theme for [Ghost](http://github.com/tryghost/ghost/). This is the latest development version of Casper! If you're just looking to download the latest release, head over to the [releases](https://github.com/TryGhost/Casper/releases) page.

&nbsp;

![screenshot-desktop](https://user-images.githubusercontent.com/1418797/183329195-8e8f2ee5-a473-4694-a813-a2575491209e.png)

&nbsp;

# First time using a Ghost theme?

Ghost uses a simple templating language called [Handlebars](http://handlebarsjs.com/) for its themes.

This theme has lots of code comments to help explain what's going on just by reading the code. Once you feel comfortable with how everything works, we also have full [theme API documentation](https://ghost.org/docs/themes/) which explains every possible Handlebars helper and template.

**The main files are:**

- `default.hbs` - The parent template file, which includes your global header/footer
- `index.hbs` - The main template to generate a list of posts, usually the home page
- `post.hbs` - The template used to render individual posts
- `page.hbs` - Used for individual pages
- `tag.hbs` - Used for tag archives, eg. "all posts tagged with `news`"
- `author.hbs` - Used for author archives, eg. "all posts written by Jamie"

One neat trick is that you can also create custom one-off templates by adding the slug of a page to a template file. For example:

- `page-about.hbs` - Custom template for an `/about/` page
- `tag-news.hbs` - Custom template for `/tag/news/` archive
- `author-ali.hbs` - Custom template for `/author/ali/` archive


# Development

Casper styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# install dependencies
yarn install

# run development server
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.
- [Color Mod](https://github.com/jonathantneal/postcss-color-mod-function)


# SVG Icons

Casper uses inline SVG icons, included via Handlebars partials. You can find all icons inside `/partials/icons`. To use an icon just include the name of the relevant file, eg. To include the SVG icon in `/partials/icons/rss.hbs` - use `{{> "icons/rss"}}`.

You can add your own SVG icons in the same manner.


# Copyright & License

Copyright (c) 2013-2025 Ghost Foundation - Released under the [MIT license](LICENSE).
