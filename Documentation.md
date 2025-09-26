---
layout: default
title: Documentation
---

## Beginning Steps
- New GitHub Repo
- `index.md`  or  `index.html` file
    - This indicates to the server ***which file to show first*** 
    - and by convention, that file is named `index` , its the **mandatory homepage**
    - so by going to `https://username.github.io/` the servers looks for `repo-root/index.html`
    - $\textcolor{red}{\textbf{There should only be one index file}}$
- The `index` file should either be placed in
    - Directly in the Root of the Repo
    - inside a folder named `/docs`
- For this test, i'll only use Markdown and **not** HTML/CSS/JS




## Enabling GitHub Pages

1. Inside of **Repo -> Settings**
2. Inside **Code and automation** -> **Pages**
3. Under **Build and Deployement**
     a. Choose Deploy From a Branch, *either main or 
     b. for The Deploy Branch, use the folder where the `index` file is located
     c. Custom Domains are Available

The Site will be published at either a personal repo page *as a personal website , or a normal page :
- **Personal Page &emsp;&emsp;&emsp;&emsp;&nbsp;&ensp;&ensp; :** a repo named `username.github.io` will be published as `https://username.github.io/`
- **Project Page** *(normal page)* **:** any other repo that's not the username or a Personal Page will be published as `https://username.github.io/repo-name/`


## Themes
It is possible to use [Jekyll Themes](https://jekyllthemes.io/) , to use one, create a `_config.yml` file **in the root of the repo** , with : 

#### If the Theme is Officially Supported By GitHub Pages 
``` yaml
theme : theme_name
```
To find free Jekyll themes, open [Jekyll Free Themes](https://jekyllthemes.io/free)
List of Supported Jekyll Themes for GitHub Pages : 
- Architect
- Cayman
- Dinky
- Hacker
- Leap day
- Merlot
- Midnight
- Minima
- Minimal
- Modernist
- Slate
- Tactile
- Time machine

>Although some of these themes seem to be supported, implementing them could be using `theme: jekyll-theme-name`

#### If the Theme is ***not*** Officially Sypported 
``` yaml
remote_theme: OWNER/REPO
```
Remote Theme requires the theme's location to be specified in the format `OWNER/REPO` , so for example to use the theme *Hyde*, a theme owned by *poole* the correct syntax would be : `remote_theme: poole/hyde`

#### For Gem Based Themes 
if a theme creator packages their theme as a **Ruby Gem** and publishes it to RubyGems, the syntax used is :
``` yaml
remote_theme: jekyll
```


#### Manual Installation with a Fork
?

--- 

## Config File

we know the `_config.yml` file was until now used for themes, but there are other things it can be used for :
