# Auth Frontend - React.js

A modern authentication frontend built with React.js, TypeScript, and Tailwind CSS that integrates with a Laravel API backend.

## Features

- 🔐 **Authentication**: Login and registration forms
- 🎨 **Modern UI**: Beautiful, responsive design with Tailwind CSS
- 🔒 **Token Management**: Secure token storage and automatic API authentication
- 📱 **Responsive**: Works perfectly on desktop and mobile devices
- ⚡ **Fast**: Built with React.js for optimal performance
- 🛡️ **Type Safe**: Full TypeScript support

## Prerequisites

- Node.js 18+ and npm
- Laravel API backend running on `http://localhost:8000`

## Installation

1. **Clone the repository:**
   ```bash
   git clone <your-github-repo-url>
   cd auth-frontend-reactjs
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm start
   ```

4. **Open your browser:**
   Navigate to `http://localhost:3001` (React.js will run on port 3001)

## API Configuration

The app is configured to connect to a Laravel API at `http://localhost:8000/api`. To change this:

1. Edit `src/services/api.ts`
2. Update the `API_BASE_URL` constant

## Available Scripts

- `npm start` - Start development server
- `npm run build` - Build for production
- `npm test` - Run tests
- `npm run eject` - Eject from Create React App (not recommended)

## Project Structure

```
src/
├── components/         # React components
│   ├── Dashboard.tsx   # User dashboard
│   ├── LoginForm.tsx   # Login form
│   └── RegisterForm.tsx # Registration form
├── context/           # React context providers
│   └── AuthContext.tsx # Authentication context
├── services/          # API services
│   └── api.ts         # API client configuration
├── types/             # TypeScript type definitions
│   └── auth.ts        # Authentication types
├── App.tsx            # Main app component
├── index.tsx          # App entry point
└── index.css          # Global styles
```

## Authentication Flow

1. **Login/Register**: Users can sign in or create new accounts
2. **Token Storage**: JWT tokens are stored in localStorage
3. **Protected Routes**: Dashboard is only accessible when authenticated
4. **Auto-logout**: Invalid tokens automatically log out users

## API Endpoints Used

- `POST /api/register` - User registration
- `POST /api/login` - User login
- `GET /api/me` - Get current user info
- `POST /api/logout` - User logout

## Technologies Used

- **React.js 18** - Frontend library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Axios** - HTTP client
- **React Context** - State management
- **Create React App** - Development environment

## Deployment

To deploy to production:

1. **Build the application:**
   ```bash
   npm run build
   ```

2. **Deploy to your preferred platform:**
   - Netlify (recommended for React apps)
   - Vercel
   - AWS S3 + CloudFront
   - Or any other hosting service

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License




