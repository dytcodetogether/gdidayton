# Girl Develop It Dayton
http://gdidayton.com/

## Who We Are

Girl Develop It is a nonprofit organization that exists to provide affordable and judgment-free opportunities for women interested in learning web and software development. Through in-person classes and community support, Girl Develop It helps women of diverse backgrounds achieve their technology goals and build confidence in their careers and their every day lives.

## Quick Start

This site uses the ruby gem Jekyll. If you haven't already, run:

`gem install jekyll`

To start the project, in your root folder, run:

`jekyll build && jekyll serve`

## Troubleshooting

Did running the project result in an error like: 

``` Ignoring executable-hooks-1.4.2 because its extensions are not built.  Try: gem pristine executable-hooks --version 1.4.2
Ignoring gem-wrappers-1.3.2 because its extensions are not built.  Try: gem pristine gem-wrappers --version 1.3.2
/System/Library/Frameworks/Ruby.framework/Versions/2.3/usr/lib/ruby/2.3.0/rubygems.rb:241:in `bin_path': can't find gem jekyll (>= 0.a) (Gem::GemNotFoundException)
	from /usr/local/bin/jekyll:22:in `<main>' 
  ```
  
If so you may need to install [Bundler](https://bundler.io/) to install missing gems.

Install Bundler:
`gem install bundler`


Install project specific ruby dependencies:
`bundle install`


Wrong version of Ruby?

Use Ruby Version Manager (RVM) to manage version of Ruby

If you're using rvm:

`rvm install 2.2.4`

`rvm use 2.2.4`

else if you're using rbenv:

`rbenv install 2.2.4`

`rbenv local 2.2.4`

## Contributing

The GDI Dayton website is an open source project always accepting community input. See something that could be better? [Submit an issue](https://github.com/gdidayton/gdidayton/issues) to us, or [create a pull request](https://github.com/gdidayton/gdidayton/pulls) to make changes. Visit [GitHub's guide to contributing](https://guides.github.com/activities/contributing-to-open-source/) for more tips.

See our [Contritubuting.md](https://github.com/gdidayton/gdidayton/blob/gh-pages/CONTRIBUTING.md) for details.
