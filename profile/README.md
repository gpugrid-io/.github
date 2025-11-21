
# GpuGrid

GpuGrid 使用户能够轻松在去中心化的 GPU 网络中运行容器化的 AI 工作负载，任何人都可以通过将计算节点连接到网络并运行容器作业来获得报酬。用户可以轻松运行 Stable Diffusion XL 和前沿开源 LLM 等作业，支持链上运行、CLI 运行以及通过网页上的 [GpuGrid AI Studio](https://app.gpugrid.io) 运行。

访问 [GpuGrid 文档](https://docs.gpugrid.io/) 站点获取更全面的入门概述，包括 [快速入门指南](https://docs.gpugrid.io/quickstart)

## 开始在 GpuGrid 上运行容器作业

可以通过使用 [可安装 CLI](https://docs.gpugrid.io/cli) 在 GpuGrid 上运行作业（容器），也可以通过 [Go 工具链](https://docs.gpugrid.io/cligo) 进行安装。设置必要的先决条件后，CLI 使用户能够按如下方式运行作业：

```
gpugrid run cowsay:v0.0.4 -i Message="moo"
```

当前模块列表可以在以下仓库中找到：

* [gridsay](https://github.com/gpugrid-io/gpugrid-module-lilysay)
* [cowsay](https://github.com/gpugrid-io/gpugrid-module-cowsay)
* [Stable Diffusion XL](https://github.com/gpugrid-io/gpugrid-module-sdxl-pipeline/)
* [Stable Diffusion Video](https://github.com/gpugrid-io/gpugrid-module-sdv-pipeline)
* [wasm](https://github.com/gpugrid-io/gpugrid-module-wasm)

可以构建容器化作业模块并添加到可用模块列表中；更多详情请访问 [构建作业](https://docs.gpugrid.io/building) 文档。如果您想贡献，请在此仓库上开启拉取请求，将您的链接添加到上面的列表中。

## 开始在 GpuGrid 网络上运行节点

作为一个分布式网络，GpuGrid 还带来了作为节点运行并为 GPU 和计算能力做贡献的能力。请参阅 [运行节点](https://docs.gpugrid.io/node) 文档，其中包含更多设置的详细说明和概述。

## 性能

我们对求解器作业匹配算法进行基准测试：https://gpugrid-io.github.io/gpugrid/dev/bench/。更多详情请参见我们的 [基准测试指南](./LOCAL_DEVELOPMENT.md#benchmarks)。
