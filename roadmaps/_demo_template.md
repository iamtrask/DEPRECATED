# < Milestone > : < Demo Name >

<b>Background:</b> In this section, you want to describe the general philosophy and intent of the demo. While there are no specific requirements for this paragraph, users should come away with a "general feeling" for the "intent" of the demo, its audience, and an approximate level of effort the demo will require (Does it require infrastructure changes? Is it similar to other demos?)

### Part 1: User Stories

(dummy stories below)
* <b>User Story A:</b> As a <b>Domain Expert</b> in a Particular Field (such as a Doctor), I want to be able to train a neural network using only my mouse (clicking) in a user interface. Furthermore, I want to not have to know anything about neural network configuration. Instead, all defaults should be provided for me, and at a very maximum intuitive explanations made that help me train this neural network on the data made available by the OpenMined blockchain ecosystem.
* <b>User Story B:</b> As a <b>Python Contributor to OpenMined</b>, I want the ability to access X API with only 3 commands. Furthermore, I want the ability to test this API without having to spin up a test blockchain.
* <b>User Story C:</b> As a <b>Designer of OpenMined Branding</b>, I want the ability to update icons and color schemes in all of our applications without having to recompile code.

### Part 2: Mockup

If your demo is a UI demo, in this section you want to include at a minimum a collection of images (and a video is preferred) outlining the exact functionality (hand drawn sketches are fine). If there are more than 2 images/videos, please opt for a list of links to the images like so:

* [Step 1 - Click Button](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium)
* [Step 2 - Fill in Form](https://github.com/OpenMined/PySonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3ALithium)
* [Step 3 - Observe Data Visualization](https://github.com/OpenMined/PySonar/issues?utf8=%E2%9C%93&q=is%3Aissue%20milestone%3ALithium)

In either video or image form, these images should give the exact functionality that is expected by the end user. Heir on the side of TOO MANY in this case. This section is likely the most important because understanding the exact end functionality allows different people on different teams to consider how their parts of the system fit into the project. If you skip a step because you think it's abundantly clear that it's supposed to be there, someone working on a distant part of the system who is not familiar with how you think about things is unlikely to notice it. (This is the kind of thing that causes us to delay Milestones, etc.). So, all that is to say... SAY TOO MUCH with these mockups.


### Part 3: Acceptance Criteria

This section is about listing _specific_ pieces of functionality that allow a developer to know that they are done. Language should be phrased in terms of specific pieces of functionality (i.e. describe the specific CODE tests that should be constructed). These should translate 1:1 into the ISSUES necessary to complete this project.

[PySyft: Epic - < Demo Name >](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium)
* [Issue 54](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Unit Tests should show that Linear models should train at 45 ms per iteration on the Diabetes Dataset.
* [Issue 55](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Unit Tests should show that Sigmoid nonlinearity should forward propagate at 10 ms per iteration on a standard CPU

[Sonar: Epic - < Demo Name >](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium)
* [Issue 321](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Unit Tests should show that ModelRepository should download models with a gas price of 25,000 or less
* [Issue 524](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Unit Tests should show that reversing a model to a former gradient is calculated lazily and costs no gas.

### Part 4: Tutorial Requirements

All Demos should have the required documentation for someone who is brand new to the platform to download and install the appropriate components and run the demo without having to ask another engineer / contributor for help. This section should outline

[Docs: Epic - < Demo Name >](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium)
* [Issue 525](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Jupyter Notebook Installation + Demo
* [Issue 624](https://github.com/OpenMined/mine.js/issues?q=is%3Aissue+milestone%3ALithium) - Hello World App Using This Functionality
