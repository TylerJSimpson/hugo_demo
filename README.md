# hugo_demo

## Setup

### Installation

```bash
sudo apt-get install hugo
```

Note you will also need to install `Node.js` and `go`.

### Create site

`hugo-demo` represents the site name

`-f yml` is optional changes from default `toml` to `yml` format for settings file.

```bash
hugo new site hugo-demo-site
```

Alternatively some templates may have a setup file/process. Browse the templates and make a choice then follow their guide. 

I will be using Hugo Universal theme https://github.com/devcows/hugo-universal-theme.

For this theme I will simply git clone their repo into the themes folder that was created upon creating the `hugo-demo-site`.

```bash
cd hugo-demo-site/themes
git clone https://github.com/devcows/hugo-universal-theme
```

Add theme by updating the [config.toml](/hugo-demo-site/config.toml) with the theme name:
```bash
baseURL = ''
languageCode = 'en-us'
title = 'Demo for Hugo'
theme = 'hugo-universal-theme'
# style = "default" # options include: blue, green, marsala, pink, red, turqoise, violet
```

Start Hugo server:
```bash
hugo server
```