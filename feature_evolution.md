# Feature Evolution Process

> How does the OpenMined platform develop new features? 🛣📈

<!-- TOC depthFrom:2 -->

- [Glossary](#glossary)
- [How work packages for components are defined](#how-work-packages-for-components-are-defined)
- [Vision to Roadmap (Top-Down FEP)](#vision-to-roadmap-top-down-fep)
    - [Milestones](#milestones)
    - [Roadmap](#roadmap)
- [Roadmap to issues](#roadmap-to-issues)
    - [Featuremap](#featuremap)
    - [Issue](#issue)
- [Ideation (Bottom-Up)](#ideation-bottom-up)

<!-- /TOC -->

## Glossary

Some words being used repeatedly in this document for quick reference. Most of them will be explained in detail later on.

`❄️ Component`: An individual part of the OpenMined **platform** (e.g. Mine, Sonar, Syft)

`⛄️ Platform`: All of OpenMineds **components** working together

`🛣 Roadmap`: Features of the whole **platform** bundled into milestones

`💡 Featuremap`: A **component** specific list of features that are planned.

`☑️ Issue`: A github issue which is the smallest description of a workpackage in a differential stlye (_add/remove .._), usually specific and belonging to a **component**

`📝 Specification`: Describing an absolute state of either a **component** or the **platform** (_component/platform spec_). Every other milestone it might make sense to combine the differential **milestones** into a new platform specification - or vice-versa.


`📦 Milestone`: Baselined version of the whole **platform** where all **components** have matching interfaces

`⚖️ acceptance criteria`: _aka Definition of Done (DoD)_, list of things that the change needs to fulfill to be considered a solution (comes with **issues** and **milestones**)

`👁 Vision`: Overall goal OpenMined is aiming to achieve (_@2017-08: Link to vision_)

`🎁 MVP`: Special **milestones** that are marketable to the outside

`🚫 PoC, Platform`: Just..don't use it please?

## How work packages for components are defined

## Vision to Roadmap (Top-Down FEP)

As the OpenMined components have very complex relationships 👨‍👩‍👧‍👦  amongst each other it is important to define development priority for the components Top-Down ⏬. Therefore the first step to figuring out what to work on is to break down the overall vision 👁 (_TODO@2017-08: add link_) into individual [milestones](#milestones). Each milestone comes with acceptance criteria that are required for the following step in the FEP.

The key components in this step are described in detail below:

### Milestones

> Baselined version of the whole **platform** where all **components** have matching interfaces

`Purpose`: Align contributors and provide

`Where to find`: Defined in the platform roadmap (_TODO@2017-08: link to actual roadmap_)

`Conventions`:
* named after elements in the [periodic table](http://www.ptable.com/) in ascending order
* happen in (roughly) fixed time intervals
* features are mapped into milestones **NOT** vice-versa i.e. break large features down
* should have a theme that is as non-technical as possible, best written as a descriptiion of what changes for the **user**
* goals need to describe the contribution of this release to the overall vision
* assumptions are optional and might describe what has been neglected on purpose

`Example`: see [hydrogen milestone](roadmap.md#hydrogen)

### Roadmap

> One document to rule all milestones you must have 💍

`Purpose`: Top Level document to get an understanding of current platform status and future plans w/ **rough** timeplan

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

> features/milestones broken down into coder speak

`Purpose`: Isolated work package description for developers to pick and code

`Where to find`: [Github issues](https://github.com/OpenMined/Sonar/issues) section for the respective repository

`Conventions`:
* issues are not assigned by default
    * assign when someone is commited to working on it
    * component maintainer checks if there are _blocked_ issues w/o progress
* issues required for milestone should have the milestone label
* use labels in a descriptive manner
    * `enhancement`, `bug`, `docs`
    * `for-beginner`, `my-first-pr`
    * `wontfix`
* add acceptance criteria as well as a full description (or links) of the issue to solve
    * try to not to enforce solutions unless technically necessary
    * refer to coding standards if necessary (e.g. existing API definitions)

`Example`: [this PySyft issue](https://github.com/OpenMined/PySyft/issues/30)

## Ideation (Bottom-Up)

In addition to breaking down features in a Top-Down manner it is helpful to have an established bottom-up process in place. The goal behind the ideation process is for a component to come up with individual features that might not be part of planned milestones. In this case the entry point for the FEP is the components [featuremap](#featuremap). Adding a new feature that is not mapped to a milestone is a valid move. However when prioritizing issue progress milestone-related issues should always be worked on first. After discussing/adding an additional feature to the featuremap the same process is done to finally end up with issues as described in the [roadmap to issues section](#roadmap-to-issues).
