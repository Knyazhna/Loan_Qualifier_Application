# Loan Qualifier Application

This is a python command-line interface application that allows users to see qualifying loans from lenders quickly and easily. The application works by taking in a `daily_rate_sheet` of loan criteria from various loan providers, asking the user a number of questions to evaluate their loan eligibility, and then returning to them a list of qualifying loans. User also has an ability to save a list of qualifying loans to a new csv file, so user can share the resuts as a spreadsheet.

---

## Technologies

This project leverages python 3.7 with the following packages:

* [fire](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint.

* [questionary](https://github.com/tmbo/questionary) - For interactive user prompts and dialogs

---

## Installation Guide

Before running the application first install the following dependencies.

```python
  pip install fire
  pip install questionary
```

```
import sys
import fire
import questionary
```
---

## Usage

To use the loan qualifier application simply clone the repository and run the **app.py** with:


```python
python3 app.py
```

Upon launching the loan qualifier application you will be greeted with the following prompts.
*Enter a file path to a rate-sheet (.csv):
When prompted for your CSV file path, please enter ./data/daily_rate_sheet.csv.
Few additional pieces of information will need to be provided:

```
    credit_score = questionary.text("What's your credit score?").ask()
    debt = questionary.text("What's your current amount of monthly debt?").ask()
    income = questionary.text("What's your total monthly income?").ask()
    loan_amount = questionary.text("What's your desired loan amount?").ask()
    home_value = questionary.text("What's your home value?").ask()
```
After information input, CLI will prompt you to save or not to save csv file. 

---

## Contributors

* Brought to you by Olga Koryachek.
* Email: olgakoryachek@live.com
* [LinkedIn](https://www.linkedin.com/in/olga-koryachek-a74b1877/?msgOverlay=true)


---

## License

Licensed under the [MIT License](https://choosealicense.com/licenses/mit/)


