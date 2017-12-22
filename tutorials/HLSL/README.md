# HLSL / GPU docs
OpenMined uses [Unity](https://unity3d.com) as explained in [Why Unity?](https://github.com/OpenMined/OpenMined/blob/master/tutorials/WhyUnity.md), so here are interesting links for learning HLSL (CUDA links are welcome).

## HLSL Overview
Introduction to Thread & Group Indexing
- https://msdn.microsoft.com/en-us/library/windows/desktop/ff471568(v=vs.85).aspx

Most excellent resource on HLSL with programming patterns (from NVIDIA)
- http://developer.download.nvidia.com/compute/DevZone/docs/html/DirectCompute/doc/DirectCompute_Programming_Guide.pdf

Introduction to Compute Shaders
- http://kylehalladay.com/blog/tutorial/2014/06/27/Compute-Shaders-Are-Nifty.html
- http://www.lindsaygcox.co.uk/tutorials/unity-shader-tutorial-an-intro-to-compute-shaders/
- http://www.emersonshaffer.com/blog/2016/5/11/unity3d-compute-shader-introduction-tutorial
- http://www.codinglabs.net/tutorial_compute_shaders_filters.aspx

## Parallel reduction techniques
Comprehensive resource on how optimize parallel reduction in GPUs. In particular, they explain the sequential addressing method we sometimes use, and more optimizations with comparative speedup scores
- http://developer.download.nvidia.com/compute/cuda/1.1-Beta/x86_website/projects/reduction/doc/reduction.pdf

HLSL tutorial project
- http://catflier.blogspot.fr/2013/10/parallel-reduction-basics.html
- https://github.com/speps/graphicsdemoskeleton


## Other
Atomic add
- https://forum.unity.com/threads/using-interlockedadd.317791/

CUDA shared memory bank conflicts explained
- http://cuda-programming.blogspot.fr/2013/02/bank-conflicts-in-shared-memory-in-cuda.html

Tame down warnings
- https://infiniteproductionsblog.wordpress.com/2016/06/30/how-to-fix-shader-warnings-with-monogame/

