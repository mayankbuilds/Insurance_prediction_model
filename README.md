# Insurance Premium Category Predictor

A full-stack machine learning web application that predicts a user's insurance premium category based on demographic, lifestyle, and financial details. The application features a robust backend powered by **FastAPI** and an intuitive, interactive frontend built with **Streamlit**. 

The project uses `uv` for lightning-fast Python package and environment management.

---

## 🚀 Features

- **FastAPI Backend:** High-performance, production-ready REST API layout with structured data validation using Pydantic.
- **Streamlit Frontend:** A clean web dashboard for inputting user attributes and displaying dynamic prediction status.
- **Modular Pipeline:** Dedicated directory layers for schemas, utility configs, and model inference logic.
- **Health Checks:** Built-in API endpoints (`/health`) to monitor active server and model version statuses.

---

## 📁 Project Structure

```text
├── config/
│   └── city_tier.py          # Configuration and utility helpers
├── model/
│   ├── model.pkl             # Trained Machine Learning serialized model
│   └── predict.py            # Inference logic execution script
├── schema/
│   └── user_input.py         # Pydantic schema schemas for API requests
├── fastapi_ml_model.ipynb    # Jupyter Notebook for experimental model training
├── frontend.py               # Streamlit web application file
├── insurance.csv             # Raw dataset used for model training
├── main.py                   # FastAPI server entry point
├── pyproject.toml            # Project configuration managed by uv
├── requirements.txt          # Exported pip dependencies configuration
└── uv.lock                   # Deterministic lockfile for dependencies