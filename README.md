# CAR BOT ASSISTANT - STUDENT PROJECT 

# 🚗 Car Bot Assistant - Student Project

**CarBot** is a web application designed to simplify the process of researching and finding information about cars. It provides users with an intuitive chat-based interaction through a virtual assistant, **Car Bot**, powered by **Wit.ai**.

---

## 🎯 Problem Statement
Many users need **quick, accurate, and detailed** car search results, including prices, specifications, and images, without visiting multiple websites. **CarBot** aggregates this information in one place, allowing users to interact through **text and voice commands**.

![Logo](./projekat/images/logo.png)

---

## 🛠️ Technology Stack

This project is built using the **MERN stack** (**MongoDB, Express.js, React.js, Node.js**) with additional integrations.

### **1️⃣ Frontend - React.js**
- **React.js** is a JavaScript library for building dynamic, interactive UIs.
- It is used in this project to:
  - Render the **chat interface** dynamically.
  - Fetch and display **car-related data** from the backend.
  - Handle **user interactions** with chatbot messages.
  - Maintain **state management** using **React Hooks**.

### **2️⃣ Backend - Node.js & Express.js**
- **Node.js** is a JavaScript runtime that allows running JavaScript on the **server-side**.
- **Express.js** is a **minimal and flexible** web framework for building APIs.
- Key backend functionalities:
  - Handles **API requests** from the frontend.
  - Sends **user queries** to Wit.ai for processing.
  - Retrieves and stores data in **MongoDB**.
  - Implements **authentication and authorization** using **JWT (JSON Web Tokens).**

### **3️⃣ Database - MongoDB**
- **MongoDB** is a **NoSQL** database used for:
  - Storing **car information** (brand, model, price, specifications).
  - Managing **chatbot conversation history**.
  - Storing structured data imported from a **CSV dataset**.
  - Handling **large-scale unstructured data efficiently**.

### **4️⃣ Chatbot & NLP - Wit.ai**
- **Wit.ai** is an **AI-powered NLP (Natural Language Processing) platform**.
- It helps **CarBot**:
  - Understand **user intent** (e.g., "Find me a car under $20,000").
  - Extract **entities** such as brand names, price ranges, and car models.
  - Respond to queries dynamically with relevant **car data**.

### **5️⃣ Real-time Communication - WebSockets**
- **Socket.io** is used for real-time **bidirectional communication**.
- It enables **instant chatbot responses** without refreshing the page.
- Maintains an **active connection** between the frontend and backend.

### **6️⃣ Image Retrieval - Unsplash API**
- The **Unsplash API** dynamically fetches **high-quality images** of cars.
- Used to provide **visual representation** of search results.

### **7️⃣ Stock Market Data - Finhub API**
- The **Finhub API** provides **real-time stock prices** for **car brands**.
- Helps users **track market trends** of car manufacturers.

---

## 📊 Application Architecture

Below is the **conceptual diagram** showing how different components interact:

![Conceptual Diagram](./projekat/images/conceptual_diagram.png)

### **🏗️ How the System Works**
1. **User Interaction:** Users communicate with **Car Bot** via text or voice.
2. **Backend Processing:** Express.js processes user queries.
3. **Natural Language Understanding (NLU):** Queries are sent to **Wit.ai** for intent recognition.
4. **Database Retrieval:** Car details are fetched from **MongoDB** or **CSV dataset**.
5. **API Communication:** The system fetches car images (**Unsplash API**) and stock data (**Finhub API**).
6. **Real-time Responses:** Chatbot dynamically **responds** using **WebSockets**.

This ensures **structured, real-time responses** to user queries.

![System Workflow](./projekat/images/Logic.png)

---

## 🏁 Installation & Setup

### 🚀 Step 1: Clone the Repository

```bash
git clone https://github.com/Rale01/CarBot-AI-Assistant.git
```

### 📦 Step 2: Install Dependencies
```bash
npm install
```

### 🔥 Step 3: Start the Server
```bash
cd projekat
cd server
npm start
```

### 🌍 Step 4: Start the Frontend
```bash
cd projekat
cd server
npm start
```

### 🛠️ Step 5: Open the Application in Your Browser
Once both frontend and backend are running, open your browser and start chatting with Car Bot! 🚀

---

## 🏆 Features

- ✔️ Search for cars by brand, model, and price
- ✔️ Retrieve car specifications from a structured CSV dataset
- ✔️ Chatbot with Natural Language Processing (Wit.ai)
- ✔️ Fetch real-time car images from Unsplash API
- ✔️ Track stock market trends of car brands (Finhub API)
- ✔️ Real-time chatbot responses via WebSockets

---

# Web app showcase

# 🏠 Home Page

## 📜 Overview
The **Home Page** is the first screen users see when they open the application. It provides an introduction to the platform with a visually appealing design, including a **slider with images**.

## 🎯 Features
- **Introduction** to the Car Bot Assistant.
- **Navigation buttons** for easy access to different sections:
  - **Find the Right Car for You**: 
    - Redirects to the **Login Page** if the user is not logged in.
    - Redirects to the **Chat Page** if the user is logged in.
  - **About Us**: Navigates to the **About Us Page**.
  - **Sign In**: Takes the user to the **Login Page**.

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture1.png)


# ℹ️ About Us Page

## 📜 Overview
The **About Us Page** provides a detailed description of the Car Bot Assistant, including its purpose and functionalities.

## 🎯 Features
- Displays **general information** about the application.
- Accessible to:
  - **Guests (non-registered users)**
  - **Logged-in users**

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture2.png)





# 🔑 Login Page

## 📜 Overview
The **Login Page** allows users to access their accounts by entering their credentials.

## 🎯 Features
- Users can **log in** by providing:
  - **Email**
  - **Password**
- Clicking the **Log In** button authenticates the user and redirects them to:
  - **Chat Page** (if login is successful).
  - **Error Message** (if credentials are incorrect).

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture3.png)







# 📝 Register Page

## 📜 Overview
The **Register Page** allows new users to create an account.

## 🎯 Features
- Users must provide:
  - **Email**
  - **Name**
  - **Password**
  - **Gender**
  - **Bio**
  - **Avatar URL**
- Clicking **Register** creates a new user profile.

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture4.png)



# 👤 User Profile Page

## 📜 Overview
After logging in, users can access their **Profile Page** to view and update their personal information.

## 🎯 Features
- View user details.
- **Update profile picture** and **bio** via a pop-up modal.
- Access the **Chat Page** to interact with the AI.

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture5.png)



# 💬 Chat Page

## 📜 Overview
The **Chat Page** allows users to interact with Car Bot in **real-time** using **text or voice input**.

## 🎯 Features
- **Real-time messaging** using **Socket.io**.
- Users can send messages via:
  - **Keyboard (Text Input)**
  - **Microphone (Voice Input)**
- AI responds dynamically using **Wit.ai**.
- AI-generated responses may include:
  - **Text responses**
  - **Images (Unsplash API integration)**

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture7.png)



# 🛠️ Admin Dashboard

## 📜 Overview
When an **Admin User** logs in, they see a **different home page layout** with access to administrative controls.

## 🎯 Features
- **Access to User Management Table**.
- Can **search**, **sort**, and **filter users**:
  - Search by **user name**.
  - Sort by **number of messages**.
  - Filter by **gender**.
- Ability to:
  - **Edit user email & name**.
  - **Delete user profiles**.
  - **Export user data** to **CSV format**.
- Built-in **pagination** for large datasets.

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture8.png)



# 📊 User Management Table (Admin)

## 📜 Overview
The **User Management Table** provides **administrators** with a structured view of all registered users.

## 🎯 Features
- **Search, Sort & Filter** Users:
  - Search by **user name**.
  - Sort by **number of messages**.
  - Filter by **gender**.
- **Manage User Accounts:**
  - **Edit user email & name**.
  - **Delete user profiles**.
  - **Export data** to **CSV format**.
- **Pagination** for improved navigation.

## 🖼️ Screenshot
![Pocetna stranica](./projekat/images/Picture9.png)



# 📈 Data Insights Page

## 📜 Overview
The **Data Insights Page** allows administrators to visualize key data points using charts.

## 🎯 Features
- **User Demographics**:
  - Gender distribution across registered users.
- **User Engagement**:
  - Number of messages exchanged with Car Bot.
- **Car Data Analytics**:
  - Number of car models for each brand.
- **Stock Market Trends**:
  - Car brand stock prices fetched from **Finhub API**.

![Pocetna stranica](./projekat/images/Picture10.png)


