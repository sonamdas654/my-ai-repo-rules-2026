# AI ki knowledge me rakho
# My AI Repo Rules 2026
# Master Rulebook
# Har nayi chat mein yeh file MANDATORY read ki jayegi.

---

## Rule 1 — Deep Learning Framework
- **PyTorch** (pytorch/pytorch) — hamesha use karo naye projects ke liye.
- TensorFlow — sirf legacy projects mein. Naye projects mein AVOID.

## Rule 2 — LLM Inference & Serving
- **vLLM** (vllm-project/vllm) — production serving ke liye BEST choice.
- Hugging Face Transformers (huggingface/transformers) — fine-tuning aur model access ke liye.

## Rule 3 — RAG & Agentic Workflows
- **LlamaIndex** (run-llama/llama_index) — data connectors ke liye better.
- **LangChain** (langchain-ai/langchain) — complex chains ke liye better.
- Dono use kar sakte ho use-case ke hisaab se.

## Rule 4 — Computer Vision
- **OpenCV** (opencv/opencv) — basics ke liye.
- **Ultralytics YOLO** (ultralytics/ultralytics) — object detection ke liye.
- Detectron2 (facebookresearch/detectron2) — INACTIVE hai, use mat karo.

## Rule 5 — Data Processing
- **Pandas** (pandas-dev/pandas) — standard data processing.
- **Apache Arrow** (apache/arrow) — columnar data ke liye.
- **Apache Spark** (apache/spark) — large scale distributed processing ke liye.

## Rule 6 — Vector Databases
- **Milvus** (milvus-io/milvus) — production scale ke liye.
- **Qdrant** (qdrant/qdrant) — high performance ke liye.
- **Chroma** (chroma-core/chroma) — prototyping ke liye sirf.
- FAISS (facebookresearch/faiss) — similarity search ke liye.

## Rule 7 — ML Lifecycle Management
- **MLflow** (mlflow/mlflow) — tracking aur model registry ke liye.
- **DVC** (iterative/dvc) — data versioning ke liye.
- **Ray** (ray-project/ray) — distributed compute ke liye.

## Rule 8 — Workflow Orchestration
- **Apache Airflow** (apache/airflow) — complex DAGs ke liye.
- **Prefect** (PrefectHQ/prefect) — dynamic workflows ke liye.
- **Dagster** (dagster-io/dagster) — data assets ke liye.

## Rule 9 — Model Serving & Deployment
- **Kubernetes** (kubernetes/kubernetes) — container orchestration.
- **KServe** (kserve/kserve) — inference on K8s.
- **BentoML** (bentoml/BentoML) — quick serving ke liye.
- **Triton Inference Server** (triton-inference-server/server) — NVIDIA GPU ke liye.

## Rule 10 — Web APIs
- **FastAPI** (fastapi/fastapi) — har naye web API ke liye FIRST choice.
- Django (django/django) — full-stack web apps ke liye.
- Flask (pallets/flask) — simple microservices ke liye.

## Rule 11 — Monitoring & Observability
- **Prometheus** (prometheus/prometheus) — metrics ke liye.
- **OpenTelemetry** (open-telemetry/opentelemetry-collector) — telemetry ke liye.
- **Langfuse** (langfuse/langfuse) — LLM observability ke liye.
- **Weights & Biases** (wandb/wandb) — experiment tracking ke liye.

## Rule 12 — LLM Evaluation
- **EleutherAI LM Evaluation Harness** (EleutherAI/lm-evaluation-harness) — benchmarks ke liye.
- **DeepEval** (confident-ai/deepeval) — unit testing ke liye.

## Rule 13 — Optimization
- **ONNX Runtime** (microsoft/onnxruntime) — cross-platform inference.
- **TensorRT** (NVIDIA/TensorRT) — NVIDIA GPU optimization.
- **JAX** (google/jax) — TPU/GPU research.

## Rule 14 — Multi-Agent Systems
- **Microsoft Agent Framework** (microsoft/autogen + microsoft/semantic-kernel merged) — primary choice.
- **CrewAI** (crewAIInc/crewAI) — role-playing agents ke liye.

## Rule 15 — DEPRECATED / HIGH RISK — AVOID
| Repo | Reason |
|------|--------|
| docker/docker-ce | Deprecated — use moby/moby |
| Significant-Gravitas/AutoGPT | Sirf prototype, production mein NEVER |
| imartinez/privateGPT | Security risks — AVOID |
| zilliztech/GPTCache | Slow development — AVOID |
| horovod/horovod | PyTorch DDP use karo instead |

## Rule 16 — Task Decision Making
- Jab bhi koi task do, in rules ke hisaab se tool choose karo.
- Tool decide karte waqt REASON batana mandatory hai.
- Agar task CRITICAL ho toh pehle approval lo.

## Rule 17 — Priority Order
Rule 1 sabse zyaada important. Rule 16 se upar ki priority descending order mein hai.

## Rule 18 — Fallback Strategy
- vLLM fail ho → Hugging Face TGI try karo.
- TGI bhi fail ho → User ko batao, manual intervention lo.

## Rule 19 — SAFETY (CRITICAL)
❌ KABHI NAHI chalana:
- `rm -rf /`
- `DROP DATABASE`
- `DELETE FROM table WHERE 1=1`
- Agar aisa karna ho toh EXPLICIT USER APPROVAL MANDATORY.

## Rule 20 — Haystack
- deepset-ai/haystack — SIRF tab use karo jab LangChain/LlamaIndex fit na ho. Warna avoid.

## Rule 21 — NLP
- **spaCy** (explosion/spaCy) — production-grade NLP ke liye: tokenization, NER, text preprocessing.

## Rule 22 — ML Pipelines on K8s
- **Kubeflow** (kubeflow/kubeflow) — full ML pipeline on Kubernetes. Heavy hai, chhoti teams AVOID karein.

## Rule 23 — Hybrid Vector Search
- **Weaviate** (weaviate/weaviate) — hybrid search ke liye. Sirf tab use karo jab Milvus/Qdrant requirements na poori karein.

## Rule 24 — Ready-Made RAG Apps
- AnythingLLM (Mintplex-Labs/anything-llm) — ready-made RAG, production custom development ke liye AVOID.

## Rule 25 — Alternative Inference Serving
- **Seldon Core** (SeldonIO/seldon-core) — sirf tab use karo jab KServe support na kare.

## Rule 26 — Parallel Computing
- **Dask** (dask/dask) — out-of-core pandas aur parallel computing ke liye. Use karo agar Ray overkill lage.

---
*Last Updated: 2026-04-19*
*Owner: sonamdas654
