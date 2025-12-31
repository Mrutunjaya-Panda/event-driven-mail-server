# 📩 Event-Driven Mail Server (Node.js)

A Node.js server that handles user POST requests, stores user queries asynchronously, sends confirmation emails using Nodemailer, and emits a custom event upon successful email delivery.

This project demonstrates **event-driven architecture** in Node.js.

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Implement a Node.js server to handle a **POST request**
2. Extract **user's name, email, and message** from the request body
3. Append the extracted data **asynchronously** to a file named `queries.txt`
4. Use **Nodemailer** to send a confirmation email to the provided email address
5. Emit a custom event **`mailSent`** after successful email delivery

---

## 🚀 Features

- Handles HTTP POST requests
- Asynchronous file handling using `fs`
- Email sending using Nodemailer
- Custom event emission using `EventEmitter`
- Demonstrates non-blocking, event-driven workflow

---

## 🧠 Tech Stack

- **Node.js**
- **Express.js**
- **Nodemailer**
- **Events (EventEmitter)**
- **File System (fs)**

---

```
.
├── index.js # Entry point
├── server.js # Server configuration
├── queries.txt # Stores user queries (auto-generated)
├── package.json
├── .gitignore
└── README.md

```


---

## 🛠️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/event-driven-mail-server.git
2. Install dependencies
   ```bash
   npm install
3. Configure email credentials
 ```
   Create a .env file:
   PORT=3000
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASS=your_app_password
```
4. Start the server
   ```bash
   npm start

⚙️ Workflow Explanation
```
  Client sends a POST request with user data

  Server extracts name, email, and message

  Data is appended asynchronously to queries.txt

  Nodemailer sends a confirmation email

  On success, a custom event mailSent is emitted

  Event listener logs confirmation
```

📌 Custom Event Used
  ```bash
  mailSent
```
🧪 Testing
```
You can test the API using:

Postman

Thunder Client

cURL
```
📄 License

This project is for learning and academic purposes.

👤 Author

Mrutunjaya Panda

## 📁 Project Structure

