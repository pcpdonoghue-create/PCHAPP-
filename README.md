# PCH Email Subscription Backend

Backend API powering the PCH email subscription system. This service handles subscriber registration, sends welcome emails, and notifies the admin when new users subscribe.

## Features

- Email subscription endpoint
- Welcome email sent to new subscribers
- Admin notification for new sign-ups
- Email validation
- Unsubscribe support
- Health check endpoint

## Tech Stack

- Node.js
- Express
- SendGrid Email API
- CORS

## Installation

Clone the repository and install dependencies.

```bash
git clone https://github.com/pcpdonoghue-create/PCHAPP-.git
cd backend
npm install
```

## Environment Variables

Create a ".env" file in the backend folder and add:

```bash
SENDGRID_API_KEY=your_sendgrid_api_key
FROM_EMAIL=pchappblog@gmail.com
ADMIN_EMAIL=pchappblog@gmail.com
PORT=3001
```

## Running the Server

Start the backend server with:

```bash
npm start
```

Server will run on: http://localhost:3001

## API Endpoints

### Subscribe
- **POST** `/api/subscribe` - Adds a new subscriber and sends a welcome email.

### Unsubscribe
- **POST** `/api/unsubscribe` - Removes a subscriber from the mailing list.

### Subscriber Count
- **GET** `/api/subscribers/count` - Returns the total number of subscribers.

### Health Check
- **GET** `/api/health` - Checks if the server is running.

## Deployment

The backend can be deployed using cloud platforms such as Render or other Node.js hosting services.

## License

This project is open for educational and development purposes.