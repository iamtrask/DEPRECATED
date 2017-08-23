# Platform Overview

Hi! Welcome to the Contributor Quickstart Guide! The purpose of this tutorial is to give you (all in one place!):

- [Vision:](#vision) a quick rundown of the problem we want to solve and why it's worth our valuable time (and yours!).
- [The Plan:](#plan) a walkthrough of what we're building (the big parts)
- [Development Priorities:](#priorities) these are the ~~droids~~ contributions we're looking for!
- [Workflow:](#workflow) how we work together as a team!
- [Getting Started:](#start) the best places to start contributing

assuming only that you have knowledge of basic Python programming one of the many fields of expertise this platform needs. Let's get started!

## Vision

The vision of our team really starts with the Business Model of the typical AI/ML company. There's a 3 step process that pretty much every company in this space has to go through, and it looks something like this:

- **Step 1:** acquire *Data* about *People* (individuals or groups)
- **Step 2:** train a *Model* that does something useful
- **Step 3:** sell the *use* of that Model (in an App)

In case the term is unfamiliar, a **Model** in this context is any function that *learns* to transform one dataset (the *Input* dataset) into another (the *Target* dataset). A valuable Input dataset might be "Monday Stock Prices" alongside a Target dataset of "Tuesday Stock Prices". Thus, a Model is valuable based on the types of datasets it can transform between, measured by its accuracy in doing so. For example, if it can accurately transform any Monday stock price into the following Tuesday's stock price with perfect accuracy, it'd be quite a valuable model indeed!

Thus, when we consider the the 3 steps for AI business, for most businesses the most valuable part is Step 1 - acquiring data. Nearly all major Machine Learning algorithms are freely available on Github, packaged nicely into one framework or another. Companies like Google and Facebook even sponsor this free software, and this is done because these popular algorithms aren't the difficult/valuable part. It's the Data that creates a competitive advantage. Data is the Natural Resource that Machine Learning / AI consumes in order to become intelligent (which is why people call Data "the new Oil"). In the competitive landscape, companies win or lose not based on the AI algorithms themselves, but based on whether they own the right Data to feed the algorithms, whether they own the Natural Resource necessary to build intelligent systems.

And, since the ultimate source of Data is People, we (as a society) have fallen into a system that rewards the ability of companies to collect data on individuals with vast sums of money, and punishes those that fail to do so with, in the extreme case, bankruptcy (if they ever get started at all). This is so extreme that the de-facto standard business model in Silicon Valley is to acquire users with a free service and then sell their data (either directly to Advertisers or leverage the data themselves for targeted advertising). This is how companies with negative profits, but tons of users/data, can achieve billion dollar valuations.

Given this setup, this creates several significant problems in society, which we, the team of Contributors, hope to solve:

### Problems We Want to Solve

- **Privacy** - people systemically lose control of their data.
- **Lost Natural Income** - data is a natural resource, but people rarely get paid for it.
- **Sensitive Product Problem** - sensitive models don't get trained (details below)
- **Aggregated Power** - a few players have most of the data.

### Privacy

The business model of Machine Learning is setup to value companies based on their ability to, frankly, compromise the privacy of consumers. The more data they can harvest, the better. The more intimate the better (more intimate/personal products!), and the more recent the better (aka the thirst will never be quenched because the data needs to be fresh).

To make matters worse, the consequence of lost privacy is lost control. First there are the obvious flavors of this: risk of theft, resale, or leakage/embarrassment. However, the true loss of control is far more slippery. The vast majority of data online is used for advertising. Advertising is systemic persuasion. Giving up your data is, fundamentally, a loss of control over your beliefs and values. Let me explain.

The advertising industry in the US alone is a [$74 billion](https://www.statista.com/topics/979/advertising-in-the-us/) business. This is for one reason: it works on **you**.

Don't feel bad about this! We're all human. If some social network owns a copy of 5% of the conversations you've had with your loved ones, (ex) girlfriends, enemies, your favorite movies, your relationships, hobbies, religion, sexuality, fears, etc... then it knows who you are. And if someone knows who you are and has the ability to interact with you [once every hour](http://www.gallup.com/poll/184046/smartphone-owners-check-phone-least-hourly.aspx), frankly, they're going to wear you down at some point!

More importantly, Machine Learning models can be trained wherein the input data is "You" and the target data is "things companies want you to do" (value their brand, vote for their candidate, or just buy stuff). Those models are used to interject information into your world 24x7, and trust me when I say that none of us are superhumans. If someone has that kind of knowledge about you and the ability to interject information into your life dozens of times a day, you can't resist. All we can do is our best to minimize its effects and remember who we are, and what we value.

**Goal #1:** So, the first goal of OpenMined is to help people to *reclaim control of their data* by creating the technology necessary for people to leverage the online goods and services they want without needing to offer up their data in return.

### Lost Natural Income

This one is quite simple. People are creating one of the most valuable natural resources of the modern age, and the vast majority of the time they trade that resource in exchange for a simple App (the primary value of which IS the consistent data of the people they know... not the Javascript/HTML used to make it).

We want to see that people are compensated directly for their data in a way that protects their privacy, by creating the first technology that allows people to **rent** their data instead of **sell** their data. We think the term **rent** is most fitting because our solution is designed to allow companies to create value from data that they never see, i.e., train Models on data without seeing the data itself. Any other solution wherein companies see the data is, in our opinion, not fitting of the term **rent** because the data, at that point, has been copied to a foreign machine and is outside the control of the consumer.

**Goal #2:** The second goal of OpenMined is to create technology that facilitates the voluntary **rental** of one's data to a third party in such a a way that privacy is protected. If successful, consumers should be able to earn a significant, passive income by simply living their lives and renting statistical access to the data it generates (not the data itself!)

### Sensitive Product Problem

Let's say I was a company who wanted to build a Machine Learning solution that helped predict whether someone was at risk of a life threatening mental health issue (such as potential suicide or an eating disorder). First, in order to solve such a high-dimensional issue (many potential indicators or false alarms), we would likely need a lot of data. Furthermore, correctly predicting something that people are inclined to hide means that we would very likely need incredibly intimate data. If we collected this kind of data around a large group of people (conversation transcripts, frequent facial expressions, relationship issues/transitions, financial state, work/life balance issues, diet over time), we would further need to know *for those same people* whether or not they had a mental condition.

Frankly, no company or organization should *control* that much data about a person, and fortunately, very few companies do. However, this also has the opposite consequence, very few products get developed to deal with the more intimate aspects of life. This is such a tragedy because mental/physical health, relationship health, and many other intimate issues are some of the most important aspects of life. It's ironic that there are seemingly thousands of apps to help me schedule meetings faster, but few apps that help with a feeling of loneliness.

The major headwind here is the availability of data to help solve the problem. This leads us to the third goal of OpenMined.

**Goal #3:** Facilitate the development of applications that help people in underserved areas, particularly those that deal with intimate/private issues such as mental, physical, and relational health which are limited by data availability.

### Decentralizing Aggregated Power

This one is also quite simple. In the modern area, ye who owns the data owns the world. Presently, the vast majority of consumer data is collected and controlled by a relatively small number of players. As a result, product development (and really societal progress) is heavily influenced by a few central authorities (and is used for their interests). By decentralizing the control of data, we also seek to decentralize the incentives for how it is used. If people own the data, they get to call the shots regarding how it's used. This power dynamic is inherently democratic and good for our society as a whole, and we're here to facilitate it.

**Goal #4:** We want the deciding voice for how data is used to be the population who creates it. Our role is to build the technology that empowers the population with this ability.

## The Plan
