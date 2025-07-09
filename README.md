# Cresento - AI Shin Guards Website

A high-end website for Cresento, an AI-powered shin guards company that tracks athlete performance metrics and provides instant AI coaching feedback.

## Project Structure

```
Cresento/
├── cresento-frontend/          # React frontend application
│   ├── src/
│   │   ├── components/
│   │   │   ├── auth/          # Authentication components
│   │   │   ├── common/        # Reusable components
│   │   │   ├── layout/        # Layout components
│   │   │   └── pages/         # Page components
│   │   ├── contexts/          # React contexts
│   │   ├── types/            # TypeScript types
│   │   └── utils/            # Utility functions
│   └── public/               # Static assets
└── cresento-backend/          # Node.js backend API
    ├── server.js             # Main server file
    ├── package.json          # Dependencies
    └── .env                  # Environment variables
```

## Features

### Frontend Features
- **Landing Page**: Video hero section with product introduction
- **About Us**: Company mission, team, and technology
- **Product Showcase**: Detailed product information and gallery
- **Features**: Interactive feature exploration
- **Pricing**: Subscription plans and pricing tiers
- **Contact**: Contact form and company information
- **Authentication**: User registration and login
- **Dashboard**: User performance tracking (placeholder)
- **Newsletter**: Email subscription functionality

### Backend Features
- **User Authentication**: JWT-based authentication
- **Newsletter Management**: Email subscription handling
- **Contact Form**: Message submission and storage
- **Database**: SQLite database for data persistence
- **API Security**: Input validation and error handling

### Design Features
- **Dark Theme**: Black background with dark green accents
- **Premium Design**: High-end aesthetic for luxury customers
- **Responsive**: Mobile-first responsive design
- **Animations**: Smooth transitions using Framer Motion
- **Typography**: Inter and Montserrat fonts

## Technology Stack

### Frontend
- React 18 with TypeScript
- Tailwind CSS for styling
- React Router for navigation
- Framer Motion for animations
- Lucide React for icons
- Axios for API calls

### Backend
- Node.js with Express
- SQLite database
- JWT authentication
- bcrypt for password hashing
- CORS for cross-origin requests
- Nodemailer for email functionality

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Cresento
   ```

2. **Start the backend:**
   ```bash
   cd cresento-backend
   npm install
   npm run dev
   ```

3. **Start the frontend:**
   ```bash
   cd cresento-frontend
   npm install
   npm start
   ```

4. **Access the application:**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

## Configuration

### Frontend Configuration
- Update API endpoints in the frontend code if needed
- Add your video file to `public/demo-video.mp4`
- Customize colors in `tailwind.config.js`

### Backend Configuration
- Update `.env` file with your settings:
  ```
  PORT=5000
  JWT_SECRET=your-secret-key
  NODE_ENV=development
  ```

## Deployment

### Frontend Deployment
The frontend can be deployed to:
- Netlify
- Vercel
- AWS S3 + CloudFront
- Any static hosting service

### Backend Deployment
The backend can be deployed to:
- Heroku
- AWS EC2
- DigitalOcean
- Railway

## API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Newsletter Endpoints
- `POST /api/newsletter/subscribe` - Subscribe to newsletter

### Contact Endpoints
- `POST /api/contact` - Submit contact form

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For support, contact the development team or create an issue in the repository.

## Future Enhancements

- Payment integration (Stripe/PayPal)
- Real-time dashboard with WebSocket
- Mobile app development
- Advanced analytics
- Email marketing automation
- Multi-language support