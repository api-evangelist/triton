# Triton Inference Server

NVIDIA Triton Inference Server provides a cloud and edge inferencing solution optimized for both CPUs and GPUs. Triton implements the KServe V2 inference protocol via HTTP/REST and gRPC, supporting TensorRT, TensorFlow, PyTorch, ONNX Runtime, Python, and more backends.

**GitHub:** [https://github.com/triton-inference-server/server](https://github.com/triton-inference-server/server)
**Documentation:** [https://docs.nvidia.com/deeplearning/triton-inference-server/](https://docs.nvidia.com/deeplearning/triton-inference-server/)

---

## APIs

### Triton HTTP/REST API
RESTful KServe V2 protocol API for model inference, health checks, metadata queries, model repository management, statistics, tracing, and logging.

- **Documentation:** [Protocol Docs](https://github.com/triton-inference-server/server/blob/main/docs/protocol/extension_binary_data.md)
- **OpenAPI:** [openapi/triton-http-rest-openapi.yml](openapi/triton-http-rest-openapi.yml)

### Triton gRPC API
High-performance gRPC inference API with streaming and binary tensor data support.

- **Documentation:** [Protocol README](https://github.com/triton-inference-server/server/blob/main/docs/protocol/README.md)
- **Protocol Buffers:** [grpc_service.proto](https://github.com/triton-inference-server/common/blob/main/protobuf/grpc_service.proto)

### Triton Metrics API
Prometheus-compatible metrics for monitoring inference throughput, GPU utilization, memory, and latency.

- **Documentation:** [Metrics Guide](https://github.com/triton-inference-server/server/blob/main/docs/user_guide/metrics.md)
- **OpenAPI:** [openapi/triton-metrics-openapi.yml](openapi/triton-metrics-openapi.yml)

---

## Artifacts

### OpenAPI Specifications
| Spec | Description |
|---|---|
| [triton-http-rest-openapi.yml](openapi/triton-http-rest-openapi.yml) | HTTP/REST KServe V2 inference and management API |
| [triton-metrics-openapi.yml](openapi/triton-metrics-openapi.yml) | Prometheus metrics endpoint |

### JSON Schemas
| Schema | Description |
|---|---|
| [triton-model-schema.json](json-schema/triton-model-schema.json) | Triton model configuration (config.pbtxt structure) |
| [triton-inference-request-schema.json](json-schema/triton-inference-request-schema.json) | Inference request payload |
| [triton-inference-response-schema.json](json-schema/triton-inference-response-schema.json) | Inference response payload |

### JSON Structure
| File | Description |
|---|---|
| [triton-model-structure.json](json-structure/triton-model-structure.json) | Structure documentation for model and inference objects |

### JSON-LD Context
| File | Description |
|---|---|
| [triton-context.jsonld](json-ld/triton-context.jsonld) | Linked data context for Triton vocabulary |

### Spectral Rules
| Ruleset | Description |
|---|---|
| [triton-rules.yml](rules/triton-rules.yml) | API linting rules for Triton KServe V2 conventions |

### Naftiko Capabilities
| Capability | Description |
|---|---|
| [model-inference.yaml](capabilities/model-inference.yaml) | Model lifecycle management and inference workflow |

**Shared Definitions:**
| File | Description |
|---|---|
| [shared/triton-http-rest.yaml](capabilities/shared/triton-http-rest.yaml) | Triton HTTP/REST API consumed definition |

### Examples
| Example | Description |
|---|---|
| [triton-model-infer-example.json](examples/triton-model-infer-example.json) | ResNet-50 image classification inference |
| [triton-repository-index-example.json](examples/triton-repository-index-example.json) | List all models in repository |

### Vocabulary
| File | Description |
|---|---|
| [triton-vocabulary.yml](vocabulary/triton-vocabulary.yml) | Domain vocabulary for Triton inference concepts |

---

## Common Resources

- **GitHub Org:** [https://github.com/triton-inference-server](https://github.com/triton-inference-server)
- **Getting Started:** [Quickstart Guide](https://github.com/triton-inference-server/server/blob/main/docs/getting_started/quickstart.md)
- **Client Libraries:** [Python, C++, Java](https://github.com/triton-inference-server/client)
- **Docker Images:** [NGC Container Catalog](https://catalog.ngc.nvidia.com/orgs/nvidia/containers/tritonserver)
- **PyTriton:** [https://github.com/triton-inference-server/pytriton](https://github.com/triton-inference-server/pytriton)
- **Model Analyzer:** [https://github.com/triton-inference-server/model_analyzer](https://github.com/triton-inference-server/model_analyzer)
- **Community:** [GitHub Discussions](https://github.com/triton-inference-server/server/discussions)

---

*Profiled: 2026-05*
