# CoinCompass-POE_demo
#  CoinCompass

> **Navigate Your Finances**

CoinCompass is an Android personal finance management application built with **Kotlin**, **Room Database**, **Material Design 3**, and **View Binding**. The app helps users track expenses, manage income, set savings goals, and monitor spending habits through an intuitive and modern interface.

---

##  Features

###  Expense Management

* Add and manage expenses
* Categorise spending
* Attach receipt images
* Track dates and time ranges

###  Income Tracking *(New in v2.0)*

* Log income entries
* Select income source
* Real-time balance updates
* Monthly income storage

###  Savings Goals

* Set monthly minimum and maximum spending goals
* Track goal progress
* View goals in dashboard and transactions

###  Budget Overview
* Set monthly minimum and maximum spending goals
* Category-based spending analysis
* Dynamic progress indicators
* Real-time financial summaries

###  Transactions Dashboard *(New in v2.0)*

* Unified transaction feed
* Filter tabs:

  * All
  * Income
  * Expenses
  * Goals
* Monthly summary cards

###  User Management

* User registration
* Secure login
* Personalized financial data
* SharedPreferences session storage

---

##  What's New in Version 2.0

| Feature                | Version 1.0     | Version 2.0 |
| ---------------------- | --------------- | ----------- |
| Income Tracking        | ❌ Not Available | ✅ Added     |
| Transactions Screen    | ❌ Not Available | ✅ Added     |
| Bottom Navigation      | ❌ Not Available | ✅ Added     |
| Monthly Income Storage | ❌ Not Available | ✅ Added     |
| Income Database Table  | ❌ Not Available | ✅ Added     |
| Real-Time Balance      | ❌ Hardcoded     | ✅ Dynamic   |
| Transaction Filters    | ❌ Not Available | ✅ Added     |
| Calendar               | ❌ Not Available | ✅ Added     |
| Gamification           | ❌ Not Available | ✅ Added     |

---

##  Tech Stack

| Technology        | Purpose               |
| ----------------- | --------------------- |
| Kotlin            | Android Development   |
| Room Database     | Local Data Storage    |
| SQLite            | Database Engine       |
| View Binding      | UI Interaction        |
| Material Design 3 | User Interface        |
| LiveData          | Reactive Data Updates |
| Coroutines        | Background Processing |

---

##  Database Structure

### Users

```text
id
username
password
fullName
monthlyIncome
```

### Categories

```text
id
name
budgetAmount
```

### Expenses

```text
id
date
startTime
endTime
description
categoryName
amount
photoPath
```

### Goals

```text
id
month
minGoal
maxGoal
```

### Income (v2.0)

```text
id
date
description
amount
source
```

---

##  Colour Palette

| Colour      | Hex     |
| ----------- | ------- |
| Dark Green  | #1B4332 |
| Mid Green   | #2D6A4F |
| Light Green | #D8E2DC |
| Gold Accent | #E9C46A |
| Cream       | #FEFAE0 |
| Delete Red  | #BA181B |
| Background  | #F5F5F5 |
| Text Grey   | #6C757D |

---

##  Screenshots

Add screenshots here:

```md
<img width="1200" height="1920" alt="WhatsApp Image 2026-06-15 at 13 00 13" src="https://github.com/user-attachments/assets/fe634088-a1be-4183-a11a-d2e700b4fcef" />
  
![splash](https://github.com/lexi0222/CoinCompass-POE_demo/blob/010c168c65bf785c015d4a4e8e255eb66e7c7c65/WhatsApp%20Image%202026-06-15%20at%2013.00.13.jpeg)
![Dashboard](screenshots/dashboard.png)
![Transactions](screenshots/transactions.png)
![Add Expense/income](screenshots/add_expense.png)
![Calendar](screenshots/calendar.png)
![gamification](screenshots/gamification.png)

```

---

##  Installation

### Clone Repository

```bash
git clone https://github.com/your-username/CoinCompass.git
```

### Open Project

1. Open Android Studio
2. Select **Open Project**
3. Navigate to the CoinCompass folder
4. Wait for Gradle Sync

### Run Application

```bash
Shift + F10
```

or click the ▶ Run button.

---

## 📁 Project Structure

```text
CoinCompass
│
├── activities
├── adapters
├── dao
├── database
├── entities
├── repositories
├── layouts
├── utils
└── resources
```

---

## 🔄 Database Migration (v1 → v2)

Version 2 introduces:

* Income table
* Monthly income tracking
* Transactions screen
* Bottom navigation
* Real-time balance calculations

Migration is handled automatically through:

```kotlin
MIGRATION_1_2
```

No user data is lost during upgrade.

---

## 🎥 Demo Video

Watch the application demo:

https://youtube.com/shorts/z0DBXnjCBFE

---

## 👨‍💻 Developer

**CoinCompass Team**

Built using Android Studio, Kotlin, Room Database, and Material Design 3.

---

## 📄 License

This project is developed for educational and portfolio purposes.
