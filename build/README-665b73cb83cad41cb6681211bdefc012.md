# MRMS Cookbook

<img src="thumbnails/mrms-thumbnail.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/mrms-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/mrms-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/mrms-cookbook/main?labpath=notebooks)
<!-- [![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405) -->


This Project Pythia Cookbook covers how to access, analyze, and visualize Multi-radar, Multi-sensor (MRMS) Data.

## Motivation

The Multi-Radar, Multi-Sensor (MRMS) System combines radar, surface, and upper-air observation to produce a high-resolution (1 km) dataset used by researchers and forecasters alike. Despite its use, there are few published Python workflows that illustrate how to access MRMS data from Amazon Web Services (AWS) and produce beautiful, useful visualizations. We hope this cookbook serves the MRMS-user community well!

## Authors

<a href="https://github.com/ProjectPythia/mrms-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/mrms-cookbook" />
</a>

### Contributors

<a href="https://github.com/ProjectPythia/cookbook-template/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/cookbook-template" />
</a>

## Structure

- <b>Chapter 1</b> offers a brief overview of MRMS data and provides context for how the data is organized on AWS.
- <b>Chapter 2</b> contains a case study of the [March 24–27 2023 Tornado Outbreak](https://en.wikipedia.org/wiki/Tornado_outbreak_of_March_24–27,_2023), showcasing fields relevant to severe weather prediction.
- <b>Chapter 3</b> examines another recent severe weather event, the [July 2025 Central Texas Floods](https://en.wikipedia.org/wiki/July_2025_Central_Texas_floods), instead focusing on precipitation fields and [FLASH](https://www.nssl.noaa.gov/projects/flash) output, including comparisons to station observations.
- <b>Chapter 4</b> compares MRMS-derived precipitation estimates at Bankhead National Forest (BNF) Field Sites.
- <b>Chapter 5</b> offers a real-time look at MRMS data with the opportunity to select certain data fields.

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
`Shift`\+`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note: not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/mrms-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/mrms-cookbook.git
   ```

1. Move into the `mrms-cookbook` directory
   ```bash
   cd mrms-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate mrms-cookbook-dev
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
