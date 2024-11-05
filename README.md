# Trap and Antiattractant Placement Generation Notebook

## Overview
This Jupyter notebook provides a specialized solution for generating trap and antiattractant placement strategies using 30-meter resolution satellite data. It's an independent adaptation of modules originally developed for the TANABBO project (Version 1.27.1), where I contributed. Unlike the original GRASS Python files used in TANABBO, this notebook is tailored for a more focused application in forest pest management.

## Prerequisites
- Basic knowledge of Jupyter notebooks.
- Understanding of GIS and remote sensing data.

## Input Data Requirements
- **Yearly Time Series of Forest Losses:** TIFF files named as `bb_spot_[year].tif`, e.g., `bb_spot_2018.tif`.
- **Spruce Forest Mask:** A mask file (e.g., `s50mask.tif`) showing spruce forest distribution. A good start could be forest units older than 50 years with >50% spruce.

### Data Specifications
- Format: TIFF
- Resolution: 30 meters
- Consistent file size across datasets.

## Installation
1. Clone or download this notebook.
2. Install Python and necessary libraries.
3. Launch the notebook in a Jupyter environment.

## Usage
1. **Loading Data:** Import forest loss and spruce forest mask files.
2. **Trap Placement Algorithm:**
   - Determines optimal trap placement.
   - Determines optimal antiattractant placement.
   - Adjustable trap spacing between each other, with a fixed distance of 15 meters from the forest edge.

## Features
- **Customizable Trap Spacing:** Modify the distance between traps.
- **Edge Detection:** For strategic trap placement.
- **Visualization:** Maps to display proposed placements.

## Limitations
- Optimized for 30m resolution. Not tested with other resolutions or sizes.
- Assumes uniformity in input data.

## Contributing
Feel free to contribute to this project. Please follow the guidelines outlined in the [tanabbo repository](https://github.com/tanabbo/tanabbo) for contributions.

## Acknowledgements
This notebook was developed as an independent extension of my work on TANABBO Version 1.27.1. Special thanks to the TANABBO team and community.

## Disclaimer
The tool is provided "as is", with no warranties. Users are responsible for their application of the tool and interpretations of the results.
