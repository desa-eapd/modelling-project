# Jekyll Advance Pro Theme

Jekyll Advance is a premium, multi-purpose Jekyll theme. It has 5 content-types for archetypical SMB and marketing websites. A modern semi-flat visual design with customisable hero images and full-width sections.

[Live Demo](https://jekyll-advance.netlify.app/) |
[Live Docs](https://www.zerostatic.io/docs/jekyll-advance/)

![Jekyll Advance Theme screenshot](https://www.zerostatic.io/theme/jekyll-advance/jekyll-advance-screenshot.png)

## Installing Jekyll

Make sure you have Ruby & Jekyll installed - For a step-by-step guide, read Jekyll docs [installation](https://jekyllrb.com/docs/installation/)

## Install Theme

Extract the theme .zip file to your local computer. Navigate to the project root (it contains the README.md)

Run `bundle install` to install gems.

Then run `jekyll serve` or `bundle exec jekyll serve` to start the Jekyll server.

To build the Jekyll site run `bundle exec jekyll build`

## Deploy

### Netlify

This theme comes with a working `netlify.toml` which will pre-configure your Netlify deployment for Jekyll. The Netlify docs have a great guide to [creating a site with Netlify](https://docs.netlify.com/site-deploys/create-deploys/).

> 💡 If you experience bundle install issues during the Netlify deployment, deleting the Gemfile.lock can sometimes help

### GitHub Pages

This theme is tested to work on Github Pages. Jekyll has a [guide to deploying on Github pages](https://jekyllrb.com/docs/github-pages/).

If you are creating a GitHub Pages "Project site" then your site will be in a sub-folder with a url like `http://username.github.io/repository`. You will need to update the `baseurl` and `url` in the `_config.yml` for the asset paths to work correctly.

## Credits

This theme uses open-source libraries and assets.

### Font Awesome 5 Free

- **Project:** https://fontawesome.com/
- **License:** https://fontawesome.com/license/free

### Demo content Images by Unsplash

- **Unsplash** https://unsplash.com/
- **License** https://unsplash.com/license
