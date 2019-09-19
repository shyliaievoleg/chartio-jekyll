---

---
# About

This Jekyll demo with Netlify CMS for basic editing content via web interface.
You can check live version here [https://chartio-jekyll.netlify.com](https://chartio-jekyll.netlify.com)


# Getting started

This project requires that [Ruby and Jekyll be installed](https://jekyllrb.com/docs/installation/).
If its your first time run `gem install jekyll bundler` to install both Jekyll and Bundler locally.

After cloning the project

- run `bundle install` to install gem dependencies

## CSS and JS and Images

The theme and JS files and images are located in the `/assets/css` and `/assets/js` and `/assets/images` folders.

## Netlify CMS Integration

The Netlify CMS edits the YAML files in `_data/*` along with the `_posts` folder for the sites News. By allowing the Netlify CMS to edit mainly the `_data` files, you are free to use complex markup on the rest of the site pages (more than markdown provides), and to pull in Netlify CMS managed content you simply tell Jekyll to output {{ site.data.home.title }} which coresponds to the `_data/home.yml` to access the Netlify CMS managed YAMl data.

Each _.html page will need a corresponding _.yml file that the Netlify CMS will edit. So you can control exactly what the client can edit.

You can have Netlify CMS save content as Markdown, and have Jekyll process it into html using the markdownify [Liquid filter](https://jekyllrb.com/docs/liquid/filters/) ex. {{ site.data.home.intro-body | markdownify }}

## Directories Explained

This is a quick overview of this projects directories, and how they are used.

- **\_data** Jekyll [Data Files](https://jekyllrb.com/docs/datafiles/) which is also what Netlify CMS will mainly edit to update site pages.
- **\_includes** [Reuseable components/partials](https://jekyllrb.com/docs/includes/) that are used across multiple pages
- **\_layouts** Default [Jekyll layouts](https://jekyllrb.com/docs/step-by-step/04-layouts/)
- **\_posts** Defautl Jekyll [Posts/News](https://jekyllrb.com/docs/posts/) articles configued to be edited by Netlify CMS
- **admin** [Netlify CMS configuration](https://www.netlifycms.org/docs/add-to-your-site/)
- **assets** SCSS/JS/media files mainly related to the Theme, processed by Gulp.js
