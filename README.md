# smart-churn-guard
smart-churn-guard/
├── README.md                     ← Your portfolio star
├── data/
│   └── telco-churn.csv           ← Famous public dataset
├── notebooks/
│   └── 01_eda_and_experiments.ipynb
├── src/
│   ├── preprocess.py
│   ├── trainer/
│   │   ├── task.py              ← Custom training (XGBoost + TF)
│   │   └── model.py
│   └── pipelines/
│       └── churn_pipeline.py    ← Kubeflow pipeline
├── terraform/                    ← Infra as Code (optional but gold)
├── .github/workflows/
│   └── vertex-deploy.yml         ← GitHub Actions CI/CD
├── requirements.txt
├── setup.py
└── kfp_components/               ← Reusable pipeline components
