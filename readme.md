# Girl Develop It Dayton
http://gdidayton.com/

## Who We Are

Girl Develop It is a nonprofit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.

## Quick Start

`gem install jekyll`

To start the project, in your root folder, run:

`jekyll build && jekyll serve`

## Contributing

The GDI Dayton website is an open source project always accepting community input. See something that could be better? [Submit an issue](https://github.com/gdidayton/gdidayton/issues) to us, or [create a pull request](https://github.com/gdidayton/gdidayton/pulls) to make changes. Visit [GitHub's guide to contributing](https://guides.github.com/activities/contributing-to-open-source/) for more tips.

### The Files Explained

At the root of this project lives the _config.yml, CNAME file, this readme.md and the html content files of gdidayton.com pages. The _config.yml, CNAME, and readme should be left alone, as modification could break the site.

The html pages located in the root are templates that are inserted into the {{ content }} tag in the _layouts/default.html (see below for details).

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
=======
>>>>>>> 354dfcff6608b44cdd6d7bcb75d4e8d9a4aa961d
