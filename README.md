# 🩺 DocSchedule AI

**An AI-powered doctor appointment booking assistant built with n8n, Telegram, Google Gemini, and Google Sheets.**

DocSchedule AI is an automation project that helps users register as patients, discover doctors, check appointment availability, book appointments, and manage existing bookings through a conversational Telegram interface.

![DocSchedule AI Banner](assets/docschedule-banner.png)

## 🤖 Live Demo

Try DocSchedule AI directly on Telegram!

👉 **[Chat with DocSchedule AI](https://t.me/DoctorAppointmentBotAssistantbot)**

Start the bot with `/start` to explore patient registration, doctor search, appointment availability, booking, rescheduling, and cancellation.

> **Note:** This educational demo uses fictional doctor and patient data.

## ✨ Features

- 👤 Patient registration and profile lookup
- 🔎 Doctor discovery by specialty
- 📅 Appointment availability checking
- ✅ Appointment booking and confirmation
- 🔄 Appointment rescheduling
- ❌ Appointment cancellation
- 📊 Google Sheets-based appointment record management
- 🤖 AI-powered conversational interaction

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| n8n | Workflow automation and orchestration |
| Telegram Bot API | Conversational interface |
| Google Gemini | Natural language understanding |
| Google Sheets | Doctor, patient, and appointment data |

## 🏗️ Workflow Architecture

1. A user starts a conversation with the Telegram bot.
2. The workflow checks the patient's registration status.
3. The AI assistant interprets the user's request.
4. Connected tools retrieve doctor, patient, and appointment information.
5. Availability is checked before booking or rescheduling.
6. The workflow updates Google Sheets and returns the result to the user.

## 📸 Project Screenshots

### 1. n8n Workflow Architecture

The main automation workflow connects the AI assistant with Telegram and the supporting appointment-management tools.

![DocSchedule AI n8n Workflow](https://github.com/CharudattaLende/docschedule-ai/blob/main/Screenshot%202026-10-15%20200721.png?raw=true)

### 2. Telegram Bot Conversation

A demonstration of the DocSchedule AI conversational interface.

![DocSchedule AI Telegram Conversation](https://github.com/CharudattaLende/docschedule-ai/blob/main/Screenshot%202026-10-15%20213515.png?raw=true)

## 📂 Repository Structure

The repository currently contains the main Telegram workflow and separate tool workflows.

```text
docschedule-ai/
├── Doctor Appointment Telegram Bot.json
├── Tool - Book Appointment.json
├── Tool - Cancel Appointment.json
├── Tool - Get All Appointments.json
├── Tool - Get Available Appointments.json
├── Tool - Get Doctor Config.json
├── Tool - Get Patient.json
├── Tool - Register Patient.json
├── Tool - Reschedule Appointment.json
└── README.md
```

## 🚀 Setup Instructions

### Prerequisites

- An n8n instance
- A Telegram bot created through BotFather
- A Google account with Google Sheets
- A Google Gemini API key

### Installation

1. Clone or download this repository.
2. Import the main workflow JSON into n8n.
3. Import the individual tool workflows if they are separate workflows.
4. Configure your own Telegram, Google Sheets, and Gemini credentials.
5. Connect the tools and configure any required workflow IDs or references.
6. Create a Google Sheets document with the expected column headers.
7. Test patient registration, doctor search, booking, rescheduling, and cancellation.

**Important:** Imported workflows may require configuration before they work. Never publish API keys, bot tokens, webhook secrets, or real patient information.

## 🧪 Demo and Testing

This project uses fictional doctor and patient data for demonstration.

Test scenarios include:

- Registering a new patient
- Finding a doctor by specialty
- Checking available time slots
- Booking an appointment
- Rescheduling an existing appointment
- Cancelling an appointment

## 🔒 Disclaimer

This is an educational automation project, not a production-ready healthcare system. It is not intended for real patient data or medical diagnosis. Production deployment would require appropriate privacy, security, access control, reliability, and healthcare compliance measures.

## 👨‍💻 Author

**Charudatta Lende**

Computer Science Engineering Student | AI Automation & Software Development

- GitHub: [CharudattaLende](https://github.com/CharudattaLende)
- Portfolio: [charudattaportfolio.vercel.app](https://charudattaportfolio.vercel.app/)

---

If you find this project interesting, consider giving the repository a ⭐!
