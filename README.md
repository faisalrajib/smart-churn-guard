# Smart Churn Guard 🔮
**End-to-end customer churn prediction platform on Google Vertex AI – fully automated MLOps**

![Pipeline](screenshots/pipeline.png)
**Live model endpoint serving <100ms predictions with drift detection**

### 🏆 Results
| Model                  | AUC   | Training time | Cost    |
|-----------------------|-------|---------------|---------|
| Vertex AutoML         | 0.854 | 1 hour        | ~$9     |
| Custom XGBoost + TF   | **0.881** | 23 min (HPT) | ~$4     |

### Architecture
![Architecture](screenshots/architecture.png)

### Features Shown
- Vertex AI Feature Store • AutoML • Custom Training • Hyperparameter Tuning
- Vertex AI Pipelines (Kubeflow) • Explainable AI • Model Monitoring
- Terraform IaC • GitHub Actions CI/CD • Online + Batch Prediction

### Quick Start
```bash
# 1. Clone & authenticate
git clone https://github.com/faisalrajib/smart-churn-guard.git
gcloud auth login

# 2. Deploy everything with Terraform
cd terraform && terraform apply

# 3. Trigger pipeline (or let GitHub Actions do it on push)
python -m pipelines.churn_pipeline
