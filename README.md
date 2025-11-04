# An Introduction to OME-Zarr for Big Bioimaging Data

This is a digital textbook that tries to explain the theory and practice behind using the [OME-Zarr data format](https://ngff.openmicroscopy.org/specifications/index.html) for big bioimaging data.
[Click here to access the book](https://ome-zarr-book.readthedocs.io/).

Feedback is very welcome, by [opening an issue](https://github.com/ome-zarr-models/ome-zarr-book/issues/new) on our GitHub issue tracker.

## Contributing

### Development

This book is built using [Jupyter Book](https://next.jupyterbook.org/).This book is built using [Jupyter Book](https://next.jupyterbook.org/).
To develop the book, it's recommended to use `uv`.
Run `uv run jupyter lab` to start Jupyter, and then navigate to the `book` directory.
Then right-click on one of the chapter's `.md` files and select "Open With" > "Jupytext Notebook".
All cells can be edited / run directly in this interface.

To build the book locally run:

```bash
cd book
jupyter book start --execute
```

This command will print a link that can be opened in a web browser to preview the book locally.

## Funding

The creation of this project was funded by the [OSCARS project](https://oscars-project.eu/), which received funding from the European Commission’s Horizon Europe Research and Innovation programme under grant agreement No. 101129751.

![OSCARS and EU logos](book/images/OSCARS-logo-EUflag.png)
