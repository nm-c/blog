---
title: How to Apply a Remote Theme on GitHub Pages
description: Learn how to apply a remote theme on GitHub Pages to create a unique and customized website.
---

GitHub Pages is a free service for hosting static websites. With it, you can create your own blog, portfolio, or landing page using HTML, CSS, JavaScript, and other tools. There are a variety of themes available that you can choose from, or you can create your own custom theme.

In this guide, we'll show you how to apply a remote theme on GitHub Pages. This means that instead of using one of the pre-built themes provided by GitHub Pages, you can use a theme hosted elsewhere on GitHub.

## Step 1: Modify the _config.yml File
First things first, GitHub Pages allows you to apply a remote theme without using a Gemfile. Instead, you can set up your remote theme in the _config.yml file, which is automatically read by GitHub Pages.

Open the _config.yml file in the root directory of your project, and add the following code:

```yml
remote_theme: [GitHub Username]/[Theme Repository]
```
Replace [GitHub Username] with the GitHub username of the person who created the theme, and [Theme Repository] with the name of the theme's repository.

For example, if you wanted to use the jekyll-architect-theme, you would add the following code:

```yml
remote_theme: jekyll-architect-theme/jekyll-architect-theme
```

## Step 2: Commit and Push
Once you've modified the _config.yml file, you need to commit the changes and push them to GitHub.

ruby
Copy code
$ git add _config.yml
$ git commit -m "Add remote theme"
$ git push
That's it! Your remote theme is now applied to your GitHub Pages website.

## Conclusion
Using a remote theme on GitHub Pages is a simple way to create a unique website that stands out from the pre-built themes available. By modifying the _config.yml file, you can easily apply any remote theme hosted on GitHub. Give it a try and see what kind of website you can create!
