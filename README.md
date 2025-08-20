# Patient Appointment Scheduler

This n8n workflow automates patient appointment scheduling for a medical chamber (SK Clinic). It uses AI to interact with patients and manage calendar appointments.

## Workflow Overview

1. **Chat Trigger**: Receives patient messages
2. **AI Agent**: Handles conversation flow and decision making
3. **Google Gemini**: Provides the AI language model
4. **Calendar Tools**:
   - `check_calendar_availability`: Finds available time slots
   - `create_calendar_appointment`: Books appointments
5. **Notification**: Sends confirmation via Discord

## Key Features

- Automated appointment scheduling in Google Calendar
- Time slot availability checking
- Patient confirmation notifications
- Conversation memory for context
- Uses UTC+6 timezone for all operations

## Requirements

- Google Gemini API credentials
- Google Calendar API credentials
- Discord webhook for notifications

## Usage

The AI agent follows these steps:
1. Asks for preferred appointment day
2. Checks calendar availability
3. Shows available slots and confirms selection
4. Collects patient details (name & email)
5. Books appointment
6. Sends confirmation

For cancellation, patients can call +8801718432571.