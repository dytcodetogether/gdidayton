## Contributing

The GDI Dayton website is an open source project always accepting community input. See something that could be better? [Submit an issue](https://github.com/gdidayton/gdidayton/issues) to us, or [create a pull request](https://github.com/gdidayton/gdidayton/pulls) to make changes. Visit [GitHub's guide to contributing](https://guides.github.com/activities/contributing-to-open-source/) for more tips.

## Architecture

This is a [Jekyll-based](http://jekyllrb.com/) website designed to be published on the
[GitHub Pages](https://help.github.com/categories/github-pages-basics/) platform.

## Setup

### Prerequisites

#### Ruby

Since this is a Jekyll-based website, you will need [Ruby](https://www.ruby-lang.org/en/). The best way to get
Ruby is to install it via [rbenv](https://github.com/rbenv/rbenv). See the
[rbenv installation instructions](https://github.com/rbenv/rbenv#installation)
to set it up on your system.

### Building and Previewing

This site uses the ruby gem Jekyll. If you haven't already, run:

`gem install jekyll`

First, install Ruby gem dependencies:

```
bundle install
```

To start the project, in your root folder, run:

`jekyll build && jekyll serve`

A development server will start at http://localhost:4000/


### The Files Explained

At the root of this project lives the `_config.yml`, CNAME file, this `readme.md` and the html content files of gdidayton.com pages. The `_config.yml`, CNAME, and readme should be left alone, as modification could break the site.

The html pages located in the root are templates that are inserted into the `{{ content }}` tag in the `_layouts/default.html` (see below for details).

* about.html
  * shows the chapter about page content: our mission, our story, our leadership team      
* code-of-conduct.html
  * shows a copy of the GDI code-of-conduct, link to it in the footer
* index.html
  * shows the front page content: this is where the events gets edited
* materials.html
  * shows the materials page content: this is where links to GDI Dayton course content lives
* supporters.html
  * shows the supporters page content: images of our supporters (Sparkbox, Proto, Littlelines, Casamatic, AIS)


The folders prefixed with the underscore (" _ ") are files that are used in the jekyll build and serve.

The _layouts folder contains the template html pages for the site. Currently there is only one layout, default.html, this contains the header and footer across the pages.
- _layouts
  - default.html

The _scss folders contain the stylesheets used for the site, these files are compiled during the jekyll build or serve into the css/application.scss file. The files should be named according to the pages or modules they modify.
Check the css/application.scss file for order of import.
- _scss
   - reset.scss
   - bourbon/bourbon
   - neat/neat
   - base.scss
   - typography.scss
   - layout.scss
   - modules.scss
   - chapters.scss
   - materials.scss
   - home-page.scss
   - about.scss
   - sponsors.scss
   - errors.scss

The _site folder contains the compiled jekyll site. Basically do not edit these files.

The css folder contains the application.scss that is used to compile application.css. Only change this file if you have added a new file to the _scss folder.

The img folder contains the images used on the site.

The javascript folder contains some jquery and other javascript scripts for the site. Some are left over from forking the GDI national site, and do not do anything.

### Contributing content and code

1. Fork the repository (or clone it if you have commit access)
2. Create a feature branch
3. Make your changes in the feature branch
4. Commit the feature branch
5. Push the feature branch to GitHub
6. Open a pull request to merge the feature branch

### Proposing changes and reporting issues

The best way to contact us regarding this site is to [open an issue on GitHub](https://github.com/gdidayton/gdidayton/issues). Please submit a new issue if you need to:

* Report a website bug
* Propose a change to the website content

## Deploying

We make use of GitHub's continuous deployment system, which automatically
deploys branches as soon as it detects a push to the gh-pages branch.

  * Chapter "About" page content: our mission, our story, and our leadership team.    
* `code-of-conduct.html`
  * Page for the GDI Code of Conduct. Link to this page in the page footer.
* `index.html`
  * Front page content, such as upcoming events.
* `materials.html`
  * Materials page content, such as links to GDI Dayton course content.
* `supporters.html`
  * Supporters page content, including logos of our sponsors (AIS, DLM, Mile Two, Sparkbox).

Folders prefixed with an underscore (" _ ") are files used in the Jekyll build and serve.

The `_layouts` folder contains the template html pages for the site. Currently there is only one layout, `default.html`. This default layout contains the header and footer for all
* `_layouts`
*  `- default.html`

The `_scss` folder contains the stylesheets used for the site. These files are compiled during the Jekyll build or serve into the `css/application.scss` file. The files should be named according to the pages or modules they modify.
Check the `css/application.scss` file for order of import.
- `_scss`
   - `reset.scss`
   - `bourbon/bourbon`
   - `neat/neat`
   - `base.scss`
   - `typography.scss`
   - `layout.scss`
   - `modules.scss`
   - `chapters.scss`
   - `materials.scss`
   - `home-page.scss`
   - `about.scss`
   - `sponsors.scss`
   - `errors.scss`

The `_site` folder contains the compiled Jekyll site. Basically do not edit these files.

The `css` folder contains the `application.scss` that is used to compile application.css. Only change this file if you have added a new file to the `_scss` folder.

The `img` folder contains the images used on the site.

The `javascript` folder contains some jQuery and other JavaScript scripts for the site. Some are left over from forking the GDI national site, and do not do anything.

### Code Styles

#### CSS/Sass
We use [SMACSS](https://smacss.com/) (pronounced "smacks") for code organization. Keep this in mind when creating new class names or modules.

A few CSS rules to follow:

* Use full CSS format for rules. Include a semicolon after the final property, and give each property/value pair their own line.

  * DO:

  ``` css
  selector  {
    property: value;
    property: value;
  }
  ```

  * NOT:

  ``` css
  selector  { property: value; }
  ```
  ``` css
  selector  {
    property: value;
    property: value
  }
  ```

* When using a decimal, include the leading zero:
  * DO :
  ``` css
    .class {
      width: 0.75rem;
    }
  ```
  * NOT:
  ``` css
    .class {
      width: .75rem;
    }
  ```


* Use `rem` or `em` instead of `px` wherever possible; specifically for sizes over `10px`.

* Use `dashes-not-underscores` to represent spaces in class names.

* Use only lower case, except with hex values for color. When using hex values for color, establish a variable in `_variables.scss`.