# Group Expense Splitter Portal

A simple console portal to track shared group expenses and split costs evenly among members.

## Features

- User login with username and password
- Add new expense records
- Search expenses by ID, description, or payer
- View all stored expenses
- Generate a split report (balances: who should receive / who should pay)
- Persistent storage using CSV (created at runtime)

## Requirements Covered

| Requirement | How it is used |
|-------------|----------------|
| Functions (`def`) | `user_login()`, `add_record()`, `search_record()`, `generate_report()`, etc. |
| Loops (`for`, `while`) | Main menu uses `while True`; expenses are processed with `for` loops |
| File handling | Creates/updates `expenses.csv` when expenses are added or on exit |
| Exception handling | Handles `FileNotFoundError`, `PermissionError`, `ValueError`, and unexpected errors |

## How to Run

```bash
python main.py
```

### Demo login credentials

| Username | Password |
|----------|----------|
| fatima | fatima123 |
| rija | rija123 |

## Project Structure

```
[25L-5188_25L-5107]_Assignment3/
├── expense-splitter.ipynb          # Main portal application
└── README.md        # Project documentation
```

`expenses.csv` is created automatically when you add the first expense.

## Sample Workflow

1. Run the program and log in
2. Choose option 1 to add an expense
3. Choose option 2 to search expenses
4. Choose option 3 to view all expenses
5. Choose option 4 to see who owes / is owed money
6. Choose option 5 to save and exit
