# Santosh Academy LLM - Educational Video Platform

A comprehensive LLM-powered educational video platform for Santosh Naira Academy that provides token-based access to educational content.

## Overview

This application integrates educational videos from [Santoshnairacademy.com](https://www.santoshnairacademy.com/) with an AI-powered learning management system. Users purchase tokens to access video content with intelligent features.

## Token System

- **Token Value**: 1 token = 50 minutes of video content
- **Token Price**: ₹20 per token
- **Usage**: Tokens are consumed based on actual viewing time
- **Features**: Real-time token balance tracking and smart notifications

## Core Features

### 🎥 Video Management
- Comprehensive video library integration
- Token-based access control
- Progress tracking and resume functionality
- Quality adaptive streaming

### 🤖 AI Integration
- LLM-powered content recommendations
- Interactive Q&A with video content
- Personalized learning paths
- Smart summary generation

### 💳 Payment & Token System
- Secure token purchasing
- Real-time balance tracking
- Usage analytics and reports
- Flexible pricing tiers

### 👤 User Management
- User authentication and profiles
- Learning progress tracking
- Achievement system
- Social learning features

## Technical Architecture

```
├── frontend/          # React/Next.js web application
├── backend/           # Node.js/Python API server
├── database/          # Database schemas and migrations
├── config/            # Configuration files
└── docs/              # Documentation and API specs
```

## Getting Started

### Prerequisites
- Node.js 18+ or Python 3.9+
- PostgreSQL/MySQL database
- Video streaming service integration
- Payment gateway setup

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd santosh-academy-llm
```

2. Install dependencies:
```bash
# Frontend
cd frontend && npm install

# Backend (Node.js)
cd ../backend && npm install

# Or Backend (Python)
cd ../backend && pip install -r requirements.txt
```

3. Configure environment variables:
```bash
cp config/.env.example config/.env
# Edit configuration as needed
```

4. Set up database:
```bash
# Run migrations
npm run migrate
# Or
python manage.py migrate
```

5. Start the application:
```bash
# Development mode
npm run dev
# Or
python manage.py runserver
```

## API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/refresh` - Token refresh

### Token Management
- `GET /api/tokens/balance` - Get user token balance
- `POST /api/tokens/purchase` - Purchase tokens
- `GET /api/tokens/history` - Token usage history

### Video Access
- `GET /api/videos` - List available videos
- `POST /api/videos/:id/access` - Request video access
- `POST /api/videos/:id/progress` - Update viewing progress

## Development

### Project Structure
- **Frontend**: Modern React/Next.js with TypeScript
- **Backend**: RESTful API with authentication and payment integration
- **Database**: Relational database with optimized queries
- **LLM Integration**: OpenAI/Anthropic API integration for intelligent features

### Key Technologies
- Frontend: React, Next.js, TypeScript, Tailwind CSS
- Backend: Node.js/Express or Python/Django
- Database: PostgreSQL with Prisma/SQLAlchemy ORM
- Authentication: JWT with refresh tokens
- Payment: Razorpay/Stripe integration
- Video: HLS/DASH streaming protocols

## Deployment

The application supports deployment on:
- **Cloud Platforms**: AWS, Google Cloud, Azure
- **Container Orchestration**: Docker, Kubernetes
- **CDN Integration**: CloudFront, CloudFlare
- **Database**: Managed PostgreSQL services

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is proprietary software for Santosh Naira Academy.

## Support

For support and queries:
- Email: support@santoshnairacademy.com
- Documentation: `/docs`
- Issue Tracker: GitHub Issues

---

**Note**: This platform combines traditional educational content delivery with modern AI capabilities to create an enhanced learning experience for students.