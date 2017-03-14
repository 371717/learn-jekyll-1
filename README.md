# LearnJekyll.js

JS mockup engine for learning how to use Jekyll basics.

**This is not a replacement for Jekyll** — it just mocks up some of its behaviors:

- Liquid templating works (`include` and `link` tags work).
- Markdown is rendered in `*.md` files.
- `site` and `page` variables work in templates.

## Usage

Javascript in a browser cannot walk the filesystem, hence a list of all content files needs to be mirrored as a YAML file `mock/structure.yml`, e.g.:

    - _posts:
      - 2017-03-13-welcome-to-jekyll.md
    - _includes:
      - sidebar.md
    - _layouts:
      - default.html
      - home.html
      - post.html
    - _config.yml
    - about.md
    - index.md

To view the mockup, just open `index.html` via any server software (e.g [Civetweb][cw]) pointed to the folder with Jekyll installation. Correct `baseurl` has to be set in `_config.yml` for the mockup to work. (When downloaded from [releases page](rel), it should work when placed right into the server root.)

[cw]: https://github.com/civetweb/civetweb
[rel]: https://github.com/jan-martinek/learn-jekyll/releases
