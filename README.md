
# ♻️ EcoVision - Smart Waste Management Platform

A smart, AI-powered web platform designed to help users identify, recycle, and responsibly dispose of waste items. Users can scan items using a camera or upload an image, and our AI model provides accurate waste classification with eco-friendly disposal suggestions.

## Features

- **User Authentication**  
  - Sign up and login functionality using Firebase Authentication with email/password and Google sign-in.

- **Smart Waste Scanner**  
  - Upload an image or use your camera to scan a waste item.
  - Powered by **Google Gemini 2.0 Flash** for fast and accurate classification.
  - The system classifies the waste into one of four categories:
    - **Recyclable** - Items that can be recycled
    - **Compostable** - Organic waste that can be composted
    - **Special** - Items requiring special disposal (e-waste, batteries, chemicals)
    - **Landfill** - Items that must go to landfill
  - Provides detailed disposal instructions and environmental impact information.

- **AI-Powered Chatbot**  
  - Get instant assistance on waste disposal, recycling tips, and eco-friendly practices.
  - Powered by **Google Gemini** for fast, intelligent responses.

- **Dark and Light Theme Support**

- **Informational Pages**
  - About Page
  - Guide Page (with recycling tips and category info)
  - Contact Page

## Tech Stack

| Layer     | Technology                    |
|-----------|-------------------------------|
| Frontend  | React (Vite) + Tailwind CSS + ShadCN UI |
| Backend   | Node.js / Express + TypeScript |
| Database  | Firebase (Authentication & Storage) |
| AI/ML     | Google Gemini 2.0 Flash (Vision + Chat) |
| Auth      | Firebase Authentication       |

## How It Works

1. **Sign up or Login** to access the platform.
2. **Upload or scan a waste item** using the camera or file picker.
3. **Get instant AI analysis** powered by Google Gemini 2.0 Flash:
   - Accurate waste category identification
   - Detailed disposal instructions
   - Environmental impact information
4. **Chat with the AI assistant** for personalized waste management advice.

## Project Structure

```
EcoVision/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/    # UI components
│   │   ├── pages/         # Page components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utilities and configs
│   │   └── App.tsx        # Main app component
│   └── index.html
├── server/                # Express backend
│   ├── gemini.ts         # Gemini AI integration
│   ├── routes.ts         # API routes
│   ├── firebase-auth.ts  # Firebase authentication
│   ├── simple-storage.ts # Data storage
│   └── index.ts          # Server entry point
├── package.json
└── README.md
---

Made with ♻️ for a sustainable future
