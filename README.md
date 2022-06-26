[![Netlify Status](https://api.netlify.com/api/v1/badges/47bcb497-a8f6-444b-9a16-a2f84ca5bf76/deploy-status)](https://app.netlify.com/sites/super-naiad-28284e/deploys)

# Portfolio and Blogs Website

A port of [Narative](https://www.narative.co/)'s beautiful Gatsby theme [Novela](https://www.narative.co/labs/novela/)

![](images/tn.png)

## Prerequisites

This starter is importing the theme as a [Hugo Module](https://gohugo.io/hugo-modules/)

- Go > 1.12
- Hugo > 0.65.0 

## Content Management System

![Forestry user interface](images/novela-forestry.png)

This starter is ready to be imported into [Forestry](https://forestry.io).

Any changes you save in the CMS will be commited back to your Git repository.

## Deploy on Netlify

Import your repository in [Netlify](https://netlify.com)

1. Create a new site in Netlify and import your repository.
2. Set the build command to: `hugo --gc --minify`
3. Set the publish directory to: `public`
4. Set `GO_VERSION` to `1.12` or above
4. Set `HUGO_VERSION` to `0.65.3` or above

That's it, now your site gets deployed automatically on `git push` or when saving documents from Forestry.

## Development

1. Install [git](https://git-scm.com/), [go](https://go.dev/doc/install) and [hugo](https://gohugo.io/getting-started/installing/) binaries.
2. Run <code>hugo server</code> in base directory of project.

## Customization

### Logo

Add to your projects layout directory your logo's SVG:
`/layouts/icons/ui/logo.html`

### Socials

In order for the Socials to be surfaced in Forestry, you should copy the theme's `config/_default/social.yaml` to your project.

### Authors

You should register authors as a taxonomy in your project's `config.yaml``

```yaml
taxonomies:
  author: authors
```

#### Creating authors

Add a similar file to your content directory and Front Matter example.

```yaml
# /content/authors/firstname-lastname/_index.md
---
title: Full Name
bio: |
  Written by You. This is where your author bio lives. Share your work, your joys and of course, your Twitter handle.
avatar: /images/dennis-brotzky.jpg
featured: true
social:
  - title: github
    url: https://github.com
  - title: twitter
    url: https://twitter.com
  - title: instagram
    url: https://instagram.com
  - title: dribbble
    url: https://dribbble.com
  - title: unsplash
    url: https://unsplash.com
---
```

#### Assigning authors to posts.

Add the name of the author to the "authors" field:

```yaml
authors:
  - Kavin Sood
```
### Newsletter call to action

This theme includes a shortcode for a newsletter callout form that you can add to any page.
It uses [formspree.io](//formspree.io/) as proxy to send the actual email. Each month, visitors can send you up to one thousand emails without incurring extra charges. Visit the Formspree site to get get going add your Formspree email to your shortcode like this:

```
{{< subscribe email="your@email.com" >}}
```


## LICENSE

MIT
