# Icon to PowerPoint Generator

A web application that allows users to input a list of icon names and generates a PowerPoint presentation with those icons.

## Features

- React frontend with clean, modern UI
- FastAPI backend with icon search and PowerPoint generation
- Iconify API integration for finding icons
- Automatic PowerPoint file download
- Grid layout with icon labels
- Error handling and loading states

## Tech Stack

- **Frontend**: React + TypeScript
- **Backend**: Python + FastAPI
- **PowerPoint Generation**: python-pptx
- **Icon Search**: Iconify API
- **Deployment**: Railway

## Local Development

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the backend server:
   ```bash
   python main.py
   ```

The backend will be available at `http://localhost:8000`

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
   npm start
   ```

The frontend will be available at `http://localhost:3000`

## Usage

1. Enter icon names in the text area (one per line)
2. Click "Generate PowerPoint" 
3. The PowerPoint file will download automatically

## Railway Deployment

1. Connect your GitHub repository to Railway
2. Deploy the backend as a Python service
3. Deploy the frontend as a static site
4. Update the API URL in the frontend to point to your deployed backend

## API Endpoints

- `GET /` - Health check
- `POST /search-icons` - Search for icons by name
- `POST /generate-powerpoint` - Generate PowerPoint with icons