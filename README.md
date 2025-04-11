# napari-mask-density

[![License BSD-3](https://img.shields.io/pypi/l/napari-mask-density.svg?color=green)](https://github.com/kuang-da/napari-mask-density/raw/main/LICENSE)
[![PyPI](https://img.shields.io/pypi/v/napari-mask-density.svg?color=green)](https://pypi.org/project/napari-mask-density)
[![Python Version](https://img.shields.io/pypi/pyversions/napari-mask-density.svg?color=green)](https://python.org)
[![tests](https://github.com/kuang-da/napari-mask-density/workflows/tests/badge.svg)](https://github.com/kuang-da/napari-mask-density/actions)
[![codecov](https://codecov.io/gh/kuang-da/napari-mask-density/branch/main/graph/badge.svg)](https://codecov.io/gh/kuang-da/napari-mask-density)
[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-mask-density)](https://napari-hub.org/plugins/napari-mask-density)
[![npe2](https://img.shields.io/badge/plugin-npe2-blue?link=https://napari.org/stable/plugins/index.html)](https://napari.org/stable/plugins/index.html)
[![Copier](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-grayscale-inverted-border-purple.json)](https://github.com/copier-org/copier)

A napari plugin for analyzing mask density in regions of interest

----------------------------------

## Installation

You can install `napari-mask-density` via [pip]:

    pip install napari-mask-density

## Description

`napari-mask-density` is a plugin for the [napari] image viewer that allows users to analyze the density of objects within selected regions of interest (ROIs). This is particularly useful for cell counting, particle analysis, and other applications where quantifying the distribution of segmented objects is important.

## Features

- **Select multiple mask layers**: Analyze multiple segmentation masks simultaneously.
- **Define custom regions of interest**: Draw rectangular ROIs to specify areas for analysis.
- **Microns-per-pixel calibration**: Convert measurements to real-world units.
- **Density calculation**: Calculate and display object density (objects per μm²).
- **Export to CSV**: Save analysis results for further processing or reporting.

## Usage

1. **Start napari** and load your images and segmentation masks
2. **Open the plugin**: Find "Mask Density" in the Plugins menu
3. **Set the microns-per-pixel value** for accurate spatial measurements
4. **Select mask layer(s)** from the list that you want to analyze
5. **Create a rectangular ROI** by clicking the "Add Selection ROI" button and drawing on the image
6. **Analyze** by clicking the "Analyze Selected Region" button
7. **View results** in the plugin panel
8. **Export results** to CSV for further analysis

## Results

For each selected mask layer within the ROI, the plugin calculates and displays:

- Number of masks (objects) detected
- Area of the region in pixels and μm²
- Density of objects per μm²

## Requirements

- napari
- numpy
- pandas
- scikit-image

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

Distributed under the terms of the [BSD-3] license,
"napari-mask-density" is free and open source software.

## Issues

If you encounter any problems, please [file an issue] along with a detailed description.

[napari]: https://github.com/napari/napari
[pip]: https://pypi.org/project/pip/
[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
[file an issue]: https://github.com/kuang-da/napari-mask-density/issues
