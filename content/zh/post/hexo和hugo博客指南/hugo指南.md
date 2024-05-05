---
title: hugo指南
date: '2023-10-04'
summary: hugo使用
---

[💻 Edit your Hugo site locally | Hugo Blox Docs](https://docs.hugoblox.com/getting-started/install-hugo/)

## View your site

View your site by running the following command:

Terminal window

```
hugo server -D
```

Hugo then provides you with a link (e.g. `http://localhost:1313/`) to open in your web browser.

For help troubleshooting common Hugo errors, check out the [Troubleshooting guide](https://docs.hugoblox.com/reference/troubleshooting/).

## Edit your content in a Markdown Editor

Check out the Write Content section of the docs. We recommend writing content with [Visual Studio Code](https://docs.hugoblox.com/getting-started/cms/visual-studio-code/), either using the online version (GitHub Codespaces) or installing the VSCode software on your computer.

[Follow the step-by-step guide to edit your new site](https://docs.hugoblox.com/tutorial/resume/step-2/).

## Edit offline

When you first run `hugo server` to preview your site, Hugo will download and cache Hugo Blox Builder on your machine.

If you prefer a more reliable and permanent place to store your site’s dependencies, you can do so with the `hugo mod vendor` command.

After running Hugo’s _vendor_ command, Hugo will load your site’s dependencies from a `_vendor` folder within your site rather than using the internet or its (hidden) cache folder.

You may notice that Hugo’s `_vendor` folder is similar to the `node_modules` folder for Javascript-based site generators, albeit storing Go modules rather than Javascript packages.

## Deploy

Once you have made changes to your site, learn how to [deploy to your preferred provider](https://docs.hugoblox.com/reference/deployment/).

**Remember to set your `baseURL` (website URL) in `config/_default/hugo.yaml` before deploying your site.**