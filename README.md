# Netlify CMS + HUGO Template

This is a small business template.
Fork from [netlify\-templates/one\-click\-hugo\-cms: Hugo template with Netlify CMS](https://github.com/netlify-templates/one-click-hugo-cms)

This template is a template with the minimum changes I would like to make to the site.

Differences from the original form template

* Update to the latest package as much as possible
* Style
  * Discard the modified CSS framework
  * Support for dark mode
  * Support for Sass(SCSS)

Live Demo (master): https://clever-bassi-f657ce.netlify.app/

## Getting started

Use the deploy button to get your site up and running quickly!

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/hazi/one-click-hugo-cms&stack=cms)

Once the site is set up, you will receive an email invitation, so don't forget to register your password.

## Local Development

```
$ git clone git@github.com:YOUR/SITE.git
$ cd SITE
$ yarn install
$ yarn start
```

## Directory

- `/src` : css, js, font source directory
- `/site` : Hugo source directory
- `/dist` : Distribution directory

## Layouts

The template is based on small, content-agnostic partials that can be mixed and matched. The pre-built pages showcase just a few of the possible combinations. Refer to the `site/layouts/partials` folder for all available partials.

Use Hugo’s `dict` functionality to feed content into partials and avoid repeating yourself and creating discrepancies.

## CSS

All CSS is linked from `src/css/main.scss`.
You can change the theme color with `src/css/_variables.scss`.

Framework

* [sanitize.css](https://github.com/csstools/sanitize.css)
* [tachyons](https://github.com/tachyons-css/tachyons)

Tools

* [PostCSS](https://github.com/postcss/postcss) (Look at `postcss.config.js`)
* [Dart Sass](https://github.com/sass/dart-sass)

## SVG

All SVG icons stored in `site/static/img/icons` are automatically optimized with SVGO (gulp-svgmin) and concatenated into a single SVG sprite stored as a a partial called `svg.html`. Make sure you use consistent icons in terms of viewport and art direction for optimal results. Refer to an SVG via the `<use>` tag like so:

```
<svg width="16px" height="16px" class="db">
  <use xlink:href="#SVG-ID"></use>
</svg>
```
