---

---
# About

This Chartio theme Jekyll demo site with Forestry CMS for basic editing content via web interface.
You can check live version here [https://chartio-jekyll.netlify.com](https://chartio-jekyll.netlify.com)


# Getting started

This project requires that [Ruby and Jekyll be installed](https://jekyllrb.com/docs/installation/).

Clone repository:

- HTTP `git clone https://github.com/shyliaievoleg/chartio-jekyll.git .` or
- SSH `git clone git@github.com:shyliaievoleg/chartio-jekyll.git .` into your project folder.

If its your first time run `gem install jekyll bundler` to install both Jekyll and Bundler locally.

After cloning the project

- run `bundle install` to install gem dependencies
- run `jekyll serve` to start dev server on http://localhost:4000/

## CSS and JS and Images

The theme and JS files and images are located in the `/assets/css` and `/assets/js` and `/assets/images` folders.

## Forestry CMS Integration

[Forestry.io](https://forestry.io) is a Git-backed CMS (content management system) for websites and web products built using static site generators. Forestry bridges the gap between developers and their teams, by making development fun and easy, while providing powerful content management for their teams.
To add your repository to forestry check this [page](https://forestry.io/docs/quickstart/setup-site/)

After adding your repository to Forestry you can create and edit content via CMS.

## Directories Explained

This is a quick overview of this projects directories, and how they are used.

- **\_data** Jekyll [Data Files](https://jekyllrb.com/docs/datafiles/) which is also what Netlify CMS will mainly edit to update site pages.
- **\_includes** [Reuseable components/partials](https://jekyllrb.com/docs/includes/) that are used across multiple pages
- **\_layouts** Default [Jekyll layouts](https://jekyllrb.com/docs/step-by-step/04-layouts/)
- **\_posts** Defautl Jekyll [Posts/News](https://jekyllrb.com/docs/posts/) articles configued to be edited by Netlify CMS
- **.forestry** [Forestry CMS configuration](https://forestry.io/docs/quickstart/setup-site/)
