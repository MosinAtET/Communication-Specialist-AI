# SocialMediaAI

A comprehensive social media management platform with AI-powered content generation and scheduling capabilities.

## Features

- **AI-Powered Content Generation**: Generate engaging social media posts using advanced AI models
- **Multi-Platform Support**: Post to multiple social media platforms (Twitter, LinkedIn, Dev.to, etc.)
- **Smart Scheduling**: Schedule posts at optimal times for maximum engagement
- **Content Analytics**: Track performance and engagement metrics
- **Modern Web Interface**: React-based frontend with intuitive UI

## Tech Stack

### Backend
- **FastAPI**: Modern, fast web framework for building APIs
- **SQLAlchemy**: SQL toolkit and ORM
- **Google Generative AI**: AI content generation
- **APScheduler**: Task scheduling
- **Multiple Social Media APIs**: Twitter, LinkedIn, Dev.to integration

### Frontend
- **React**: Modern JavaScript library for building user interfaces
- **TypeScript**: Type-safe JavaScript
- **Vite**: Fast build tool and development server

## Project Structure

```
SocialMediaAI/
├── backend/                 # FastAPI backend
│   ├── app/                # Main application code
│   ├── test/               # Test files
│   └── venv/               # Python virtual environment
├── frontend/               # React frontend
│   ├── src/                # Source code
│   ├── public/             # Static assets
│   └── package.json        # Node.js dependencies
└── README.md              # This file
```

## Getting Started

### Prerequisites

- Python 3.8+
- Node.js 16+
- Git

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp env.example .env
   # Edit .env with your API keys and configuration
   ```

5. Run the development server:
   ```bash
   uvicorn app.main:app --reload
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## Environment Variables

Create a `.env` file in the backend directory with the following variables:

```env
# Database
DATABASE_URL=your_database_url

# AI Services
GOOGLE_API_KEY=your_google_api_key

# Social Media APIs
TWITTER_API_KEY=your_twitter_api_key
TWITTER_API_SECRET=your_twitter_api_secret
TWITTER_ACCESS_TOKEN=your_twitter_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_twitter_access_token_secret

LINKEDIN_CLIENT_ID=your_linkedin_client_id
LINKEDIN_CLIENT_SECRET=your_linkedin_client_secret

DEVTO_API_KEY=your_devto_api_key

# Application Settings
SECRET_KEY=your_secret_key
DEBUG=True
```

## API Documentation

Once the backend is running, you can access the interactive API documentation at:
- Swagger UI: `http://localhost:8000/docs`
- ReDoc: `http://localhost:8000/redoc`

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue on GitHub or contact the development team. 