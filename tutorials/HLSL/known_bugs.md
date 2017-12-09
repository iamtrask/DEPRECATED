# HLSL Known Bugs

**Background:** HLSL is the language for our GPU backend which has the rather incredible ability to cross-compile GPU code to almost every GPU on the market. However, like all great technologies, it has a few bugs which we've found as different people go to run our project on new platforms. The purpose of this document is to document those bugs so that we can keep track of them over time.

- Windows - Passing in the same ComputeBuffer Twice - https://github.com/OpenMined/OpenMined/issues/95
- Linux - GPU variable names with mulitple underscores - https://github.com/OpenMined/OpenMined/issues/102
