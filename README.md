
# SpendWise - Interactive Budget Tracker

## Project Description

SpendWise is a simple budgeting application developed using HTML, CSS, and JavaScript.

The application helps users manage their money by setting a budget, recording expenses, calculating total spending, and checking their remaining balance.

This week's improvements make the application interactive and allow users to manage multiple expense records directly on the webpage.

## Improvements Made This Week

The following features were added:

1. Users can set and update their monthly budget.
2. Users can add multiple expenses.
3. Users can select expense categories.
4. The application automatically calculates total expenses.
5. The remaining balance is displayed dynamically.
6. Users can delete individual expenses.
7. Users can clear all expense records.
8. The application provides warnings when spending exceeds the budget.
9. The dashboard updates automatically when users make changes.

## JavaScript Concepts Implemented

### 1. Conditional Statements

Conditional statements help the application make decisions based on the user's budget and expenses.

For example:

- If the budget is zero, the application asks the user to enter a budget.
- If expenses exceed the budget, a warning is displayed.
- If the remaining balance is low, the application displays a warning.
- If the user manages the budget well, a positive message is displayed.

### 2. Arrays

An array called `expenses` is used to store multiple expense records.

Each expense contains:

- Expense name
- Amount
- Category
- Unique identifier

Example:

```javascript
let expenses = [];

expenses.push({
    id: Date.now(),
    name: "Food",
    amount: 1500,
    category: "Food"
});
```

This makes it easier to add, manage, and delete expense records.

### 3. Loops

Loops are used to process the expense records.

A `for` loop calculates the total expenses by adding all the amounts stored in the array.

The `forEach()` method displays each expense on the webpage.

### 4. DOM Manipulation

DOM manipulation allows JavaScript to update webpage content without refreshing the page.

The application uses:

- `getElementById()` to select HTML elements.
- `textContent` to display information.
- `createElement()` to create expense records.
- `appendChild()` to add records to the webpage.

### 5. Event Listeners

Event listeners allow the application to respond to user actions.

The project uses:

- `submit` events to handle budget and expense forms.
- `click` events to delete expenses and clear records.
- `preventDefault()` to stop forms from refreshing the webpage.

### 6. Functions

Reusable functions are used to organize the JavaScript code.

Examples include:

- `formatMoney()`
- `calculateTotalExpenses()`
- `calculateBalance()`
- `displayExpenses()`
- `updateDashboard()`

These functions make the code easier to understand and maintain.

## Challenges Encountered and Solutions

### Challenge 1: Managing Multiple Expenses

It was difficult to manage several expense records using individual variables.

Solution: I used an array to store multiple expenses and loops to process them.

### Challenge 2: Updating Dashboard Information

The dashboard needed to display new information whenever an expense was added or deleted.

Solution: I created an `updateDashboard()` function that recalculates and updates the information automatically.

### Challenge 3: Handling Incorrect User Input

Users might enter empty fields or invalid amounts.

Solution: I used conditional statements and input validation to prevent incorrect information from being accepted.

### Challenge 4: Monitoring the Budget

Users needed to know when their spending was higher than their budget.

Solution: I used conditional statements to compare the total expenses with the available budget and display appropriate messages.

## How to Run the Project

1. Download or clone the SpendWise repository.
2. Open the project folder in Visual Studio Code.
3. Ensure all four files are in the same folder.
4. Open `index.html` in your web browser.
5. Enter a monthly budget.
6. Add expenses and test the dashboard.

## Testing

The following features should be tested:

- Setting a monthly budget.
- Adding different expenses.
- Calculating total expenses.
- Calculating the remaining balance.
- Deleting an individual expense.
- Clearing all expenses.
- Checking the warning when the budget is exceeded.
- Testing invalid input.

## Technologies Used

- HTML5
- CSS3
- JavaScript

## Conclusion

SpendWise demonstrates how JavaScript can make a webpage interactive.

Through conditional statements, arrays, loops, DOM manipulation, functions, and event listeners, users can manage their expenses and monitor their budgets more easily.
