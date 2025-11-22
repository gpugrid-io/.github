# Gpugrid

GpuGrid enables users to easily run containerized AI workloads on a decentralized GPU network, where anyone can get paid by connecting compute nodes to the network and running container jobs. Users can easily run jobs such as Stable Diffusion XL and cutting-edge open source LLMs, supporting on-chain execution, CLI execution, and execution via [GpuGrid AI Studio](https://app.gpugrid.io) on the web.

Visit the [GpuGrid documentation](https://docs.gpugrid.io/) site for a more comprehensive getting started overview, including the [Quick Start Guide](https://docs.gpugrid.io/quickstart).

## Getting Started Running Container Jobs on GpuGrid

Jobs (containers) can be run on GpuGrid using the [installable CLI](https://docs.gpugrid.io/cli), or installed via the [Go toolchain](https://docs.gpugrid.io/cligo). After setting up the necessary prerequisites, the CLI enables users to run jobs as follows:

``
grid run cowsay:v0.0.4 -i Message="moo"
``

The current list of modules can be found in the following repositories:

* [gridsay](https://github.com/gpugrid-io/gpugrid-module-lilysay)
* [cowsay](https://github.com/gpugrid-io/gpugrid-module-cowsay)
* [Stable Diffusion XL](https://github.com/gpugrid-io/gpugrid-module-sdxl-pipeline/)
* [Stable Diffusion Video](https://github.com/gpugrid-io/gpugrid-module-sdv-pipeline)
* [wasm](https://github.com/gpugrid-io/gpugrid-module-wasm)

Containerized job modules can be built and added to the available module list; more details can be found in the [Building Jobs](https://docs.gpugrid.io/building) documentation. If you'd like to contribute, please open a pull request on this repository to add your link to the list above.

## Getting Started Running Nodes on the GpuGrid Network

As a distributed network, GpuGrid also brings the ability to run as a node and contribute GPU and compute power. See the [Running Nodes](https://docs.gpugrid.io/node) documentation for more detailed instructions and an overview of the setup.

## Performance

We benchmark the solver job matching algorithm at: https://gpugrid-io.github.io/gpugrid/dev/bench/. More details can be found in our [Benchmarking Guide](./LOCAL_DEVELOPMENT.md#benchmarks).
