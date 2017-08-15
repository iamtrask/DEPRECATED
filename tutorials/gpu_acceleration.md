# GPU (Graphic Processing Unit) Acceleration (or GPGPU, General Purpose Graphic Processing Unit)

## Why

GPU acceleration greatly improves the performance of mathematical operations because the processors are specifically designed to do one thing very well.  For overly brief video to outline this in practice, we can thank mythbusters [Mythbusters - CPU vs GPU](https://www.youtube.com/watch?v=-P28LKWTzrI).  There is also a benchmark here: [gpu.js](http://gpu.rocks)

## Types

| Platform        | Technology            | Libraries                                                 |
|-----------------|-----------------------|-----------------------------------------------------------|
| Web/Javascript  | WebGL                 | [gpu.js](http://gpu.rocks)                                |
| Node            | Arrayfire, OpenCL     | [ArrayFire.js](https://github.com/arrayfire/arrayfire-js), [Nooocl](https://github.com/unbornchikken/nooocl) |
| Python          | Cuda?                 | ?                                                         |

## How

A current proposal for javascript is to use [gpu.js](http://gpu.rocks) for javascript because you can write in simple javascript and it is translated to whatever technology the platform you are working on supports (WebGL now, and OpenCL when it is available).

### Examples

```js
//import gpu.js
import Gpu from 'gpu';

//instantiate a gpu.js instance
const gpu = new Gpu();

//create your function
const multiplyElement = gpu.createKernel(function(matrix1, matrix2) {
  return matrix1[this.thread.y][this.thread.x] * matrix2[this.thread.y][this.thread.x];
});

//user your kernel
const c = multiplyElement(a, b);
```
