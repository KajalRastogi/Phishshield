# PhishShield - AI Phishing Email Detector (Full Edition)

## Quick start

1. Create & activate virtual environment
   - Windows (PowerShell):
     ```powershell
     python -m venv venv
     .\venv\Scripts\activate
     ```
   - macOS / Linux:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create sample data (if you don't have data/emails_sample.csv):
   ```bash
   python create_sample_data.py
   ```

4. Train fallback model:
   ```bash
   python train_fallback.py
   ```

5. Run Flask API:
   ```bash
   python api/flask_api.py
   ```

6. Test API:
   ```bash
   python test_api.py
   ```

7. Run Streamlit UI (in another terminal):
   ```bash
   streamlit run app/streamlit_app.py
   ```

8. (Optional) Load `chrome_ext/` in Chrome (Developer mode -> Load unpacked) to test the extension UI.

## Files included
- create_sample_data.py
- model_utils.py
- train_fallback.py
- app/streamlit_app.py
- api/flask_api.py
- test_api.py
- chrome_ext/* (manifest, popup.html, popup.js)
- requirements.txt
