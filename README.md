# Fake News Detection Web App

A modern web application for detecting fake news using Google Fact Check Tools API.

## Features

- 🔍 Real-time fact-checking using Google Fact Check API
- ✅ Simple TRUE/FAKE result display
- 🎨 Modern and responsive UI
- ⚡ Fast and lightweight

## How It Works

1. Enter news text or a claim in the textarea
2. Click "Analyze News"
3. The app searches Google's fact-check database
4. Results show either **REAL NEWS** or **FAKE NEWS**

## Logic

- If the text contains a comma (`,`), it's marked as **FAKE NEWS**
- If there are 4 or more false/misleading reviews → **FAKE NEWS**
- If there are less than 4 false/misleading reviews → **REAL NEWS**
- If no results found → **REAL NEWS**

## Deployment on Vercel

### Option 1: Deploy via Vercel Dashboard

1. Go to [vercel.com](https://vercel.com)
2. Sign in with your GitHub account
3. Click "New Project"
4. Import the repository `Prabuddha747/Fake-new`
5. Vercel will automatically detect it as a static site
6. Click "Deploy"

### Option 2: Deploy via Vercel CLI

```bash
# Install Vercel CLI globally
npm i -g vercel

# Navigate to project directory
cd "fake new detection using api"

# Deploy
vercel

# Follow the prompts to complete deployment
```

## Project Structure

```
.
├── index.html          # Main application file
├── .gitignore         # Git ignore file
└── README.md          # This file
```

## API Configuration

The app uses Google Fact Check Tools API. The API key is embedded in the code. For production, consider using environment variables.

## Live Demo

After deployment, your app will be available at a Vercel URL like:
`https://fake-new-xxx.vercel.app`

## Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- Google Fact Check Tools API

## License

MIT License

