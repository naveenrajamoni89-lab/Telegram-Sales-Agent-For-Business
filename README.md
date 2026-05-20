# AI Telegram Ordering Automation Bot

An AI-powered Telegram ordering and payment automation system built using n8n, Google Gemini AI, Telegram Bot API, and Google Sheets.

This workflow automates customer communication, order handling, payment verification, and delivery management through Telegram.

---

## Features

- AI-powered Telegram chatbot
- Automatic order taking
- Payment screenshot detection
- Admin approval workflow
- Real-time customer responses
- Google Sheets order logging
- AI conversation memory
- Delivery status updates
- Automated payment verification flow
- Smart order management system

---

## Tech Stack

- n8n
- Telegram Bot API
- Google Gemini AI
- Google Sheets API
- AI Agent
- Memory Buffer

---

## Workflow Overview

```text
Customer → Telegram Bot
         ↓
AI Agent Handles Order
         ↓
Customer Sends Payment Screenshot
         ↓
Screenshot Forwarded to Admin
         ↓
Admin Approves / Declines
         ↓
Customer Gets Status Update
         ↓
Order Stored in Google Sheets
```

---

## Automation Flow

### 1. Telegram Trigger
Receives customer messages automatically from Telegram.

### 2. AI Agent
Handles:
- customer conversations
- menu responses
- order confirmations
- delivery details
- payment instructions

### 3. Memory System
Stores conversation history for context-aware responses.

### 4. Payment Screenshot Detection
Detects when customers upload payment screenshots.

### 5. Admin Approval System
Automatically forwards payment proof to admin for verification.

### 6. Approval Classification
Classifies admin responses:
- Approved
- Declined

### 7. Google Sheets Integration
Automatically stores:
- Customer Name
- Chat ID
- Phone Number
- Address
- Order Details
- Payment Status
- Order Status
- Timestamp

---

## Google Sheets Format

```text
Order ID | Customer Name | Chat ID | Phone Number | Delivery Address | Order Info | Total Price | Payment Status | Order Status | Timestamp
```

---

## Installation

### 1. Clone Repository

```bash
git clone https://github.com/naveenrajamoni89-lab/calling-agent-.git
```

---

### 2. Install n8n

```bash
npm install n8n -g
```

---

### 3. Start n8n

```bash
n8n start
```

---

## Required Integrations

- Telegram Bot API
- Google Gemini API
- Google Sheets API

---

## Telegram Bot Setup

1. Open BotFather on Telegram
2. Create a new bot
3. Copy Bot Token
4. Add token inside n8n Telegram credentials

---

## Google Gemini Setup

1. Create Gemini API key
2. Add Gemini credentials inside n8n
3. Connect Gemini node to AI Agent

---

## Google Sheets Setup

1. Create Google Sheet
2. Add required columns
3. Connect Google account in n8n
4. Add Sheet ID to workflow

---

## Example Use Cases

- Restaurant ordering system
- Food delivery automation
- AI customer support
- Order management system
- Telegram business automation
- Payment verification workflow

---

## Future Improvements

- WhatsApp Integration
- Voice Ordering
- Multi-language Support
- CRM Integration
- Admin Dashboard
- Analytics System
- AI Sales Agent

---

## Author

**Naveen Rajamoni**

---

## License

This project is licensed under the MIT License.
