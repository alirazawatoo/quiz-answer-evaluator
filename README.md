# Quiz Answer Evaluator

A Django API and React client for loading a quiz, collecting answers, submitting them for evaluation, and presenting the result.

## Structure

- `quiz_app_api/quiz` — quiz model, submission endpoint, validation, and API tests.
- `quiz-app-web/src/components/quiz.js` — quiz rendering and answer state.
- `quiz-app-web/src/routes/api.js` — client API boundary.

## Local setup

```bash
cd quiz_app_api
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

In another terminal, run `npm install && npm start` from `quiz-app-web`. Tests exist for API submission and frontend behavior. Evaluation is limited to rules represented in the code, not general semantic grading.
