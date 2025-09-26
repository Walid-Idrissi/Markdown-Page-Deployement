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
``` yaml
theme : theme_name
```
To find free Jekyll themes, open [Jekyll Free Themes](https://jekyllthemes.io/free) , for this test I will be using [Hyde](https://jekyllthemes.io/theme/hyde)





