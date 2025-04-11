# 💬 Real-Time Customer Support Chatbot

A real-time customer service chatbot built with **Node.js**, **Socket.IO**, **MySQL**, and **Vanilla JS**. This project simulates a simple yet functional customer-agent chat system, including smart auto-replies using keyword detection.

---

## 🚀 Features

- 🔌 Real-time messaging with Socket.IO
- 🤖 Intelligent auto-replies based on keywords
- 💾 Persistent chat history using MySQL
- 👤 Message metadata (sender name and timestamp)
- 🌐 Simple and responsive frontend with HTML/CSS/JS
- 🔐 Secure configuration with `.env` support

---

## 📽️ Demo (Screen Recording)

🎥 [Watch the demo video on Google Drive](https://drive.google.com/file/d/1ynkup5GKoZwajuihPK-M53oxKYKq3gn1/view?usp=sharing)

---

## 🛠 Technologies Used

- **Node.js + Express** – Server-side logic
- **Socket.IO** – WebSocket-based real-time chat
- **MySQL** – Database for storing messages
- **HTML/CSS/JS** – Client-side interface
- **dotenv** – Environment variable management

---

## 📁 Project Structure

```
project/
├── server/
│   ├── server.js          # Backend logic and socket events
│   ├── .env               # Environment variables (not pushed to GitHub)
│   └── public/            # Static frontend files
│       └── index.html     # Chat UI
├── README.md
└── package.json
```

---

## ⚙️ Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name/server
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Setup Environment Variables
Create a `.env` file inside the `server/` folder:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=chatbotdb
```

### 4. Start MySQL and Create Database
Login to MySQL and run the following:
```sql
CREATE DATABASE chatbotdb;
USE chatbotdb;

CREATE TABLE messages (
  id INT AUTO_INCREMENT PRIMARY KEY,
  sender VARCHAR(255),
  receiver VARCHAR(255),
  message TEXT,
  timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### 5. Start the Server
```bash
node server.js
```

### 6. Open in Browser
```
http://localhost:3000
```

---

## 💬 Test the Chatbot
You can try sending messages like:
- "Hello"
- "What are your features?"
- "I need help"
- "How can I return an item?"
- "What is the price?"
- "How to reset my password?"

The bot will respond with predefined smart replies.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
