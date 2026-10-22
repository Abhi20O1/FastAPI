# FastAPI Machine-Learning APIs

A learning project that combines FastAPI, Pydantic validation, scikit-learn inference, and JSON-backed patient operations.

## Included examples

- `FastAPI/app.py` — insurance-premium category prediction endpoint using a serialized scikit-learn model.
- `FastAPI/main.py` — patient management API with create, view, update, and sorting routes.
- `FastAPI/frontend.py` — Streamlit client for the prediction example.
- `FastAPI/fastapi-ml-model.ipynb` — model preparation and evaluation notebook.

## API examples

Run the patient API from the `FastAPI/` directory:

```bash
pip install fastapi uvicorn pydantic pandas scikit-learn
uvicorn main:app --reload
```

Open the generated API documentation at `http://127.0.0.1:8000/docs`.

## Notes

The bundled datasets and serialized model are demonstration assets. Do not use the example patient data or model for real medical or insurance decisions. For a production deployment, add authentication, secrets management, tests, structured logging, and model/version validation.
