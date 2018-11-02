# UltraSuite Documentation

The source for UltraSuite documentation is in this directory under `docs/`.
Our documentation uses extended Markdown, as implemented by [MkDocs](http://mkdocs.org) and is inspired by the Keras documentation.
The directory `custom/` includes some tweaks to the original [readthedocs](https://www.mkdocs.org/user-guide/styling-your-docs/) template.

## Building the documentation

- install MkDocs: `pip install mkdocs`
- `cd` to the `docs/` folder and run:
    - `mkdocs serve`    # Starts a local webserver:  [localhost:8000](localhost:8000)
    - `mkdocs build`    # Builds a static site in "site" directory

## Deploying the documentation

- instructions are available [here](https://www.mkdocs.org/user-guide/deploying-your-docs/#organization-and-user-pages).
