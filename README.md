# 🤝 AidMatch AI

<div align="center">
  <p><strong>Smart Resource Allocation System for NGOs and Social Organizations</strong></p>
</div>

## 📖 Project Overview

### The Problem
During crises, natural disasters, or community outreach programs, identifying exact needs and matching them with available resources quickly is a logistical nightmare. Often, resources are misallocated, delayed, or fail to reach those with the most urgent needs due to manual processing and lack of real-time insights.

### The Solution
**AidMatch AI** is an intelligent, automated resource allocation system. It collects community needs, processes them using advanced AI to classify the request type, determines the urgency (priority level), and instantly matches them with the most suitable available resources (volunteers, supplies, etc.). This ensures a faster, more efficient, and impactful response.

### Real-World Use Cases
- **Disaster Relief:** Rapidly processing SOS requests and dispatching rescue volunteers or medical supplies based on urgency.
- **Community Outreach:** Matching community needs (food, education, shelter) with available local NGO resources.
- **Volunteer Management:** Automatically assigning tasks to volunteers based on the requirements of an incoming request.

---

## ✨ Features

- 🧠 **AI-Based Need Classification:** Automatically categorizes needs (e.g., Medical, Food, Shelter) using AI analysis.
- 🚨 **Priority Detection:** Intelligently assigns priority levels (**High**, **Medium**, **Low**) based on the context of the request.
- 🎯 **Smart Resource Allocation:** Seamlessly matches available resources or volunteers to the identified needs.
- 📊 **Real-Time Dashboard:** A modern, intuitive interface to monitor available resources, total needs, and urgent requests at a glance.
- 🕒 **History Tracking:** Keeps a detailed log of all processed requests, assignments, and outcomes for transparency and auditing.

---

## 🛠️ Tech Stack

- **Frontend:** Antigravity UI (HTML, CSS, JavaScript) for a modern, responsive, card-based aesthetic.
- **Backend:** Node.js with Express (RESTful APIs).
- **AI Integration:** Claude API for natural language processing and smart classification.
- **Data Integration:** Stitch for seamless data flow.
- **Database:** MongoDB (or simulated local data for development) to store needs, resources, and history logs.

---

## 🏗️ System Architecture

1. **Frontend (User Interface):** Users submit a need through the "Add Need" interface. The dashboard continuously fetches and displays resource metrics and allocation status.
2. **Backend (Node.js/Express):** Acts as the middleman. It receives the need data from the frontend and sends it to the AI service.
3. **AI Engine (Claude API):** Processes the text of the need, extracts the category, determines the priority, and suggests resource allocation.
4. **Database (MongoDB):** Stores the newly processed need, updates the available resource counts, and logs the transaction.
5. **Data Integration (Stitch):** Facilitates the smooth synchronization of data between the backend and the database.

---

## 🚀 Installation & Setup

Follow these steps to get the project running locally.

### Prerequisites
- [Node.js](https://nodejs.org/) installed
- [MongoDB](https://www.mongodb.com/) installed and running (or a MongoDB Atlas cluster)

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/AidMatch-AI.git
cd AidMatch-AI
```

### 2. Install Dependencies
```bash
# Navigate to the backend directory (if applicable) and install
npm install
```

### 3. Environment Variables
Create a `.env` file in the root directory and add necessary API keys and database URIs:
```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
CLAUDE_API_KEY=your_claude_api_key
```

### 4. Run the Backend Server
```bash
npm start
# or for development:
npm run dev
```

### 5. Open the Frontend
If the frontend is served statically, simply open `index.html` in your browser, or use a tool like Live Server.

---

## 💡 Usage Guide

1. **Dashboard Overview:** Upon opening the app, view the main dashboard to see "Available Resources," "Total Needs," and "Urgent Requests."
2. **Add a Need:** Navigate to the "Add Need" section. Enter the details of the community requirement.
3. **Analyze & Allocate:** Instead of standard submission, click "Analyze & Allocate".
4. **AI Processing:** The system will use AI to analyze the text, automatically assign a priority level (High/Medium/Low), and categorize the request.
5. **Resource Matching:** View the Results presentation to see exactly which resources/volunteers have been allocated to the specific need.

---

## 📂 Project Structure

```text
AidMatch-AI/
├── backend/                  # Node.js Express server
│   ├── routes/               # API endpoints
│   ├── controllers/          # Logic for handling requests
│   ├── models/               # MongoDB schemas
│   └── server.js             # Entry point
├── frontend/                 # UI components
│   ├── index.html            # Main Dashboard
│   ├── add-need.html         # Add Need Page
│   ├── needs-list.html       # Results & Allocations
│   ├── styles.css            # Antigravity UI styling
│   └── script.js             # Frontend logic & API calls
├── .env.example              # Environment variables template
├── package.json              # Project metadata and dependencies
└── README.md                 # Project documentation
```

---

## 📸 Screenshots

### Dashboard UI
![Dashboard UI](placeholder-dashboard.png)
*Real-time metrics and overall system status.*

### Add Need Page
![Add Need Page](placeholder-add-need.png)
*Interface for submitting new community requirements.*

### Results & Allocation Page
![Results Page](placeholder-results.png)
*AI analysis results showing priority, category, and assigned resources.*

---

## 🔮 Future Improvements

- **Real-Time Alerts:** Implement WebSocket or Push Notifications for immediate alerts on High-Priority needs.
- **Map Integration:** Add geospatial visualization to map needs and resources geographically.
- **Multi-NGO Collaboration:** Allow different organizations to connect, share resources, and handle overflow needs collaboratively.

---

## 👥 Team

- **[Team Member 1 Name]** - [Role/Contribution] - [GitHub Profile Link]
- **[Team Member 2 Name]** - [Role/Contribution] - [GitHub Profile Link]

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
