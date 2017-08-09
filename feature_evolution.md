# Feature Evolution Process

> How does the OpenMined ecosystem develop new features? 🛣📈

<!-- TOC depthFrom:2 -->

- [Glossary](#glossary)
- [How work packages for components are defined](#how-work-packages-for-components-are-defined)
- [Vision to Roadmap (Top-Down FEP)](#vision-to-roadmap-top-down-fep)
    - [Milestones](#milestones)
    - [Roadmap](#roadmap)
- [Roadmap to issues](#roadmap-to-issues)
    - [Featuremap](#featuremap)
    - [Issue](#issue)

<!-- /TOC -->

## Glossary

Some words being used repeatedly in this document for quick reference. Most of them will be explained in detail later on.

`❄️ Component`: An individual part of the OpenMined **system** (e.g. Mine, Sonar, Syft)

`⛄️ System`: All of OpenMineds **components** working together

`🛣 Roadmap`: Features of the whole **system** bundled into milestones

`💡 Featuremap`: A **component** specific list of features that are planned.

`☑️ Issue`: A github issue which is the smallest description of a workpackage in a differential stlye (_add/remove .._), usually specific and belonging to a **component**

`📝 Specification`: Describing an absolute state of either a **component** or the **system** (_component/system spec_). Every other milestone it might make sense to combine the differential **milestones** into a new system specification - or vice-versa.


`📦 Milestone`: Baselined version of the whole **system** where all **components** have matching interfaces

`⚖️ acceptance criteria`: _aka Definition of Done (DoD)_, list of things that the change needs to fulfill to be considered a solution (comes with **issues** and **milestones**)

`👁 Vision`: Overall goal OpenMined is aiming to achieve (_@2017-08: Link to vision_)

`🎁 MVP`: Special **milestones** that are marketable to the outside

`🚫 PoC, Project`: Just..don't use it please?

## How work packages for components are defined

## Vision to Roadmap (Top-Down FEP)

As the OpenMined components have very complex relationships 👨‍👩‍👧‍👦  amongst each other it is important to define development priority for the components Top-Down ⏬. Therefore the first step to figuring out what to work on is to break down the overall vision 👁 (_TODO@2017-08: add link_) into individual [milestones](#milestones). Each milestone comes with acceptance criteria that are required for the following step in the FEP.

The key components in this step are described in detail below:

### Milestones

> Baselined version of the whole **system** where all **components** have matching interfaces

`Purpose`: Align contributors and provide

`Where to find`: Defined in the system roadmap (_TODO@2017-08: link to actual roadmap_)

`Conventions`:
* named after elements in the [periodic table](http://www.ptable.com/) in ascending order
* happen in (roughly) fixed time intervals
* features are mapped into milestones **NOT** vice-versa i.e. break large features down
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

### Roadmap

> One document to rule all milestones you must have 💍

`Purpose`: Top Level document to get an understanding of current project status and future plans w/ **rough** timeplan

`Where to find`: Markdown in the OpenMined/docs repositry. _TODO@2017-08: Link to trasks doc_

`Conventions`:
* should feature at least 3 milestones into the future 🔮
* core team is responsible to break milestone goals/acceptance critera into issues

`Example`: Not necessary as there is only one roadmap, [look at it](TODO@2017-08://link.lol) ffs.

## Roadmap to issues

The acceptance criteria for a milestone are broken down into features for affected components. For this step it is crucial to get all affected components involved. This process is initiated as part of the regular `core team meeting`, detailed discussions are postponed to individual sessions. Breaking down acceptance criteria can go one of two ways:
1. the feature that componentA needs to contribute to a milestone is already available, due to pre-development / frontloading ➡️ all good
2. issues need to be created to fulfill the milestone acceptance criteria. This should become apparent at least 2 milestones in advance  ➡️ create issues and integrate with featuremap

### Featuremap

> Describing the active/future feature development for an individual component

`Purpose`: Allow ideation within a single component and align with OpenMined vision

`Where to find`: Markdown document in each component repository. _TODO@2017-08: Link to feauturemap prototype_

`Conventions`:
* features required for a milestone should be marked with the milestone name
* available issues should be linked to the issues
* featuremaps are discussed with the top contributors of the respective component
* features that require other components to be modified should be _nominated_ and proposed during the `core team meeting` as potential goals for an upcoming milestone
    * bonus points for features that are developed isolated in a component with mocked interfaces
* features are turned into issues/issue proposals ➡️ actual issues ➡️ implementation

### Issue

> work packages for any developer to pick and work on

`Purpose`: 

`Where to find`: Github issues section for the respective repository

`Conventions`:
