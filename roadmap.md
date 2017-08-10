# Roadmap

> Features of the whole OpenMined **platform** bundled into milestones 🛣 

<!-- TOC depthFrom:2 -->

- [Active](#active)
    - [Hydrogen](#hydrogen)
- [Future](#future)
    - [Helium](#helium)
    - [Lithium](#lithium)
- [Past](#past)

<!-- /TOC -->

This document is part of the [feature evolution process](feature_evolution.md) and provides an overview of all the platform milestones. If you wish to learn more about how these milestones are created, the conventions or what their individual properties represent please refer to the [milestone definition](feature_evolution.md#milestone) and their part in the [roadmap creation](feature_evolution.md#roadmap).

## Active

> currently active milestone

### Hydrogen

**Theme:** Reproduce the [diabetes demo use case](https://github.com/OpenMined/PySonar/blob/master/notebooks/Sonar%20-%20Decentralized%20Model%20Training%20Simulation%20(local%20blockchain).ipynb) with all components running indivdually

**Goals:**
* enable distributed development
* ease onboarding of developers by decoupling the domains

**Assumptions:**
* No Capsule: Data Scientist holds Homomorphic Keys

**Acceptance Criteria:**

The AC for this milestone is defined in form of work instructions necessary for a user to start up a local version of the whole OpenMined platform.

1. no tooling required besides `docker` and `docker-compose` to run locally
1. `docker run` [OM/Sonar](https://github.com/OpenMined/Sonar)
    * local ethereum chain
    * starts blockchain with all contracts compiled into it
1. `docker-compose` [OM/mine](https://github.com/OpenMined/mine.js)
    * spawns `10` mine instances with unique addresses
    * starts local `IPFS` node (for each mine)
    * connectivity to the blockhain from the OM/Sonar step
1. `docker run` [OM/PySonar](https://github.com/OpenMined/PySonar)
1. optional: all these commands are bundled into a single `docker-compose` file available within the PySonar repository

**Issues:**

_TODO@2017-08: add link to issues_

## Future

> lists the specified future milestones (next one on top)

### Helium

**Theme:** Improve security and differential privacy by introducing `capsule`

**Goals:**
* 

**Use Case:**

**Assumptions:**


**Acceptance Criteria:**



### Lithium

**Theme:**

**Goals:**
* 

**Use Case:**

**Assumptions:**

**Acceptance Criteria:**


## Past

> all finished milestones (latest on top)
