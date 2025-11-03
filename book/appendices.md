---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.16.4
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

# Appendices

## OME-Zarr creation libraries

A number of libraries exist for creating OME-Zarr datasets from existing data.
This table lists them, and drawbacks when working with 3D imaging data.

| Library                                                   | Drawbacks                                                                                                     |
| --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| [ome-zarr-py](https://github.com/ome/ome-zarr-py)         | Not able to correctly downsample 3D images (see [issue #262](https://github.com/ome/ome-zarr-py/issues/262)). |
| [ngff-zarr ](https://ngff-zarr.readthedocs.io/en/stable/) |                                                                                                               |

## OME-Zarr visualisation

There are many different viewers available for OME-Zarr images - see a full [list in the NGFF documentation](https://ngff.openmicroscopy.org/tools/index.html#image-viewers).

### Napari

A good Python-based option is [`napari`](https://napari.org/stable/) - see [installation instructions](https://napari.org/stable/tutorials/fundamentals/installation.html#napari-installation) on their website.

By default, `napari` supports opening Zarr arrays e.g.

```python
import napari

# Data as a zarr array
heart_image = load_heart_data(array_type='zarr')

viewer = napari.Viewer()
viewer.add_image(heart_image)
napari.run()
```

To open OME-Zarr images, you will need to install the [napari-ome-zarr plugin](https://napari-hub.org/plugins/napari-ome-zarr).

Note: `napari`'s support for viewing large, multi-resolution images is still being developed / improved over time. You may find it difficult to browse very large Zarr images through this interface - if so, you may want to try other viewers such as [`webknossos`](https://home.webknossos.org/), [`neuroglancer`](https://github.com/google/neuroglancer) or [`BigDataViewer`](https://imagej.net/plugins/bdv/).
