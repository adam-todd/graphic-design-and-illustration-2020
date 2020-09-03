# LJMU 2020

LJMU 2020 is built using [Jekyll](https://jekyllrb.com/).

## Developer setup

### Prerequisites / requirements

The following requirements must be met to run a development environment or to the build the static site ready for deployment.

These are not required on the web-server which will simply be serving a static set of HTML, CSS and JavaScript files.

- A **GNU/Linux, Unix, or macOS system** (Windows is not officially supported by Jekyll - but there are [workarounds](https://jekyllrb.com/docs/windows/))
- **[Ruby](https://www.ruby-lang.org/en/downloads/) version 2.2.5** or above, including all development headers. We've tested using v2.4.2.
- **[RubyGems](https://rubygems.org/pages/download)** (which you can check by running gem -v)
- **[GCC](https://gcc.gnu.org/install/)** and **[Make](https://www.gnu.org/software/make/)** (in case your system doesn’t have them installed, which you can check by running gcc -v,g++ -v and make -v in your system’s command line interface)

### Running the app in development

The application can be run locally using the following commands:

```
bundle install
jekyll serve --livereload
```

This will serve the website on `http://127.0.0.1:4000/` with live reloading enabled when code or content changes are detected.

### Deployment

To generate the static files for the website run:

```
jekyll build
```

This will generate the static files for the website in the `public` folder. This folder will need to be deployed to the server and the web server configured to serve `index.html`.
