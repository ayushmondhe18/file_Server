# ☁️ CloudShare — File Sharing Application

A simple and efficient **file-sharing web application** that allows users to upload files and share them with others through a generated download link.

This repository contains the **backend REST API** built using **Node.js, Express.js, and MongoDB**.

## 🚀 Features

* 📤 Upload files through the web application
* 🔗 Generate shareable download links
* 📥 Download shared files
* 📧 Share files with recipients through email
* 🗄️ Store file metadata using MongoDB
* ⚡ RESTful API architecture
* 🌐 Simple and responsive file-sharing workflow
* 🔒 Environment-based configuration for sensitive credentials

## 🛠️ Tech Stack

### Backend

* **Node.js**
* **Express.js**
* **MongoDB**
* **Mongoose**
* **REST API**

### Frontend

The frontend can be integrated separately with this backend API.

## 📁 Project Structure

```text
CloudShare/
│
├── config/
│   └── Database configuration
│
├── models/
│   └── MongoDB data models
│
├── routes/
│   └── API routes
│
├── services/
│   └── Application/business logic
│
├── public/
│   └── Static files
│
├── uploads/
│   └── Uploaded files
│
├── views/
│   └── Server-side views
│
├── .env.example
├── .gitignore
├── package.json
├── server.js
├── script.js
└── README.md
```

## ⚙️ Prerequisites

Make sure you have the following installed:

* [Node.js](https://nodejs.org/)
* npm
* MongoDB / MongoDB Atlas
* Git

## 📥 Installation

### 1. Clone the repository

```bash
git clone https://github.com/codersgyan/inshare-file-sharing-app-api.git
```

### 2. Navigate to the project

```bash
cd inshare-file-sharing-app-api
```

### 3. Install dependencies

Using npm:

```bash
npm install
```

Or using Yarn:

```bash
yarn install
```

### 4. Configure environment variables

Rename `.env.example` to `.env`:

```bash
.env.example → .env
```

Then add your required configuration and credentials.

Example:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

> Do not commit your `.env` file to GitHub. Keep credentials and API keys private.

## ▶️ Running the Application

Start the development/server environment with:

```bash
npm start
```

or:

```bash
yarn start
```

Once the server starts, the API will be available at:

```text
http://localhost:5000
```

## 🔄 How It Works

The application follows a simple file-sharing workflow:

```text
User
  │
  ▼
Upload File
  │
  ▼
Express.js API
  │
  ├──► Store File
  │
  └──► Store File Metadata
          │
          ▼
       MongoDB
          │
          ▼
   Generate Share Link
          │
          ▼
     Share with User
          │
          ▼
       Download
```

## 🔌 API Workflow

The backend provides the API layer responsible for handling file-sharing operations.

Typical workflow:

### Upload

```text
Client
  ↓
POST Request
  ↓
Express Server
  ↓
File Upload
  ↓
MongoDB Metadata
  ↓
Shareable Link
```

### Download

```text
Shareable Link
      ↓
Backend API
      ↓
Find File
      ↓
Return File
      ↓
User Downloads File
```

## 🧩 Frontend

The original project has a separate frontend implementation.

Frontend repository:

https://github.com/ShivamJoker/InShare

The frontend communicates with this backend through the REST API.

## 🔐 Environment Variables

Never expose sensitive credentials directly in your source code.

Create a `.env` file and configure values such as:

```env
PORT=5000
MONGO_URI=your_mongodb_uri
```

Depending on your configuration, additional variables may be required.

## 🧪 Development

After making changes to the project:

```bash
npm install
npm start
```

Test the API using tools such as:

* Postman
* Thunder Client
* Browser
* Your frontend application

## 📌 Use Cases

This project can be used for:

* Sharing documents
* Sharing project files
* Sending files to friends or teammates
* Academic project submissions
* Temporary file transfer
* Learning REST API development
* Learning file uploads with Node.js

## 🔮 Future Improvements

Some possible improvements include:

* 🔑 User authentication and authorization
* 🔒 Password-protected file links
* ⏳ Automatic link expiration
* 🗑️ Automatic file deletion
* 📊 Download analytics
* 📦 Cloud storage integration
* 🧾 File size/type validation
* 🛡️ Rate limiting and additional security
* 📱 Mobile-friendly interface
* ☁️ Deployment using services such as Render, Railway, or AWS

## 👨‍💻 Technologies Learned

Through this project, developers can practice:

* Node.js
* Express.js
* REST API development
* MongoDB
* Mongoose
* File handling
* Backend architecture
* Environment variables
* API integration
* Full-stack application development

## ⭐ Credits

This project is based on the original **InShare File Sharing API** by **CodersGyan**.

Original repository:

https://github.com/codersgyan/inshare-file-sharing-app-api

---

## 📄 License

This project is intended for educational and development purposes.
