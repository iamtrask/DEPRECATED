# Feature Evolution Process

> How does the OpenMined ecosystem develop new features 🛣📈

<!-- TOC depthFrom:2 -->

- [Glossary](#glossary)
- [How to define work packages for a component](#how-to-define-work-packages-for-a-component)
    - [Milestones](#milestones)

<!-- /TOC -->

## Glossary

Some words being used repeatedly in this document for quick reference. Most of them will be explained in detail later on.

`Component`: An individual part of the OpenMined **system** (e.g. Mine, Sonar, Syft)

`System`: All of OpenMineds **components** working together

`Roadmap`: Features of the whole **system** bundled into milestones

`Featuremap`: A **component** specific list of features that are planned.

`Issue`: A github issue which is the smallest description of a workpackage, usually specific and belonging to a **component**

`Milestone`: Baselined version of the whole **system** where all **components** have matching interfaces

`MVP`: Special **milestones** that are marketable to the outside

`PoC`: Just..don't use it please?

## How to define work packages for a component

As the OpenMined components have very complex relationships 👨‍👩‍👧‍👦  amongst each other it is important to define development priority for the components Top-Down ⏬. Therefore the first step to figuring out what to work on is to break down the overall vision 👁 (_TODO: add link_) into individual milestones.

### Milestones

> Baselined version of the whole **system** where all **components** have matching interfaces

`Purpose`: Align contributors and provide

`Where to find`: Defined in the system roadmap (_TODO: link to actual roadmap_)

`Conventions`:
* named after elements in the periodic table in ascending order
* should have a theme that is as non-technical as possible, best written as a descriptiion of what changes for the **user**
* goals need to describe the contribution of this release to the overall vision
* assumptions are optional and might describe what has been neglected on purpose

`Example`:

**Milestone Hydrogen**

**Theme:** Reproduce the [diabetes demo use case](https://github.com/OpenMined/PySonar/blob/master/notebooks/Sonar%20-%20Decentralized%20Model%20Training%20Simulation%20(local%20blockchain).ipynb) with all components running indivdually

**Goals:**
* Important Baseline to Enable Distributed Development
* Important Baseline for Onboarding/Teaching Developers

**Use Case:** Diabetes Demo 

**Assumptions:**
* No Capsule: Data Scientist holds Homomorphic Keys

```