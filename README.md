# Triton Inference Server (triton)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
