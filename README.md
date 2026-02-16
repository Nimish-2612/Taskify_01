# Taskify

A full-stack web application for managing tasks and todos with integrated Google Calendar support and authentication.

## Features

- **User Authentication**: Secure login and signup with session management
- **Todo Management**: Create, update, and track your daily tasks
- **Google Calendar Integration**: Sync tasks with your Google Calendar
- **Dashboard**: Visual overview of your tasks and progress
- **Progress Tracking**: Monitor your task completion with progress bars
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack

- **Backend**: Node.js with Express.js
- **Frontend**: EJS templating, HTML/CSS, JavaScript
- **Database**: MySQL/Database connection
- **Authentication**: Session-based authentication with Google OAuth
- **Styling**: Custom CSS with modular organization

## Project Structure

```
Taskify/
├── app.js                 # Main application entry point
├── package.json           # Project dependencies
├── config/               # Configuration files
├── controller/           # Route controllers
├── data/                 # Database connections
├── middlewares/          # Custom middleware
├── models/               # Database models
├── public/               # Static assets
│   ├── images/
│   ├── scripts/
│   └── styles/
├── routes/               # API routes
├── util/                 # Utility functions
└── views/                # EJS templates
```

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Nimish-2612/Taskify.git
   cd Taskify
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory:
   ```
   DATABASE_URL=your_database_url
   SESSION_SECRET=your_session_secret
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   PORT=3000
   ```

4. **Start the application**
   ```bash
   npm start
   ```

The application will be available at `http://localhost:3000`

## Usage

- **Sign Up**: Create a new account with email and password
- **Login**: Access your account securely
- **Add Tasks**: Create new todos from the dashboard
- **Manage Tasks**: Update, complete, or delete existing tasks
- **Calendar Sync**: Add tasks to your Google Calendar
- **Track Progress**: Monitor completion rates with visual progress indicators

## Features by Module

### Authentication (`controller/auth.controller.js`)
- User registration and login
- Session management
- Password validation

### Todo Management (`controller/todos.controller.js`)
- Create, read, update, delete todos
- Task status tracking
- Priority and date management

### Google Integration (`controller/google.controller.js`)
- OAuth authentication
- Calendar event creation
- Calendar synchronization

### Dashboard (`views/landing/dashboard.ejs`)
- Task overview
- Progress visualization
- Quick task creation

## Security Features

- Protected routes with authentication middleware
- Session-based security
- Environment variable protection
- Input validation and sanitization

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

**Nimish-2612** - [GitHub Profile](https://github.com/Nimish-2612)

**Happy Task Managing! 🚀**
