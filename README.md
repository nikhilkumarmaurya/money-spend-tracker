# money-spend-tracker
This is a  simple front end HTML website where you can add item name ,quality, and each price to calculate.

# 💸 Spend Tracker (Single-File Application)

This is a premium, modern, and dark-themed personal expense tracking tool implemented entirely within a single HTML file using **Tailwind CSS** for rapid styling and plain **JavaScript** for all application logic and state management via **Local Storage**.

It allows users to track their spending against a set budget using a simple input format.

## ✨ Features

* **Single-File Simplicity:** The entire application is contained in one portable `index.html` file.
* **Persistent State:** All budget and expense data is saved and loaded automatically using the browser's **Local Storage**.
* **Budget Tracking:** Set a total budget and instantly see your **Total Spent** and **Remaining/Overspent** amount.
* **Intuitive Input:** Quickly add expenses using a simplified format: `ItemName Quantity UnitPrice` (e.g., `Coffee 2 4.50`).
* **CRUD Operations:** Easily **Add**, **View**, **Edit** (with inline editing), and **Delete** expenses.
* **Real-time Search:** Filter your expense history instantly with a live search bar.
* **Modern UI:** A slick, responsive, and professional dark-theme interface powered by Tailwind CSS and Lucide icons.
* **PDF Export:** Generate a clean, printable financial report of all expenses and the budget summary.
* **Toast Notifications:** Provides real-time feedback for adding, deleting, and updating data.

<img src="https://i.ibb.co/Tqbny1bb/Screenshot-20251020-213525-Chrome.jpg" alt="Screenshot-20251020-213525-Chrome" border="0">


## 🚀 How to Use

### 1. Setup

1.  **Save the file:** Save the entire provided code snippet as an `index.html` file.
2.  **Open in Browser:** Double-click the `index.html` file to open it in any modern web browser. No server is required!

### 2. Core Actions

#### Set Budget
1.  Click the **"Set Budget"** button in the header.
2.  Enter your desired maximum spending amount (e.g., `500.00`).
3.  Click **"Save Budget"**. The summary will update immediately.

#### Add Expense
1.  Use the **"Add New Expense"** form.
2.  Input your expense using the format: **Item Name Quantity UnitPrice**.
    * **Example:** `Gala Apples 5 1.20` (5 units at $1.20 each = $6.00 total)
    * **Example:** `Netflix Subscription 1 15.99` (1 unit at $15.99 each = $15.99 total)
3.  Click **"Add Expense"**.

#### Edit/Delete Expense
1.  Locate the expense in the **Expense History**.
2.  Click the **Pencil icon** (✏️) to switch to inline edit mode. You can then modify the item, quantity, and unit price. Click the **Save icon** (💾) to apply changes.
3.  Click the **Trash icon** (🗑️) to instantly delete the expense.

#### Search
* Use the search bar below the add expense form to filter the expense list by **Item Name**.

#### Export
* Click the **Download icon** in the top right of the history section to generate a formatted PDF report of your current budget summary and all expenses.

## ⚙️ Technical Stack

* **Styling:** Tailwind CSS (via CDN)
* **Icons:** Lucide Icons (via CDN)
* **Logic:** Vanilla JavaScript
* **Data Persistence:** Browser Local Storage (`STORAGE_KEY: 'nikcoderSpendTrackerData'`)

## ⚠️ Note on Currency

The application uses the rupee symbol (₹) in the summary headers in the HTML/CSS, but the JavaScript logic and all numerical displays are hardcoded to show the dollar sign (**$**) for simplicity and consistency in the code, using the `formatCurrency` function. If you need to change the displayed currency, modify the following lines in the `<script>` tag:

* **`updateSummary` function:** Change `$` in the `textContent` lines.
* **`createExpenseCard` function:** Change `$` in the card template strings.
* 

My thinking my idea, concept and Algorithm , only code is written by Ai
