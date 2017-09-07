# Helium : Arbitrary Data Demo

<b>Background:</b> In the Hydrogen release, we took the original [Sonar Demo Notebook](https://github.com/OpenMined/PySonar/blob/master/notebooks) and packaged it into a single on-liner which you can see in this [Video](https://www.youtube.com/watch?v=cc7Lh9TgSeI). This runs the entire ecosystem for the OpenMined platform. However, unfortunately this is tied to a specific demo dataset. In this project, we want to allow for this demo to be executed against any arbitrary dataset such that when the (one-liner) Demo is run, Data Scientists can open the notebook and run arbitrary experiments against any dataset they disperse throughout the 10 demo miners.

### Part 1: User Stories

* <b>User Story A:</b> As a user of the Docker one-liner, I want the ability to spin up test mines on any dataset of my choosing (not just the Diabetes Dataset) so that I can run arbitrary simulations with arbitrary dataset.

* <b>User Story B:</b> As a miner using mine.js, I want the ability to upload one or more datasets into the Mine which have a specific name or ID. I then want the ability to perform data science using PySonar wherein I select a dataset according to this simple name or ID lookup.

### Part 2: Acceptance Criteria

[mine.js: Epic - Arbitrary Data Demo](https://github.com/OpenMined/mine.js/issues/43)
  - [Issue 44](https://github.com/OpenMined/mine.js/issues/44) - a stand-alone set of instructions should exist for loading an arbitrary number of datasets into a mine assuming those datasets are in a standardized format.
  - [Issue 45](https://github.com/OpenMined/mine.js/issues/45) - The one-liner should be runnable against an arbitrary folder of datasets.

### Part 3: Tutorial Requirements

All Demos should have the required documentation for someone who is brand new to the platform to download and install the appropriate components and run the demo without having to ask another engineer / contributor for help.

Docs
* [Docs Issue 57](https://github.com/OpenMined/Docs/issues/57) - User Story B - Tutorial
* [Docs Issue 58](https://github.com/OpenMined/Docs/issues/58) - User Story A Tutorial
