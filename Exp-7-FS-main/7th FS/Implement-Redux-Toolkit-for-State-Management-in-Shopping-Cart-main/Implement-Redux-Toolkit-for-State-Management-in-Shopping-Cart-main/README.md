# 🛒 React Shopping Cart (Custom Redux-like Implementation)

A simple shopping cart built with **React** and a **custom Redux-like state management** system — no external libraries required!

---


---

## 🖼️ Output Preview

### /OUTPUT/OUTPUT 1.png
![Output](OUTPUT/OUTPUT%201.png)

---


## 🚀 Features Implemented

✅ **Custom Redux Store** – Lightweight store with `getState`, `dispatch`, and `subscribe`  
✅ **Reducer Pattern** – Handles `ADD`, `REMOVE`, and `UPDATE` actions  
✅ **Global State Management** – Centralized cart state across components  
✅ **Add to Cart** – Products increase quantity if already in the cart  
✅ **Remove from Cart** – Deletes items completely  
✅ **Update Quantity** – Editable item quantity via input  
✅ **Total Calculation** – Cart total auto-calculates  
✅ **Instant UI Updates** – State changes reflect immediately  
✅ **No External Libraries** – Works without Redux Toolkit or React-Redux  

---

## 🛠️ Installation

```bash
npm install
npm start
```

If you wish to use Redux Toolkit instead, install:
```bash
npm install @reduxjs/toolkit react-redux
```

---

## 📂 File Structure

```
src/
├── store.js          # Custom Redux-like store and cart reducer
├── App.js            # Main component with Products and ShoppingCart
└── components/       # (Optional) Separate component files
```

## 💡 Explanation

This app mimics Redux functionality **without any external dependencies**.  
It uses a global store created via `createStore()` with manual `subscribe()` to React state updates.

**Key Functions:**
- `createStore()` – Initializes store and state
- `dispatch()` – Updates state via reducer
- `subscribe()` – Triggers re-renders on change
- `cartReducer()` – Handles all cart operations

---
