# Helium Roadmap

**Theme:** Full Local Linear MVP

**Helium Demos:**
* [Arbitrary Data Demo](https://github.com/OpenMined/Docs/roadmaps/helium/arbitrary_data_demo.md)
* [Twitter Adapter Demo](https://github.com/OpenMined/Docs/roadmaps/helium/twitter_adapter_demo.md)
* [Capsule Hosted Black Box Demo Demo](https://github.com/OpenMined/Docs/roadmaps/helium/hosted_capsule_demo.md)
* [Capsule Key Rotation Demo Demo](https://github.com/OpenMined/Docs/roadmaps/helium/key_rotation_capsule_demo.md)
* [YASHE based Logistic Regression Demo](https://github.com/OpenMined/Docs/roadmaps/helium/YASHE_logistic_demo.md)


**Goals:**
* Introduce `capsule` component
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
