# Triton Inference Server (triton)

NVIDIA Triton Inference Server provides a cloud and edge inferencing solution optimized for both CPUs and GPUs. Triton supports an HTTP/REST and gRPC protocol that allows remote clients to request inferencing for any model being managed by the server. Open source and part of the broader NVIDIA AI ecosystem, Triton implements the KServe V2 inference protocol supporting TensorRT, TensorFlow, PyTorch, ONNX Runtime, Python, and more backends.

**APIs.json:** [https://github.com/triton-inference-server/server](https://github.com/triton-inference-server/server)

## Tags

- AI
- Deep Learning
- Inference
- Machine Learning
- Model Serving
- NVIDIA
- Open Source

## Timestamps

- **Created:** 2024-01-15
- **Modified:** 2026-05-19

## APIs

### Triton HTTP/REST API

RESTful API implementing the KServe V2 inference protocol for model inference, health checks, metadata queries, model repository management, statistics, tracing, and logging.

- **Human URL:** [https://github.com/triton-inference-server/server/blob/main/docs/protocol/extension_binary_data.md](https://github.com/triton-inference-server/server/blob/main/docs/protocol/extension_binary_data.md)
- **Base URL:** `http://localhost:8000`

#### Tags

- HTTP
- Inference
- Model Management
- REST
- KServe

#### Properties

- [Documentation](https://github.com/triton-inference-server/server/blob/main/docs/protocol/extension_binary_data.md)
- [OpenAPI](https://github.com/triton-inference-server/server/blob/main/docs/protocol/rest_api.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman  Collection](https://www.postman.com/nvidia-triton)
- [OpenAPI](openapi/triton-http-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/triton-http-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/triton-http-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Triton GRPC API

High-performance gRPC API for model inference with support for streaming and binary tensor data.

- **Human URL:** [https://github.com/triton-inference-server/server/blob/main/docs/protocol/README.md](https://github.com/triton-inference-server/server/blob/main/docs/protocol/README.md)
- **Base URL:** `grpc://localhost:8001`

#### Tags

- GRPC
- High Performance
- Inference
- Streaming

#### Properties

- [Documentation](https://github.com/triton-inference-server/server/blob/main/docs/protocol/README.md)
- [Protocol  Buffers](https://github.com/triton-inference-server/common/blob/main/protobuf/grpc_service.proto)
- [Examples](https://github.com/triton-inference-server/client/tree/main/src/python/examples)
- [Postman Collection](collections/triton-http-rest.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/triton-http-rest.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/triton-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/triton-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Triton Metrics API

Prometheus-compatible metrics API for monitoring server and model performance including inference request counts, latencies, GPU utilization, and memory usage.

- **Human URL:** [https://github.com/triton-inference-server/server/blob/main/docs/user_guide/metrics.md](https://github.com/triton-inference-server/server/blob/main/docs/user_guide/metrics.md)
- **Base URL:** `http://localhost:8002/metrics`

#### Tags

- Metrics
- Monitoring
- Observability
- Prometheus

#### Properties

- [Documentation](https://github.com/triton-inference-server/server/blob/main/docs/user_guide/metrics.md)
- [Metrics  Format](https://prometheus.io/docs/instrumenting/exposition_formats/)
- [OpenAPI](openapi/triton-metrics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/triton-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/triton-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Repository](https://github.com/triton-inference-server/server)
- [Documentation](https://docs.nvidia.com/deeplearning/triton-inference-server/)
- [Getting Started](https://github.com/triton-inference-server/server/blob/main/docs/getting_started/quickstart.md)
- [Client  Libraries](https://github.com/triton-inference-server/client)
- [Model  Repository](https://github.com/triton-inference-server/server/blob/main/docs/user_guide/model_repository.md)
- [Supported  Backends](https://github.com/triton-inference-server/backend)
- [Docker  Images](https://catalog.ngc.nvidia.com/orgs/nvidia/containers/tritonserver)
- [Community  Forum](https://github.com/triton-inference-server/server/discussions)
- [Release Notes](https://github.com/triton-inference-server/server/releases)
- [Py Triton](https://github.com/triton-inference-server/pytriton)
- [Model  Analyzer](https://github.com/triton-inference-server/model_analyzer)
- [Triton  C L I](https://github.com/triton-inference-server/triton_cli)
- [OpenAPI](openapi/triton-http-rest-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/triton-metrics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON-LD](json-ld/triton-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/triton-model-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/triton-inference-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/triton-inference-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [J S O N  Structure](json-structure/triton-model-structure.json)
- [Spectral  Rules](rules/triton-rules.yml)
- [Vocabulary](vocabulary/triton-vocabulary.yml)
- [x-profiled](2026-05)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
