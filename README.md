## EGraph

EGraph can be integrated into the existing GPU-accelerated graph processing systems to efficiently support concurrent execution of TGP jobs on large-scale dynamic graphs with the help of GPU accelerators.

#### Graph formats

EGraph accepts the binary serialized pre-built CSR graph representation. Reading binary formats is faster and more space efficient.

#### Compilation

To compile EGraph, just run make in the root directory. The only requrements are g++ and CUDA toolkit.

#### Running applications in EGraph

The applications take a graph as input as well as some optional arguments. For example:

```
$ ./sssp-TGP --input path-to-input-graph
$ ./sssp-TGP --input path-to-input-graph --source 10