# NexaFlow OrderOps

AI-Powered Manufacturing Order Management System

---

# Overview

NexaFlow OrderOps is a web-based AI manufacturing order management platform that allows users to interact with the system completely through natural language.

Instead of filling complex forms manually, users can communicate with the platform using chat-based instructions to:

* Create manufacturing orders
* Update order statuses
* Log quality reports
* Track orders in real time

The system uses Natural Language Processing (NLP) to extract important details such as:

* Part Name
* Material
* Quantity
* Deadline
* Order Status
* Quality Notes

---

# Features

## 1. NLP Chat Interface

Users can interact with the system using plain English.

### Example Commands

```text
Create 500 aluminum gears due next Friday
```

```text
Update order #2 to In Review
```

```text
Add quality note to order #2: minor surface scratch detected
```

---

## 2. Smart Order Creation

The AI assistant extracts:

* Part name
* Material
* Quantity
* Deadline

and automatically creates a structured order card.

### Initial Status Flow

```text
Received → In Review → Accepted
```

---

## 3. Order Status Management

Users or operations teams can update order status directly through chat.

### Example

```text
Order #4 has been reviewed and accepted
```

---

## 4. Quality Report Logging

Quality checkpoints and inspection notes are stored with timestamps.

### Example

```text
Add quality note to order #3: dimensions verified successfully
```

---

## 5. Real-Time Order Dashboard

The dashboard displays:

* Order ID
* Part Name
* Material
* Quantity
* Deadline
* Current Status
* Latest Quality Notes

---

## 6. User Authentication

The system includes:

* User Registration
* Login Authentication
* Session-based Access Control
* Secure Logout

Only authenticated users can access the dashboard and AI assistant.

---

# Technologies Used

| Technology      | Purpose                |
| --------------- | ---------------------- |
| Html       | Frontend UI            |
| JavaScript      | Application Logic      |
| CSS3            | Styling                |
| Python Flask    | Demo Data Persistence  |
| Gemini API      | NLP Intent Processing  |
| SQLlite    | Icons                  |
| Session Storage | Authentication Session |

---

# Project Structure

```text
src/
│
├── services/
│   └── app.js
│
├── login.html
├── index.html
├── app.py
```

---

# Installation Guide

## Step 1: Clone Repository

```bash
git clone <repository-url>
```

---

## Step 2: Install Dependencies

```bash
npm install
```

---

## Step 3: Start Development Server

```bash
npm run dev
```

---

# Gemini API Setup

This project uses the Gemini API for natural language understanding.

## Get API Key

Visit:

[https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)

Generate your Gemini API key.

---

## Add API Key

After login, the system prompts for:

```text
Gemini API Key
```

Paste the generated API key to enable AI functionality.

---

# Authentication System

## Registration

Users must register before accessing the platform.

### Registration Fields

* Full Name
* Username
* Password
* Confirm Password

---

## Login

Users authenticate using:

* Username
* Password

After successful authentication:

```text
Session Token Generated
→ Dashboard Access Granted
```

---

# Data Persistence

The application stores data using browser localStorage.

## Stored Data

| Storage Key      | Purpose                 |
| ---------------- | ----------------------- |
| orders_data      | Stores orders           |
| chat_history     | Stores conversations    |
| registered_users | Stores registered users |
| gemini_api_key   | Stores Gemini API Key   |

---

# Order Workflow

```text
User Creates Order
        ↓
Status = Received
        ↓
Ops Team Reviews Order
        ↓
Status = In Review
        ↓
Order Accepted
        ↓
Quality Notes Logged
```

---

# Sample Order Object

```json
{
  "id": 1,
  "partName": "Steel Bolt",
  "material": "Stainless Steel",
  "quantity": 500,
  "deadline": "2026-05-20",
  "status": "Received",
  "notes": []
}
```

---

# Sample Quality Note

```json
{
  "id": 1001,
  "text": "Minor scratch detected",
  "timestamp": "2026-05-07 11:30"
}
```

---

# Future Enhancements

* MongoDB Database Integration
* JWT Authentication
* Role-Based Access Control
* Voice Commands
* AI Predictive Analytics
* Email Notifications
* Real-Time Collaboration
* Advanced Dashboard Charts

---

# Security Features

* Protected Dashboard Access
* Session-Based Authentication
* API Key Validation
* Secure Logout

---

# Use Cases

This system is useful for:

* Precision Manufacturing Companies
* Operations Teams
* Quality Inspection Teams
* Manufacturing Workflow Automation
* AI-Based Order Processing

---

# Advantages

* Eliminates manual paperwork
* Simplifies order management
* Real-time order tracking
* AI-powered workflow automation
* User-friendly conversational interface
* Easy integration with modern systems

---

# Author

Developed as an AI-powered manufacturing workflow management project using React and NLP integration.

---

# Team
1) Sharath (https://github.com/1225)
2) Akhilesh Shetty (https://github.com/)
3) Amith S Devadiga (https://github.com/)
4) Pranav (https://github.com/)

---
# License

This project is developed for educational and demonstration purposes.
