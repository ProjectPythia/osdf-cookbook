# OSDF Cookbook

<img src="thumbnails/OSDF_OSPool_Logos.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)

This Project Pythia Cookbook covers using the Open Science Data Federation (OSDF), a service for streaming scientific data across the globe.

## Motivation

Have you ever been frustrated by the complications of accessing scientific data?  Why can't it "just work", like watching a Netflix movie?

The OSDF is a service that simplifies the streaming of a wide range of scientific datasets with a goal that data access "just works".  It
is meant to improve data availability for researchers working at any scale from individual laptops to distributed computing services
such as the OSG's [OSPool](https://osg-htc.org/ospool).

This cookbook gives motivating use cases from the geoscience community, including using datasets from NSF NCAR's [Research Data Archive](https://rda.ucar.edu/) (RDA) and the datasets of AWS [OpenData](https://aws.amazon.com/opendata/).

## Authors
[Harsha R. Hampapura](https://github.com/hrhampapura)
[Brian Bockelman](https://github.com/bbockelm)
[Alexander Hoelzeman](https://github.com/ahoelzemann)
[Emma Turetsky](https://github.com/turetske)
[Amandha Wingert Barok](https://github.com/amandhawb)
[Aashish Panta](https://github.com/aashishpanta0)
[Justin Hiemstra](https://github.com/jhiemstrawisc)
[Douglas Schuster](https://github.com/DCSCHUS)
[Riley Conroy](https://github.com/rpconroy)
[Kibiwott Koech](https://github.com/kkbch)


### Contributors

<a href="https://github.com/ProjectPythia/osdf-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/osdf-cookbook" />
</a>

## Structure

This cookbook is broken up into two pieces - some background knowledge on the OSDF service itself
and then a series of motivating examples from different repositories accessible via the OSDF.

### OSDF Fundamentals

What is the OSDF?  Who supports it? How can it benefit from my science?  A dive into the infrastructure itself.

### Using Datasets from NCAR's Research Data Archive

NSF NCAR's [Research Data Archive](https://rda.ucar.edu/) (RDA) contains a large collection of meteorological, atmospheric composition, and oceanographic observations, and operational and reanalysis model outputs, integrated with NSF NCAR High Performance Compute services to support atmospheric and geosciences research. This chapter demonstrates how to use common data science tools when streaming from the RDA.

### Using Datasets from FIU's Envistor

Florida International University (FIU) runs the [Envistor project](https://envistorhome.fiu.edu/envistor/), aggregating climate datasets from the south Florida region.

### Using NOAA's SONAR Fisheries Datasets

NOAA maintains a copy of its SONAR-based datasets of Atlanta fisheries data in the popular Zarr format.  This chapter shows how to load and use the datasets and fuse it with other products.

### Using Sentinel Data from AWS

All of AWS OpenData is connected to the OSDF!  This chapter includes examples of streaming Sentinel-2 data, stored in AWS's OpenData program, to your notebook.

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
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the `https://github.com/ProjectPythia/osdf-cookbook` repository:

   ```bash
    git clone https://github.com/ProjectPythia/osdf-cookbook.git
   ```

1. Move into the `osdf-cookbook` directory
   ```bash
   cd osdf-cookbook
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate osdf-cookbook
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
