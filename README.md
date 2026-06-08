# MindCheck AI

Professional Flask web application for a mental health prediction project.

## What is included

- Flask backend with clean routes
- Dark responsive UI using Bootstrap, custom CSS, and JavaScript
- Survey page with MCQs, sliders, text input, and progress tracking
- Random Forest ML prediction with a cached pickle model
- Result page with prediction, confidence, suggestions, and Chart.js visualizations
- SQLite login/signup and saved assessment dashboard
- Help/resources page and basic wellbeing chatbot

## Project structure

```text
mindcheck_v3/
  app.py
  requirements.txt
  survey.csv
  Mental_Health_Dataset.csv
  models/
    mindcheck_model.pkl        # created automatically on first run
  instance/
    mindcheck.sqlite3          # created automatically
  static/
    css/styles.css
    js/app.js
  templates/
    base.html
    index.html
    survey.html
    result.html
    about.html
    contact.html
    auth.html
    dashboard.html
```

## Run locally

```bash
pip install -r requirements.txt
python app.py
```

Open:

```text
http://localhost:5000
```

On the first run, the app trains the model from the two CSV files and saves it to `models/mindcheck_model.pkl`. Later runs load the pickle directly.

## Notes

This is an educational screening application. It is not a diagnostic device and should not replace care from a qualified mental health professional.

