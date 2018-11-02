# UltraSuite Documentation

The source for UltraSuite documentation is in this directory under `docs/`. 
Our documentation uses extended Markdown, as implemented by [MkDocs](http://mkdocs.org) and is similar to Keras.

## Building the documentation

- install MkDocs: `pip install mkdocs`
- `cd` to the `docs/` folder and run:
    - `mkdocs serve`    # Starts a local webserver:  [localhost:8000](localhost:8000)
    - `mkdocs build`    # Builds a static site in "site" directory
