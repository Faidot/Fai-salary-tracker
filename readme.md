# 🏦 Fai Salary Tracking - Terafort Edition

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Tech](https://img.shields.io/badge/stack-HTML%20%7C%20Tailwind%20%7C%20JS-3b82f6)
![License](https://img.shields.io/badge/license-MIT-green)

A sophisticated, client-side salary tracking application designed for **Terafort / Elite Qubit** employees. This tool helps manage monthly finances, track "Abi" (advance) withdrawals, calculate daily accruals, and synchronize data with Google Sheets for reliable cloud backup.

---

## ✨ Key Features

### 📊 Smart Dashboard
- **Live Status**: Real-time visualization of the current salary cycle.
- **Accrual Tracking**: Automatically calculates how much salary has "accrued" based on the number of days passed in the current cycle.
- **Available Limit**: Shows exactly how much you can withdraw right now based on your daily limit and current withdrawals.
- **Visual Progress**: Progress bar indicating the completion percentage of the current month.

### 💸 Transaction Management
- **Abi Withdrawals**: Easily record advance salary withdrawals.
- **Fee Calculation**: Automatically adds transaction fees (default Rs 150) to every withdrawal.
- **History**: View and delete recent transactions.

### ☁️ Cloud Sync (Google Sheets)
- **Backup & Restore**: One-click synchronization with a personal Google Sheet.
- **Two-Way Sync**: Push local data to the cloud or restore data to a new device.
- **Secure**: Uses your own Google Apps Script deployment.

### 📑 Comprehensive Reports
- **Monthly Summaries**: Detailed breakdown of Net Salary, Total Deductions (Abi + Fees), and Final HR Payable amount.
- **Status Tracking**: Mark months as "Running", "Pending", or "Settled".
- **History**: Keeps a record of all past salary cycles.

### ⚙️ Flexible Configuration
- **Custom Salary**: Adjust Gross Salary and Fixed Deductions (PF/Tax) for each month individually.
- **Persistent Settings**: Configuration is saved per month, allowing for salary increments or changes over time.

---

## 🛠️ Technology Stack

- **Frontend**: HTML5, Vanilla JavaScript
- **Styling**: [TailwindCSS](https://tailwindcss.com/) (CDN), Custom CSS for Glassmorphism effects
- **Icons**: [FontAwesome](https://fontawesome.com/)
- **Storage**: Browser `localStorage` (Offline first) + Google Sheets (Cloud)

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Edge, Safari, Firefox).
- Internet connection (for loading Tailwind/FontAwesome resources and Cloud Sync).

### Installation

1.  **Clone or Download** the repository:
    ```bash
    git clone https://github.com/yourusername/elite-salary-tracker.git
    ```
2.  **Open the App**:
    Simply double-click `index.html` to open it in your browser. No server required!

---

## ☁️ Setting Up Cloud Sync (Optional)

To enable the "Cloud Backup" feature, you need to deploy the backend script:

1.  Go to [Google Sheets](https://sheets.google.com) and create a new blank sheet.
2.  Go to **Extensions > Apps Script**.
3.  Copy the contents of the `Google Apps Script` file from this repository.
4.  Paste it into the script editor (replace any existing code).
5.  Click **Deploy > New deployment**.
6.  Select type: **Web app**.
7.  Set **Who has access** to: **Anyone** (required for the app to talk to the sheet without complex OAuth).
8.  Click **Deploy** and copy the **Web App URL**.
9.  Open the **Fai Salary Tracking** app, paste the URL into the "Cloud Backup" section, and click **Sync**.

---

## 📖 Usage Guide

1.  **Initial Setup**:
    - Enter your **Gross Salary** and **Deductions** in the Configuration panel.
    - The app will automatically calculate your Net Salary and Daily Limits.

2.  **Recording a Withdrawal**:
    - Go to the "Abi Withdrawal" section.
    - Select the Date and enter the Amount.
    - Click **Confirm Withdrawal**.

3.  **Viewing Reports**:
    - Scroll down to "Monthly Reports & Payouts".
    - You will see a row for the current month (Running) and any past months.
    - Once you receive your salary, click **Mark Received** to settle the month.

4.  **Syncing**:
    - Click **Sync** to save your data to Google Sheets.
    - Click **Restore** if you are on a new device and want to load your data.

---

## 🎨 Design

The application features a modern **Glassmorphism** design with:
- Translucent panels with blur effects.
- Soft shadows and rounded corners.
- Interactive hover states and micro-animations.
- Responsive layout that works on Desktop and Mobile.

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.