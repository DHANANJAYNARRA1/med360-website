# Med360 Website Deployment Guide

## Quick Deploy to Vercel

### Option 1: Using Vercel CLI (Recommended)
```bash
# Install Vercel CLI
npm install -g vercel

# Login to Vercel (if not already logged in)
vercel login

# Deploy the project
vercel
```

### Option 2: Using GitHub
1. Push your code to a GitHub repository
2. Go to [vercel.com](https://vercel.com)
3. Click "Add New Project"
4. Select your GitHub repository
5. Click "Deploy"

## Project Structure (Required for Vercel)
```
med360-website/
├── med360.html      # Main website file (at root level)
├── logo.svg         # Logo file (at root level)
├── vercel.json      # Vercel configuration
└── README.md        # This file
```

## Current Configuration
- The website is a single HTML file with embedded CSS and JavaScript
- All external resources (CDN links for fonts, icons, EmailJS) are already configured
- The `vercel.json` file ensures all routes serve the main HTML file

## Features
- Fully responsive design
- Hero section with phone mockup
- "How It Works" journey section
- Services overview
- Contact form with EmailJS integration
- Smooth scroll navigation

## Notes
- The contact form uses EmailJS - you'll need to configure your own EmailJS public key
- Currently uses CDN for Font Awesome icons which works on Vercel
- **Important**: Keep files at root level (not in subfolder) for Vercel to work properly