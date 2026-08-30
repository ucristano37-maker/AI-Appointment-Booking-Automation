# Appointment Booking Workflow

## Flow

1. **Booking Request** starts the workflow.
2. **Customer Request** contains the incoming booking message.
3. **Build Booking Prompt** prepares structured instructions for the AI.
4. **AI Booking Input** prepares the request for an AI provider.
5. Connect the AI step to a calendar provider to check availability and create the appointment.
6. Send a confirmation only after the booking is successfully created.

## Production Notes

Use n8n credentials for API authentication. Validate timezone, date, service, and required customer details before creating an appointment. Never store real secrets in GitHub.
