# Personal Finance Tracker

## Overview

The **Personal Finance Tracker** is a web-based application designed to help users manage their personal finances by tracking income and expenses. This tool allows users to add, view, and delete financial entries, keeping a running tally of their balance. Data is stored in the browser's LocalStorage, ensuring persistence across page reloads.

## Features

- **Track Income and Expenses:** Add new entries specifying whether they are income or expenses.
- **Dynamic Summary:** View total income, total expenses, and current balance.
- **Editable Entries:** Remove entries from the list to adjust your financial data.
- **Responsive Design:** Adaptable layout for various screen sizes and devices.

## How to Use

1. **Add New Entries:**
   - Select whether the entry is an expense or income from the dropdown menu.
   - Enter the name and amount of the entry.
   - Click the "Add Expense" button to add the entry to the list.

2. **View Summary:**
   - The summary section displays your total income, total expenses, and current balance.

3. **Delete Entries:**
   - Click the delete icon next to an entry to remove it from the list and update the summary.

## LocalStorage API

The application uses the [LocalStorage API](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) to persist data across page reloads. LocalStorage allows us to store data in the user's browser in a key-value pair format.

### How It Works

- **Storing Data:**
  Data is stored in LocalStorage using `localStorage.setItem(key, value)`. In this application, financial entries are saved as a JSON string. For example:
  ```javascript
  localStorage.setItem("tableEntries", JSON.stringify(tableEntries));

## Project Structure

- **HTML:** Defines the structure of the application and includes the main elements such as the summary, input form, and table.
- **CSS:** Provides styling for the application, ensuring a clean and responsive design.
- **JavaScript:** Handles the application logic, including adding, removing, and updating financial entries, as well as managing LocalStorage.



