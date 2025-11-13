# Graphene Optimizer

Simple Streamlit app + XGBoost models to predict yield and Raman I_D/I_G from biomass carbonization & catalytic graphitization parameters.

## Quick start (local)

1. Create and activate venv:
   - python -m venv venv
   - Windows: venv\Scripts\activate
   - macOS/Linux: source venv/bin/activate

2. Install:
   - pip install -r requirements.txt

3. Train models (uses data/runs.csv):
   - python model/train_model.py

4. Run Streamlit app:
   - streamlit run app/dashboard.py

## Deployment (Streamlit Cloud)
1. Create a GitHub repo, push all files.
2. Sign into https://streamlit.io/cloud and link the repo.
3. Set the app path to `app/dashboard.py`. Deploy.

## Notes
- Replace `data/runs.csv` with your real experiment logs (keep header).
- Retrain models after adding measured outputs (run_id rows with real yield/raman).