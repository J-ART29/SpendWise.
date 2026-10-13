# SpendWise - JavaScript Foundation

## Project Overview

SpendWise is a simple browser-based budgeting application. Users enter a
monthly budget, review or edit a set of sample expenses, and add more expenses
as needed. The application calculates total expenses and the remaining balance,
then displays a summary and an expense table.

## Features

- Opens an on-page budget form when the user clicks **Start Budgeting**.
- Pre-fills sample expenses with a name, amount, category, and date.
- Lets users add or remove expenses and choose from common categories.
- Validates the budget and expense details before calculating.
- Displays the monthly budget, total expenses, remaining balance, and expense list.
- Prints the completed report in the browser developer console.
- Includes budgeting tips on the page.

## JavaScript Concepts Implemented

### Variables and Data Types

The application stores the sample expenses and user-entered expenses as arrays
of objects. Each expense object contains a name, numeric amount, category, and
date. The budget and calculated totals are numbers, while names, categories,
and dates are strings.

### User Input and Validation

The form collects the monthly budget and expense details with HTML input
elements. JavaScript reads the form values, converts amounts to numbers, and
checks that the budget is greater than zero and that each entered expense has
a name, amount, and date. Incomplete expense rows show a validation message
instead of producing a report.

### Calculations

The `showBudgetSummary()` function adds expense amounts with `reduce()` to get
the total expenses. It subtracts that total from the monthly budget to calculate
the remaining balance.

### Functions and Events

- `formatMoney()` formats amounts as Kenyan shillings.
- `addExpenseField()` creates an expense entry and wires up its remove button.
- `showBudgetSummary()` calculates and displays the budget results.
- Event listeners reveal the form, add expense rows, and handle form submission.

### Output

The results are rendered in the page, including an accessible expenses table.
The application also uses `console.log()` and `console.table()` to print the
budget report in the browser developer console.

## Technologies Used

- HTML
- CSS
- JavaScript

## How to Run

1. Open `index.html` in a browser, or serve the folder with VS Code Live Server.
2. Click **Start Budgeting**.
3. Enter a monthly budget. The provided sample expenses can be edited, removed,
   or supplemented with **Add another expense**.
4. Click **Calculate budget** to view the summary and expense table.
5. To see the logged report, open the browser developer tools and select the
   Console tab.

## Author

SpendWise Project