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
    * jupyter notebook is accessible from host system

1. optional: all these commands are bundled into a single `docker-compose` file available within the PySonar repository

**Involved components & issues:**
* [OM/mine](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3AHydrogen)
* [OM/Sonar](https://github.com/OpenMined/Sonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3AHydrogen%20)
* [OM/PySonar](https://github.com/OpenMined/PySonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3AHydrogen%20)

## Future

> lists the specified future milestones (next one on top)

### Helium

**Theme:** Introduce `capsule` component

**Goals:**
* Improve security by trusted component with key ownership
* Tackle differential privacy issue by shielding individual gradients from the data scientist

**Assumptions:**
* no changes in mine or Sonar

**Acceptance Criteria:**
1. [OM/capsule](https://github.com/OpenMined/Capsule) is dockerized and can be started using `docker run` (platform wide description updated respectively)
1. `diabetes usecase` according to **hydrogen** is (still) operational

**Involved components & issues:**
* [OM/capsule](https://github.com/OpenMined/capsule/issues?q=is%3Aissue+milestone%3AHelium)
* [OM/PySonar](https://github.com/OpenMined/PySonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3AHelium)

### Lithium

**Theme:** Distributed OpenMined platform for _tweet content_ ➡️  _hashtag prediction_

**Goals:**
* use a public blockchain to enable multi-user proof of concept phase
* support `diabetes` and personal `twitter` data in the mine/Sonar
* basic NLP support in `pySonar`

**Assumptions:**
* `pySonar` features might be tailored towards this use case
* a user in the network might not own twitter data (diabetes dummy comes with the mine)
* there are no dynamic rules in the training priority

**Acceptance Criteria:**
_MISSING_

**Involved components & issues:**
* [OM/mine](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium)
* [OM/PySonar](https://github.com/OpenMined/PySonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3ALithium)

## Past

> all finished milestones (latest on top)
