# 🧮 Sum Server – A Simple Express API

Welcome to **Sum Server**! 🚀  
This is a lightweight Express.js API project deployed on an **AWS EC2 instance**. It provides utility endpoints for basic arithmetic, interest calculation, notifications, and a simple todo system – perfect for learning and demos.

---

## 🌐 Live on AWS EC2
This application is **deployed on an AWS EC2 Ubuntu instance** using Node.js and NVM. Follow the steps below to deploy it yourself.

---

## 🛠️ Features

✅ `/sum?a=10&b=20` – Returns the sum  
✅ `/interest?principal=1000&rate=5&time=2` – Simple interest calculator  
✅ `/todos` – Returns a random list of todo items  
✅ `/todo?id=2` – Returns a specific todo  
✅ `/notifications` – Returns random notification counts  

---

## 📦 Tech Stack

- **Backend:** Node.js + Express.js  
- **Deployment:** AWS EC2 (Ubuntu)  
- **Package Manager:** npm  
- **Node Versioning:** nvm  

---

## 🚀 Deployment Instructions on AWS EC2

### 1. 🔁 Clone the repository

```bash
git clone https://github.com/Namrathaaaaaa/sum-server.git
cd sum-server
```

### 2. 🧰 Install Node.js using NVM

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

After installation, activate NVM:

```bash
export NVM_DIR="$HOME/.nvm"
source ~/.bashrc
```

### 3. 📦 Install Node.js LTS and dependencies

```bash
nvm list-remote
nvm install --lts
npm install
```

### 4. ▶️ Run the server

```bash
node index.js
```

Server will start on [http://localhost:8080](http://localhost:8080)

---

## 🧪 API Endpoints

| Endpoint         | Method | Description                            |
|------------------|--------|----------------------------------------|
| `/sum`           | GET    | Returns `a + b`                        |
| `/interest`      | GET    | Returns simple interest + total amount|
| `/todos`         | GET    | Returns random todos                  |
| `/todo?id=2`     | GET    | Returns a specific todo               |
| `/notifications` | GET    | Simulates notification counts         |
| `/`              | GET    | Welcome message (recommended to add)  |

---

## ✅ Example

**GET** `http://localhost:8080/sum?a=10&b=15`  
**Response:**  
```
25
```

---

## 📌 To-Do
- [ ] Add POST and PUT endpoints
- [ ] Connect to a database (MongoDB or PostgreSQL)
- [ ] Add Swagger for API documentation

---

## 💡 Tip

To make your server more informative, add this in `index.js`:

```js
app.get("/", (req, res) => {
  res.send("✅ Sum Server is up and running on AWS EC2!");
});
```

---

## 🙌 Author

Developed by [Namratha](https://github.com/Namrathaaaaaa)  
Feel free to contribute or fork!
