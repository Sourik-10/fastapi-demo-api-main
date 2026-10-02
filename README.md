# FastAPI + ML Deployment — Learning Practice

Followed [CampusX's FastAPI tutorial series](https://www.youtube.com/@campusx-official)
to learn how to serve an ML model through a FastAPI backend with a Streamlit
frontend. This is a practice/learning repo, not an original project — built
to understand:

- Pydantic data validation + `@computed_field` for server-side feature engineering
- Serving a trained scikit-learn model via a `/predict` endpoint
- Connecting a Streamlit frontend to a FastAPI backend
- Basic CRUD API design (`main.py` — patient management demo)

## What's here

| File | Purpose |
|---|---|
| `app.py` | Insurance premium prediction API (synthetic dataset) |
| `frontend.py` | Streamlit UI that calls `app.py` |
| `main.py` | Separate CRUD API practice (patient records) |
| `fastapi_ml_model.ipynb` | Model training notebook |

## Run locally

```bash
pip install -r requirements.txt
uvicorn app:app --reload
streamlit run frontend.py
```
