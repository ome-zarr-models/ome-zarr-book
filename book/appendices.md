# Appendices

## OME-Zarr creation libraries

There are many different creation software libraries available for OME-Zarr images - see a full [list in the NGFF documentation](https://ngff.openmicroscopy.org/tools/index.html#dataset-reading-writing).
When choosing a tool to write OME-Zarr data, you should be aware of how it handles memory, in particular if it reads entire images into memory at once or not.

## OME-Zarr visualisation

There are many different viewers available for OME-Zarr images - see a full [list in the NGFF documentation](https://ngff.openmicroscopy.org/tools/index.html#dataset-viewers).

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
