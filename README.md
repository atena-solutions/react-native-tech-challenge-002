# 🧪 React Native Technical Challenge: Personal Finance Tracker App

## 🎯 Objective

Build a **React Native** mobile app that allows users to track their personal finances. The app should allow users to manage **income**, **expenses**, and **monthly budgets**, and give a clear overview of their financial balance.

---

## 📚 User Stories

### 1. Register a Transaction

As a user, I want to register an **income** or **expense**, so I can track my financial movements.

Each transaction must include:
- `type`: `"income"` or `"expense"`
- `category`: e.g., `"food"`, `"salary"`, `"entertainment"`
- `amount`: number
- `currency`: e.g., `"USD"`, `"EUR"`, `"BRL"`
- `date`: use a date picker
- `description`: optional

### 2. Define Monthly Budgets

As a user, I want to define **monthly budgets** per category.

Example:
- `"food"` → `$1000` for June

### 3. View Monthly Summary

As a user, I want to see a **monthly summary** that includes:
- Total income and expenses
- Remaining budget per category
- Alerts if any category has exceeded the budget

---

## 🌍 External API Integration

When registering a transaction in a currency different from the base currency (assume `USD`), the app must:

✅ **Call a public exchange rate API** to convert the amount to USD.

You may use one of the following APIs:
- https://exchangerate.host/
- https://open.er-api.com/
- https://currencyapi.com/

### Integration Requirements:
- Isolate the external API logic in a **dedicated service layer**.
- Implement proper **error handling** (e.g., retries, fallbacks).
- Handle loading and failure states gracefully in the UI.

---

## 📐 Architecture Guidelines

Your app must follow **clean architecture principles** and be modular. Organize your code using folders such as:

- `screens/`
- `components/`
- `services/`
- `contexts/` or `store/`
- `utils/`

You may use any of the following:
- Context API or Zustand for state management
- React Navigation for navigation
- Axios or Fetch for HTTP requests
- Expo or React Native CLI (your choice)

---

## ✅ Bonus Points

- Unit and/or integration tests using Jest and React Native Testing Library
- Offline support or local caching using AsyncStorage or MMKV
- TypeScript support
- Responsive layout and polished UI/UX
- E2E testing with Detox (optional)

---

## 📦 Delivery Instructions

1. Push your code to a **public GitHub repo**.
2. Include a `README.md` with:
   - Project overview
   - Setup instructions
   - Any relevant notes (e.g., limitations, improvements)
   - `.env.example` if using API keys

---

## 💡 What We'll Be Evaluating

- Code structure and readability
- Architectural decisions
- State management and data flow
- API integration quality
- UX polish and error handling
- Testing approach (if present)
- Communication and documentation
