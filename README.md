# AI-Powered Travel Itinerary Generator

A modern full-stack application that generates personalized travel itineraries using AI.

## Features

- **AI Generation**: Custom itineraries based on destination, dates, interests, and budget.
- **Real-time Streaming**: Watch your itinerary being built step-by-step.
- **Itinerary Management**: Save, view, and delete your generated travel plans.
- **Beautiful UI**: Modern, responsive design with a travel-inspired aesthetic.

## Tech Stack

- **Frontend**: React, TypeScript, Vite, Tailwind CSS, Framer Motion, Lucide Icons.
- **Backend**: Node.js, Express, TypeScript.
- **Database**: PostgreSQL with Drizzle ORM.
- **AI**: OpenAI (GPT-5.2) via Replit AI Integrations.

## Prerequisites

- [Node.js](https://nodejs.org/) (v20 or higher recommended)
- [PostgreSQL](https://www.postgresql.org/) database
- [FFmpeg](https://ffmpeg.org/) (required for audio processing features)

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone <your-repo-url>
   cd travel-itinerary-generator
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure Environment Variables**:
   Create a `.env` file in the root directory with the following variables:
   ```env
   DATABASE_URL=postgres://username:password@localhost:5432/database_name
   AI_INTEGRATIONS_OPENAI_API_KEY=your_openai_api_key
   AI_INTEGRATIONS_OPENAI_BASE_URL=https://api.openai.com/v1
   SESSION_SECRET=your_secret_session_key
   ```
   *Note: In the Replit environment, the AI secrets are managed automatically.*

4. **Initialize the Database**:
   Run the schema push command to set up your tables:
   ```bash
   npm run db:push
   ```

5. **Start the Development Server**:
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:5000`.

## Scripts

- `npm run dev`: Starts both the Express backend and Vite frontend development servers.
- `npm run build`: Builds the application for production.
- `npm run start`: Runs the built application.
- `npm run db:push`: Syncs the Drizzle schema with the database.
- `npm run db:studio`: Opens Drizzle Studio to explore your data.

## Project Structure

- `client/`: React frontend source code.
- `server/`: Express backend and database storage logic.
- `shared/`: Shared types and database schemas.
- `attached_assets/`: Static assets and imagery.
