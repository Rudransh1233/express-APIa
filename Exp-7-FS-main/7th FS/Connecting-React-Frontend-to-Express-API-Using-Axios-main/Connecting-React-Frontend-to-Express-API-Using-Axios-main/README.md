# Connecting React Frontend to Express API Using Axios

---

## Expected Output
![Output](/OUTPUT/OUTPUT%201.png)


---

## Objective
Learn how to connect a React frontend application to a backend Express.js API using Axios to fetch data. This helps you understand how to integrate frontend and backend parts of a full stack application and handle HTTP requests in React.

---

## Task Description
1. Create a simple **Express.js API** that returns a list of products (each with a name and price).
2. Build a **React frontend application** that uses **Axios** to fetch product data from the Express API when the component mounts.
3. Display the list of products in a user-friendly layout (name + price).
4. Handle loading states and errors properly.
5. Test the connection by running both frontend and backend locally.

---

## Backend Setup

### 1. Initialize Node.js Project
```bash
npm init -y
npm install express cors
```

### 2. Create the Server File
Save the following code as `server.js`

```js
const express = require('express');
const cors = require('cors');
const app = express();

app.use(cors());

const products = [
  { id: 1, name: 'Laptop', price: 1200 },
  { id: 2, name: 'Mouse', price: 25 },
  { id: 3, name: 'Keyboard', price: 45 }
];

app.get('/api/products', (req, res) => {
  res.json(products);
});

app.listen(5000, () => console.log('Server running on port 5000'));
```

### 3. Run the Server
```bash
node server.js
```

Your backend will be available at:
```
http://localhost:5000/api/products
```
