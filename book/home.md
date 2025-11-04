---
authors:
  - name: David Stansby
    id: dstansby
    orcid: 0000-0002-1365-1908
    github: dstansby
    corresponding: true
    email: d.stansby@ucl.ac.uk
    bluesky: "@dstansby.bsky.social"
    url: https://davidstansby.com
    affiliations:
      - id: ucl
        institution: UCL
        city: London
        ror: https://ror.org/02jx3x895

  - name: Ruaridh Gollifer
    id: ruaridhg
    orcid: 0000-0001-9319-936X
    github: ruaridhg
    affiliations:
      - id: ucl

  - name: Kimberly Meechan
    id: K-Meech
    orcid: 0000-0003-4939-4170
    github: K-Meech
    affiliations:
      - id: ucl
---

# An Introduction to OME-Zarr for Big Bioimaging Data

This book tries to explain the theory and practice behind handling large bioimaging datasets using the OME-Zarr data format.

It is written for anyone working with bioimaging data that is 'big'.
This means too big to transfer the data quickly from where it's stored to where you need it in one go.
This can include downloading it over the internet for viewing, or loading it from your hard drive into memory for analysis.

The tools and methods in this texbook are tailored to working with big imaging data.
Tackling this data adds complexity to the tools and methods, so if you have smaller data it might be easier to use other file formats and tools.
See the [Introduction to Bioimage Analysis textbook](https://bioimagebook.github.io) for other options.

## Reading this book

### Pre-requisites

This textbook assumes some familiarity with images.
The practical examples in this textbook are written in the Python programming language, but you can still read the book with out running or understanding the code.
The first two chapters give theoretical background and code is only used to explain concepts; the later chapters explain the practice of working with OME-Zarr datasets and contain code that you could copy and adapt for your own use.
The [Introduction to Bioimage Analysis textbook](https://bioimagebook.github.io) has a good primer on images in the context of both Python and Biology.

### Reading the book

Every chapter is designed to be read from start to end in a linear fashion.
Each chapter builds upon the previous ones, so they should be read in order.
It is not designed to have hands-on examples, and should complement other resources that provide interactive lessons, such as the [OME-Zarr lesson in the Bioimage Analysis Training Resources](https://neubias.github.io/training-resources/ome_zarr/index.html).
Some of the code examples provided to explain concepts might be a useful starting point for writing your own data management and analysis code.

### Running code

If you want to you can [download the Python requirements](https://raw.githubusercontent.com/ome-zarr-models/ome-zarr-book/refs/heads/main/requirements.txt) used to generate the output in this book, and use them to create a fresh Python environment.

## Contributing

This is a community resource - everyone is welcome to read and contribute to the textbook!
There are lots of different ways you can contribute:

- **Feedback**: either email David (email link above), post on our image.sc thread, or [open an issue on GitHub](https://github.com/ome-zarr-models/ome-zarr-book/issues).
- **Suggestions** for new content: same as feedback.
- **Writing** new content: please open a pull request with your suggested update. If you want to make a major change it might be best to open an issue first to discuss it briefly and check it fits in with the rest of the book.

### Roadmap

The textbook is not complete; here are chapters we would like to add:

- Add a chapter explaining image containers in OME-Zarr (Zarr groups containing more than one OME-Zarr image), including high content screening and label groups.
- Expand the "Exporting" chapter to explain how to process one resolution level, and apply that processing to many other resolution levels of a OME-Zarr image.

If you would like to write a chapter, or propose another new chapter to add to the roadmap, please get in touch!

## Acknowledgements

The creation of this book was funded by the [Handling Enormous Files from Tomographic Imaging Experiments (HEFTIE) project](https://oscars-project.eu/projects/heftie-handling-enormous-files-tomographic-imaging-experiments).
HEFTIE was funded by the [OSCARS project](https://oscars-project.eu/), which received funding from the European Commission’s Horizon Europe Research and Innovation programme under grant agreement No. 101129751.
![OSCARS and EU logos](images/OSCARS-logo-EUflag.png)
Thanks to Alessandro Felder for reviewing and providing helpful improvements and comments.
