# Expense Tracker Web Application

A simple, intuitive web application to manage expenses. Users can log their expenses, view a summary with individual entries as cards, and see a cumulative total. The app uses `sessionStorage` to store data temporarily, making it lightweight and suitable for quick budgeting tasks.

## Features

- **Add Expense**: Users can enter an expense with the amount, date, and category. Each expense is stored as an entry in `sessionStorage`.
- **Summary Page**: Displays all submitted expenses in a card format, showing details for each entry along with a total amount of all expenses.
- **Clear All**: A button that clears all stored expense data from `sessionStorage` and resets the summary display.
- **Close Tab**: A button to close the current tab (note: may only work if the tab was opened via JavaScript due to browser security).

## Pages and Structure

1. **Add Expense Page (`add-expense.html`)**:
   - Allows users to input and submit expenses.
   - Each submission is stored in `sessionStorage` as an object (amount, date, and category).
   - Redirects to the `summary.html` page after submission.

2. **Summary Page (`summary.html`)**:
   - Retrieves and displays all stored expense entries as styled cards.
   - Shows a cumulative total of all expenses.
   - Provides "Clear All" and "Close Tab" buttons.

## Code Structure

- **HTML**: Each page (Add Expense and Summary) is built with simple HTML for form submission and dynamic display.
- **JavaScript**: Manages data flow using `sessionStorage`, dynamically creates cards for expenses, calculates the total, and handles button functions like clearing data and closing the tab.
- **CSS**: Provides styling for a clean, card-based layout on the summary page, making each expense entry visually distinct.

## How to Run

1. Clone or download this repository.
2. Open `add-expense.html` in your preferred browser.
3. Start by entering expenses through the form.
4. View the summary page, where all expenses and the total amount are displayed.

> **Note**: Data is stored in `sessionStorage`, so it will be cleared when the browser session ends. Use the "Clear All" button to clear the stored data manually.

## Future Enhancements

Consider adding these features:
- **Persistent Storage**: Use local storage or a database to make data persistent across sessions.
- **Export Option**: Add a feature to export expenses to a CSV or JSON file.
- **Enhanced Categories**: Allow users to add custom categories.
