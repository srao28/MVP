# MVP
# MVP
# Expense Manager

Flask + SQLite expense tracking app.

## Requirements

* Python 3.9+
* `pip install -r requirements.txt`

## Setup

```bash
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Run

```bash
python app.py
```

App runs at `http://127.0.0.1:5000/`.

## Structure

```
expense_manager/
├── app.py
├── database.py
├── models.py
├── expenses.db
├── requirements.txt
├── static/
│   └── style.css
└── templates/
    ├── index.html
    └── add_expense.html
```

## Routes

* `GET /` list expenses
* `GET /add` new expense form
* `POST /add` create expense

## Database

Table: `expenses`

| column      | type    |
| ----------- | ------- |
| id          | INTEGER |
| amount      | REAL    |
| category    | TEXT    |
| description | TEXT    |
| date        | TEXT    |
