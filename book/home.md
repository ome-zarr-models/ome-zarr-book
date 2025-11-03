# Handling Enormous Files from 3D Imaging Experiments

This book tries to explain the theory and practice behind handling large bioimaging datasets using the OME-Zarr data format.

It is written for anyone working with bioimaging data that is 'big'.
This means too big to transfer the data quickly from where it's stored to where you need it in one go.
This can include downloading it over the internet for viewing, or loading it from your hard drive into memory for analysis.

The tools and methods in this texbook are tailored to working with big imaging data.
Tackling this data adds complexity to the tools and methods, so if you have smaller data it might be easier tot you use other file formats and tools.
See the [Introduction to Bioimage Analysis textbook](https://bioimagebook.github.io) for other options.

## Using this book

### Pre-requisites

This textbook assumes some familiarity with images.
The practical examples in this textbook are written in the Python programming language.
The first two chapters give theoretical background and code is only used to explain concepts
The later chapters explain the practice of working with OME-Zarr datasets and contain code that you could copy and adapt for your own use.
The [Introduction to Bioimage Analysis textbook](https://bioimagebook.github.io) has a good primer on images in the context of both Python and Biology.

### Reading the book

Every chapter is designed to be read from start to end in a linear fashion.
Each chapter builds upon the previous ones, so they should be read in order.
It is not designed to have hands-on examples, and should complement other resources that provide interactive lessons, such as the [OME-Zarr lesson in the Bioimage Analysis Training Resources](https://neubias.github.io/training-resources/ome_zarr/index.html).
Some of the code examples provided to explain concepts might be a useful starting point for writing your own data management and analysis code.

### Running code

If you want to you can [download the Python requirements](https://raw.githubusercontent.com/ome-zarr-models/ome-zarr-book/refs/heads/main/requirements.txt) used to generate the output in this book, and use them to create a fresh Python environment.

## Acknowledgements

The creation of this book was funded by the [Handling Enormous Files from Tomographic Imaging Experiments (HEFTIE) project](https://oscars-project.eu/projects/heftie-handling-enormous-files-tomographic-imaging-experiments).
HEFTIE is funded by the [OSCARS project](https://oscars-project.eu/), which has received funding from the European Commission’s Horizon Europe Research and Innovation programme under grant agreement No. 101129751.
![OSCARS and EU logos](images/OSCARS-logo-EUflag.png)
Thanks to Alessandro Felder for reviewing and providing helpful improvements and comments.
