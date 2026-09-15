# Flood Visualizer using Google Earth Engine

This project detects and estimates flooded areas using Sentinel-1
Synthetic Aperture Radar (SAR) imagery and Google Earth Engine.

## Study Area

Ernakulam District, Kerala, India

The project focuses on detecting changes in surface water before and
after the 2018 Kerala floods.

## Technologies Used

- Google Earth Engine
- JavaScript
- Sentinel-1 SAR
- Google Earth Engine Datasets
- Refined Lee Speckle Filter
- Google Cloud / Earth Engine

## Methodology

The flood detection process consists of the following steps:

1. Load and filter Sentinel-1 SAR data
2. Generate pre-flood and post-flood images
3. Visualize RGB composites
4. Apply Refined Lee speckle filtering
5. Detect flooded areas using thresholding
6. Remove permanent water bodies
7. Remove steep areas using slope filtering
8. Remove disconnected pixels
9. Calculate the total flooded area
10. Export the flooded-area result as a CSV file

## Project Structure

### 01 - Load and Filter Sentinel-1 Data

Loads Sentinel-1 GRD data and filters it according to:

- Study area
- Date range
- Instrument mode
- Polarization
- Orbit direction
- Spatial resolution

### 02 - Visualizing RGB Composite

Creates a visualization using Sentinel-1 VV and VH bands
along with their ratio.

### 03 - Applying Speckle Filter

Applies the Refined Lee filter to reduce speckle noise
from Sentinel-1 SAR imagery.

### 04 - Applying a Threshold

Uses changes between pre-flood and post-flood images
to identify potential flooded areas.

### 05 - Applying Masks

Removes:

- Permanent water bodies
- Steep areas
- Small disconnected regions

to improve flood detection accuracy.

### 06 - Calculating Flooded Area

Calculates the total flooded area in hectares and
exports the result as a CSV file to Google Drive.

## Google Earth Engine

This project is intended to run using my own
Google Earth Engine / Google Cloud project.

> Note: The Google Earth Engine application is deployed
> separately through Google Earth Engine. The GitHub repository
> contains the source code and documentation.

## Application

The Google Earth Engine application link will be added here
after deployment.

## Author

**Sarbojit Ghosh**

M.Tech — Distributed & Mobile Computing  
Jadavpur University

## Repository

This repository contains my independent copy of the
Flood Visualizer project for development, experimentation,
and deployment using Google Earth Engine.
