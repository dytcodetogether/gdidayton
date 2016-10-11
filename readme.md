http://gdidayton.github.io/gdidayton


to run locally:

in root folder

```
jekyll build
```
```
jekyll serve
```

Navigating the files:

The folders prefixed with the underscore (" _ ") are files that are used in the jekyll build and serve.

The layouts folder contains the template html pages for the site. Currently there is only one layout, default.html, this contains the header and footer across the pages.
_layouts
  -default.html

The scss folders contain the stylesheets used for the site, these files are compiled during the jekyll build or serve into the css/application.scss file. The files should be named according to the pages or modules they modify.
Check the css/application.scss file for order of import.
_scss
   -reset.scss
   -bourbon/bourbon
   -neat/neat
   -base.scss
   -typography.scss
   -layout.scss
   -modules.scss
   -chapters.scss
   -materials.scss
   -home-page.scss
   -about.scss
   -sponsors.scss
   -errors.scss

   
