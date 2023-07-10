## Setting up a Website

### Project Summary

Our company 'AutoNotes' aims to build an personal knowledge base product that rivals Obsidian without the need to know Markdown syntax. Go will be help power our backend web and database servers and distributed service offerings on the cloud. However, additional investors will be needed for this year-long project. To promote our product, we have created a basic website using [HUGO](https://gohugo.io). The theme for this website is the [Hugo Winston theme](https://themes.gohugo.io/themes/hugo-winston-theme/). This theme does have a [Live Demo](https://hugo-winston.netlify.app/) which made it simple to deploy onto [Netlify](https://www.netlify.com/). All descriptions are fictional and generated using [ChatGPT](https://chat.openai.com/).

## Theme features

- Posts (Markdown)
- Basic Page (Markdown)
- SCSS (Hugo Pipelines)
- Responsive design
- 100/100 Google Lighthouse speed score
- 100/100 Google Lighthouse SEO score
- 100/100 Google Lighthouse accessibility score
- Google analytics configured in `config.toml`
- Configure GID using env variable HUGO_GOOGLE_ANALYTICS_ID, compatible with Netlify.
- Title, meta description and meta tags automatically generated for every page
- OG Meta data for Facebook and Twitter
- Semantic HTML document structure

## Installation

**1. Install Hugo**

To use this theme you will first need to have Hugo installed. Please follow the official [installation guide](https://gohugo.io/getting-started/installing/)

> ⚠️ **Note:** Check your Hugo version - **Hugo Extended** is required!

This theme uses [Hugo Pipes](https://gohugo.io/hugo-pipes/scss-sass/) to compile SCSS and minify assets which means if you are not using the Hugo extended version this theme will not work. To check your version of Hugo, run `hugo version`. Make sure you see **/extended** after the version number, for example _Hugo Static Site Generator v0.51/extended darwin/amd64 BuildDate: unknown_ You do not need to use version v0.51 specifically, it just needs to have the _/extended_ part.

**2. Import Hugo site locally**

Download or git clone this project onto local machine into folder on local machine.

```
git clone https://github.com/asaraog/msds431week3.git
cd msds431week3
cd exampleSite
hugo serve
```
Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.

# Configuration

### Config options

```toml
# config.toml
[params]
  google_analytics_id = ""
  twitter_handle = "@zerostaticio"
  showAuthorOnHomepage = true
  showAuthorOnPosts = false
  showIntroContentOnHomepage = true
  showPostsOnHomepage = true
  usePaginationOnHomepage = false
  limitPostsOnHomepage = 3 # only used if usePaginationOnHomepage is false
  sortPostsByDateOldestFirst = false
  addDot = true
  addFrame = true
  highlightColor = '#7b16ff'
  baseColor = "#ffffff"
  baseOffsetColor = "#eaeaea"
  headingColor = "#1c1b1d"
  textColor = "#4e5157"
  dotColor = "#7b16ff"
  enableGoogleFonts = true 
  googleFontsUrl = "https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap"
  fontFamilyHeading = "Poppins"
  fontFamilyParagraph = "Helvetica"
  fontFamilyMonospace = "monospace"
```

### Google Analytics

Add your google analytics ID to the `config.toml`

```toml
# config.toml
[params]
  google_analytics_id="UA-132398315-1"
```

### Plausible Analytics

Add your plausible analytics domain to the `config.toml`.
This is `data-domain` in your [tracking script code](https://plausible.io/docs/plausible-script).

```toml
# config.toml
[params]
  plausible_analytics_domain = "example.com"
```

# Deploying to Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/zerostaticthemes/hugo-winston-theme)

This theme includes a `netlify.toml` which is [configured to deploy to Netlify](https://discourse.gohugo.io/t/deploy-your-theme-to-netlify/15508) from the `exampleSite` folder. If you have installed this theme into a new Hugo site and the exampleSite folder was copied or removed, you should delete the `netlify.toml` file.

