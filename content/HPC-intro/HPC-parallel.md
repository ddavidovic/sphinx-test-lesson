# Parallel computing

<!--
## Serial vs. parallel computing
-->

```{figure} ../img/dist-share-mem.png
Shared-memory vs. distributed-memory system arhitecture.
```

## Parallel programming models

### MPI

### OpenMP

### CUDA/ROCm

```{figure} ../img/gpu_acceleration.png
Heterogeneous programming model. Figure taken from [https://es.mathworks.com/help/gpucoder/gs/gpu-prog-paradigm.html](https://es.mathworks.com/help/gpucoder/gs/gpu-prog-paradigm.html)
```
Highly parallelizabile portions of the code are executed on the GPU devices, while the reminder of the code or sequential parts are still executed on the CPU.

## Measuring the performance

```{Callout} Measure of computer performance
**Floating-point operations per second (FLOPS)**: Number of floating-point artihmetic calculations that the processor can perform within a second.
```

| Name     | Unit     | Value |
|----------|----------|----------|
| megaFLOPS | MFLOPS |  10<sup>6</sup> |
| gitaFLOPS | GFLOPS |  10<sup>9</sup> |
| teraFLOPS | TFLOPS |  10<sup>12</sup> |
| petaFLOPS | PFLOPS |  10<sup>15</sup> |
| exaFLOPS  | EFLOPS |  10<sup>18</sup> |
| zettaFLOPS | ZFLOPS |  10<sup>21</sup> |


### Benchmarks

The main benchmark used for the Top500 list is the *High Performance LINPACK* ([HPL](https://www.netlib.org/benchmark/hpl/)) test and is based on a variant of *LU* factorization with row partial pivoting. The main critism is that it is not representative of many important applications.

A new benchmark, called the *High Performance Conjugate Gradients* ([HPCG](https://www.hpcg-benchmark.org)) is designed to exercise computational and data access pattern that more closely match a broader set of important applications.