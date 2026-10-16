# Awesome-Cloud-ML-APIS

## Top Cloud ML APIs Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Serverless Model Serving, GPU Inference & Production Deployment*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud ML APIs**. These tools enable developers to run machine learning models in the cloud via API—from serverless GPU platforms that scale to zero to managed inference services that abstract away infrastructure entirely.



**Examples** include AWS SageMaker Endpoints, Google Vertex AI Endpoints, Azure ML Endpoints, BentoML, Modal, Anyscale, Together AI, Replicate, RunPod, and Baseten (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, model serving, and open inference infrastructure—ideal for ML engineers, backend developers, and organizations seeking transparent, vendor-independent model serving.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Replicate](https://replicate.com/)**  

  **Run machine learning models in the cloud via API** . **The most developer-friendly model hosting platform**—**thousands of open-source models** ready to run with a single API call . **Features**: **hosted models** (no deployment required), **custom model deployment** via Cog, **automatic scaling**, **pay-per-second billing**, and **Python/JavaScript SDKs** . **Used by 1.5M+ developers** for image generation, video processing, text-to-speech, and LLM inference . **The fastest path from model to API** .



- **[AWS SageMaker Endpoints](https://aws.amazon.com/sagemaker/)**  

  **Fully managed ML inference service** . Features **real-time endpoints**, **serverless inference**, **asynchronous inference**, and **batch transform** . **Deep AWS ecosystem integration** with IAM, VPC, and CloudWatch . **The enterprise standard** for AWS-native ML deployment .



- **[Google Vertex AI Endpoints](https://cloud.google.com/vertex-ai)**  

  **Google Cloud's unified ML platform** with **online prediction**, **batch prediction**, and **model monitoring** . Features **custom containers**, **pre-built containers**, and **Model Garden** for foundation models . **The most integrated with Gemini and Google Cloud ecosystem** .



- **[Azure ML Endpoints](https://azure.microsoft.com/en-us/products/machine-learning/)**  

  **Microsoft's managed ML endpoint service** with **online and batch endpoints** . Features **MLflow integration**, **responsible AI dashboards**, and **managed online endpoints** with autoscaling . **The best choice for Microsoft-centric organizations** .



- **[Modal](https://modal.com/)**  

  **Serverless GPU platform with native GPU support** (A10G, A100, H100) . **Scales to 50,000+ concurrent containers** . **Python-first API with sub-second cold starts** . **Sandbox workloads priced at ~$0.14/vCPU-hour** . **Best for**: bursty, Python-native workloads that can return to zero without violating UX .



- **[Anyscale](https://www.anyscale.com/)**  

  **Managed Ray platform for distributed AI workloads** . **Python-native `@ray.remote` decorator distributes functions across clusters** without Kubernetes expertise . **Enterprise adds monitoring, logging, and security** on top of open-source Ray . **Best for**: distributed training and inference at scale .



- **[Together AI](https://www.together.ai/)**  

  **Full-stack generative AI platform** with managed inference for open models . **Instant deployment**, **auto-scaling**, and **pay-per-token pricing** for inference . **The best choice for open-model inference without GPU management** .



- **[RunPod](https://www.runpod.io/)**  

  **GPU cloud with serverless endpoints, pods, and secure cloud options** . **Instant deployment**, **per-second billing**, and **community cloud pricing** . **The most affordable GPU cloud** for developers .



- **[Baseten](https://baseten.co/)**  

  **ML infrastructure platform for model deployment** . **Truss for model packaging** and **autoscaling inference** . **The most focused on production model serving** with observability and performance .



## Open-Source GitHub Projects



- **[BentoML](https://github.com/bentoml/BentoML)**  

  **The most flexible open-source model serving framework** (Apache-2.0) . **18,000+ GitHub stars** . **Packages models, dependencies, and inference logic into standardized Bentos** deployable anywhere . **Features**: **adaptive micro-batching**, **multi-model serving**, **OpenAI-compatible API**, and **one-click deployment** to AWS, Azure, GCP, and Kubernetes . **BentoML thinks in Docker containers**—the best choice when you own the containerization layer . **The reference implementation for self-hosted model serving** .



- **[Ray Serve](https://github.com/ray-project/ray)**  

  **Model serving built on Ray** (Apache-2.0) . **Best when you already have a Ray cluster** and want to share compute between training and serving . **Features**: **autoscaling**, **multi-model composition**, **traffic splitting**, and **model multiplexing** . **Note**: Requires a persistent cluster—even at idle, you pay . **Ray Serve thinks in distributed computing** .



- **[KServe](https://github.com/kserve/kserve)**  

  **Standardized Serverless ML Inference Platform on Kubernetes** (Apache-2.0) . **The CNCF standard for Kubernetes-native model serving** . **Features**: **serverless inference** via Knative, **canary rollouts**, **transformer pipelines**, **model explainability**, and **multi-framework support** (TensorFlow, PyTorch, ONNX, XGBoost, scikit-learn) . **The best choice for Kubernetes-native ML platforms** .



- **[vLLM](https://github.com/vllm-project/vllm)**  

  **The production default for high-concurrency LLM serving** (Apache-2.0) . **PagedAttention** for efficient KV cache management, **continuous batching** for throughput, and **prefill/decode disaggregation** for optimized resource allocation . **The most widely deployed open-source inference engine** for LLMs .



- **[SGLang](https://github.com/sgl-project/sglang)**  

  **The fastest engine for chat, agents, and structured generation** (Apache-2.0) . **RadixAttention** organizes KV cache as a radix tree enabling **variable-length prefix sharing** . **Native structured generation** integrated at the scheduling layer . **The best choice for agent and structured-output workloads** .



- **[Triton Inference Server](https://github.com/triton-inference-server/server)**  

  **NVIDIA's open-source inference serving software** (BSD-3-Clause) . **The most comprehensive multi-framework serving engine**—supports TensorRT, PyTorch, TensorFlow, ONNX, OpenVINO, and Python backends . **Features**: **dynamic batching**, **concurrent model execution**, **model ensembles**, and **GPU/CPU inference** . **The enterprise standard for NVIDIA-based inference** .



- **[Text Embeddings Inference (TEI)](https://github.com/huggingface/text-embeddings-inference)**  

  **Hugging Face's high-performance text embeddings inference toolkit** (Apache-2.0) . **The fastest path to deploying embedding models**—supports BGE, E5, GTE, and other popular embedding models . **Features**: **dynamic batching**, **token-based routing**, **Flash Attention**, and **ONNX support** .



- **[OpenLLM](https://github.com/bentoml/OpenLLM)**  

  **Run open-source LLMs in production with OpenAI-compatible API** (Apache-2.0) . **`openllm start llama2 --backend vllm`** —the simplest path to self-hosted LLM serving .



- **[Cog](https://github.com/replicate/cog)**  

  **Containers for machine learning** (Apache-2.0) . **The packaging standard behind Replicate**—define your model's environment in a `cog.yaml`, build a Docker image, and push . **The most portable model packaging format** for cloud deployment .



- **[Ollama](https://github.com/ollama/ollama)**  

  **Get up and running with Llama 3, Mistral, and other large language models** (MIT) . **The simplest local LLM runner**—one command to run any supported model . **The best choice for local development and edge deployment** .



- **[LocalAI](https://github.com/mudler/LocalAI)**  

  **OpenAI-compatible API for local inference** (MIT) . **Drop-in replacement for OpenAI API** running on consumer hardware . **The most accessible local inference platform** .



### Additional Strong Open-Source Options



- **[LitServe](https://github.com/Lightning-AI/LitServe)** — Minimal Python framework for AI inference servers (Apache-2.0) . **The lightest-weight open-source serving framework** for custom inference endpoints .

- **[Xinference](https://github.com/xorbitsai/inference)** — Unified, production-ready inference for text, speech, and multimodal models (Apache-2.0) .

- **[TorchServe](https://github.com/pytorch/serve)** — PyTorch model serving (Apache-2.0) . **The official PyTorch serving framework** .

- **[TensorFlow Serving](https://github.com/tensorflow/serving)** — TensorFlow model serving (Apache-2.0) . **The original production serving system** .

- **[ONNX Runtime](https://github.com/microsoft/onnxruntime)** — Cross-platform inference engine (MIT) . **The standard for optimized model deployment** .

- **[TensorRT](https://github.com/NVIDIA/TensorRT)** — NVIDIA's SDK for high-performance deep learning inference (Apache-2.0) .

- **[MLflow Models](https://github.com/mlflow/mlflow)** — Model packaging and serving (Apache-2.0) . **The standard for ML lifecycle management** .

- **[Ray](https://github.com/ray-project/ray)** — Distributed computing framework (Apache-2.0) . **The foundation for Ray Serve and distributed inference** .

- **[LangServe](https://github.com/langchain-ai/langserve)** — Deploy LangChain applications as REST APIs (MIT) .

- Community **n8n** workflows for model deployment automation and inference alerting.



**Frameworks for building custom systems**: Combine **BentoML** for flexible model packaging with **KServe** for Kubernetes-native serving, **vLLM** or **SGLang** for LLM inference, **Triton** for multi-framework serving, and **Ray Serve** for distributed inference—creating a fully self-hosted, enterprise-grade model serving platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud ML API platforms handling model inputs and outputs must comply with data protection regulations (GDPR, CCPA, etc.) and model provider terms of service.

- **Open-source model serving is mature and production-ready.** BentoML packages models for any deployment target . KServe is the CNCF standard for Kubernetes-native serving . vLLM and SGLang lead LLM inference performance . **These are genuine alternatives to commercial platforms.**

- **BentoML vs Ray Serve: pick based on your stack.** BentoML thinks in Docker containers and scales to zero via serverless . Ray Serve thinks in distributed computing and requires a persistent cluster . **Pick BentoML if you own containerization; pick Ray Serve if you're already knee-deep in Ray** .

- **Serverless vs. persistent infrastructure is a cost decision.** Modal, RunPod, and Replicate scale to zero—you pay only for execution . Ray Serve and traditional Kubernetes serving require persistent infrastructure—idle capacity costs money . **Match the platform to your workload's traffic pattern.**

- **Model packaging matters for portability.** Cog's container-based packaging is portable across clouds . BentoML's Bentos are portable across deployment targets . **Avoid vendor-specific packaging that locks you into one platform.**

- Self-hosted open-source solutions require proper GPU provisioning, model management, and ongoing maintenance. **Inference platforms are performance-critical infrastructure**—benchmark against your specific workload before production deployment.



---



**Made for ML engineers, backend developers, and organizations building transparent model serving solutions.**  

Let's make Cloud ML APIs more open, data-driven, and serverless.
