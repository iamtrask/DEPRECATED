## Step 1: Introduce Yourself!

#### Part 1: Join the Slack Team
Proceed to our website (http://openmined.org/) and click the link to get an invitation to our Slack team.

#### Part 2: Star the Repos!!
Help show your support for OpenMined by starring our Github Repositories!!! This not only helps show your presence via the stargazers list, but it also helps raise awareness for our repositories on Github's "Trending Repositories" page!

#### Part 3: Fill out your Slack Profile
Fill out your Slack profile with your background and interests, and introduce yourself in the #general-discussion channel.

#### Part 4: Fill out the New Contributor Survey!
This will help us know who you are!
https://goo.gl/forms/86y61YQx6bIAI8TF3

## Step 2: OpenMined Introduction

This video covers the platform as a whole including high-level goals and the broad architecture strategies (the big moving parts!).

[![Watch the video](https://github.com/OpenMined/Docs/raw/master/img/OpenMinedIntro.png)](https://www.youtube.com/watch?v=sXFmKquiVnk)

- [OpenMined Introduction Slides](https://docs.google.com/presentation/d/1Tm7jh3pChks0ObJNb7x2ZZhhVOJhmCVN2KDPWyZohQU/edit)
- [Frequently Asked Questions](../faq.md)

### Next Steps

Great!  You've made it this far.  Steps 3 - 6 get a little technical.  If you're not a developer or don't want to get into the weeds for now, then head down to Step 7.  There we'll discuss how you can get started contributing to OpenMined based on your interests and skills!

## Step 3: Syft Installation + Homomorphic Encryption Demo

Once you've got a general understanding of the platform, you'll want to start with the basics, getting Homomorphic Encryption up and running within PySyft.

- [First, install PySyft](https://github.com/OpenMined/PySyft/)
- [Second, test this notebook](https://github.com/OpenMined/PySyft/blob/master/notebooks/Syft%20-%20Paillier%20Homomorphic%20Encryption%20Example.ipynb)

## Step 4: Homomorphically Encrypted Linear Classifier Demo

[Complete this Notebook](https://github.com/OpenMined/PySyft/blob/master/notebooks/Syft%20-%20Paillier%20Encrypted%20Linear%20Classification.ipynb)

## Step 5: Install Sonar, PySonar, and Demo

- [Install Sonar](https://github.com/OpenMined/Sonar)
- [Install PySonar](https://github.com/OpenMined/PySonar)
- Demo: Encrypted Neural Network on Test Ethereum Blockchain
  - https://github.com/OpenMined/PySonar/blob/master/notebooks/Sonar%20-%20Decentralized%20Model%20Training%20Simulation%20(local%20blockchain).ipynb

- Demo2: Encrypted Neural Network on Test Ethereum Blockchain (from source)
  - https://github.com/OpenMined/PySonar/blob/master/notebooks/Sonar%20-%20Decentralized%20Learning%20Demo.ipynb

## Step 6: Install Zenhub Plugin

In order to see our documentation and issues in all their full glory, you'll want to install this browser plugin for Zenhub. Just navigate to http://zenhub.com and click the "Add ZenHub to GitHub" button.

## Step 7: Figure out where you want to contribute!

We welcome all people willing to contribute, Irrespective of their skill set and level of experience. The following is a list of consistently needed skillsets:

### Machine learning
**Repositories:**
- [PySonar](https://github.com/OpenMined/PySonar) - Python client to blockchain application (Sonar)
- [sonar.js (Link pending) - Node.js client to blockchain application (Sonar)
- [Sonar](https://github.com/OpenMined/Sonar) - Python Ethereum blockchain implementation
- [PySyft](https://github.com/OpenMined/PySyft) - Python deep learning library

**Slack channels:** #team_sonar, #team_syft

### Homomorphic Encryption
**Repositories:**
- [PySyft](https://github.com/OpenMined/PySyft) - Python deep learning library

**Slack channels:** #team_syft

### Blockchain
**Repositories:**
- [Sonar](https://github.com/OpenMined/Sonar) - Python Ethereum blockchain implementation
- [PySonar](https://github.com/OpenMined/PySonar) - Python client to blockchain application (Sonar)
- sonar.js (Link pending) - Node.js client to blockchain application (Sonar)

**Slack channels:** #team_sonar

### Node.js Development
**Repositories:**
- [mine.js](https://github.com/OpenMined/mine.js) - Node.js implementation of a user's personal data store, calls Syft for training
- sonar.js (Link pending) - Node.js client to blockchain application (Sonar)

**Slack channels:** #team_sonar, #team_syft, #team_mine

### Python Development
**Repositories:**
- [PySonar](https://github.com/OpenMined/PySonar) - Python client to blockchain application (Sonar)
- [PySyft](https://github.com/OpenMined/PySyft) - Python deep learning library
- [Capsule](https://github.com/OpenMined/Capsule) - Blockchain oracle for time released public/private key generation/interaction
- [PyYASHE](https://github.com/OpenMined/PyYashe) - An experimental library for developing a high performance YASHE implementation

**Slack channels:** #team_sonar, #team_syft, #team_capsule

### React.js Development
**Repositories:** Coming soon.

**Slack channels:** #team_uiux

### DevOps
**Repositories:** All

**Slack channels:** #team_devops

### Technical Writing
**Repositories:** None

**Slack channels:** #process, #team_docs

### UI Design
User interface design is currently underway on SonarUI and MineUI - the user interfaces for data scientists and data hosts respectively. These are currently being discussed in the UI channel of Slack.

### UX Testing
We need lots of testers. Currently, this work is not related to any user interfaces, as those have not yet been designed or developed. We will have more need for this in the **very** near future, however. Feel free to reach out in the UX channel of Slack.

### Legal and Marketing
For any of these topics - reach out to @trask in Slack. The needs of each are varied... here are a few examples:

There are a plethora of legal issues that come with a person taking back ownership of their information. How is ownership of data is transferred or dissolved after death? How tightly can we implement with third-party data providers from a legal perspective? What does the future of data ownership look like from a legal perspective?

We have a highly capable set of creative people working on the brand of OpenMined. How do we get this brand to be viewed positively by developers? How would a rollout to the general public work? How much time should an open source project spend on marketing itself?

### Anything else?
We'd love to have you! The only requirement for joining the OpenMined contributor network is a desire to follow the core values and vision of the project. Feel free to reach out in the #general-discussion, #beginner, and #questions channel on Slack and someone will be sure to point you in the right direction!

## Step 8: Congratulations You're Ready!

You now have the basics of the OpenMined ecosystem up and running and are ready to take on `beginner` level projects (Issues). We've gone out of our way to make sure that there are a plethora of mini-projects (Issues) that are 100% entry level. The way to find one is to pick any GitHub repository and click the *Issues* Tab at the top. This should take you to a place that looks like this.

![Issues.png](https://github.com/OpenMined/Docs/raw/master/img/issues.png)


Next, you click "Labels -> beginner".


Or, click on this link:
[Labels -> beginner](https://github.com/OpenMined/PySyft/issues?q=is:open+is:issue+label:beginner).


This will filter out all tickets except for the `beginner` tickets.


Click one of the tickets and you'll see something like this:

![https://github.com/OpenMined/Docs/raw/master/img/beginner_ticket.png](https://github.com/OpenMined/Docs/raw/master/img/beginner_ticket.png)

This ticket contains instructions for how to add a subtraction function to our Base Tensor object, with links to further documentation to help explain everything the ticket should do. If you have ANY questions about a ticket, simply message the person who created the ticket (in the ticket above, that's @trask on Slack)

Before beginning work, make sure to be aware of our [contributing guidelines](./guidelines.md).

Once your first Pull Request is merged into an OpenMined repository, you'll get your official invite to become a *Member of the Github Organization*!
